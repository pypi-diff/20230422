# Comparing `tmp/triplify_csv-0.2.1.tar.gz` & `tmp/triplify_csv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.2.1.tar", max compression
+gzip compressed data, was "triplify_csv-0.2.2.tar", max compression
```

## Comparing `triplify_csv-0.2.1.tar` & `triplify_csv-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1526 2022-01-03 13:53:09.772724 triplify_csv-0.2.1/LICENSE
--rw-r--r--   0        0        0     7042 2022-06-24 22:32:46.702602 triplify_csv-0.2.1/README.md
--rw-r--r--   0        0        0      585 2022-06-24 22:49:25.643525 triplify_csv-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2021-12-28 19:22:13.383258 triplify_csv-0.2.1/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    17258 2022-06-22 14:27:52.678102 triplify_csv-0.2.1/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     8219 2022-06-24 22:57:19.898108 triplify_csv-0.2.1/setup.py
--rw-r--r--   0        0        0     7827 2022-06-24 22:57:19.898756 triplify_csv-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7042 2023-04-03 19:59:17.539697 triplify_csv-0.2.2/README.md
+-rw-r--r--   0        0        0      568 2023-04-21 08:39:08.590347 triplify_csv-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.2.2/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    17486 2023-04-21 08:17:19.466388 triplify_csv-0.2.2/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     7839 1970-01-01 00:00:00.000000 triplify_csv-0.2.2/PKG-INFO
```

### Comparing `triplify_csv-0.2.1/LICENSE` & `triplify_csv-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.2.1/README.md` & `triplify_csv-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.2.1/triplify_csv/triplify_csv.py` & `triplify_csv-0.2.2/triplify_csv/triplify_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from rdflib import Graph, Literal, URIRef, Namespace, Dataset, BNode
+from rdflib import Graph, Literal, URIRef, Dataset, BNode
 import csv
-from rdflib.plugins import sparql
-from rdflib.namespace import XSD, RDF, FOAF 
+#from rdflib.plugins import sparql
+from rdflib.namespace import XSD, RDF, FOAF, Namespace
 import re
 from itertools import takewhile
 import os
 import sys, getopt
 import urllib.parse
 from datetime import datetime
 import click
@@ -47,14 +47,18 @@
 		self.set_column_names()
 		return self
 		
 	def __exit__(self, *args):
 		if self.csvfile:
 			self.csvfile.close()
 			
+	def closefile(self):
+		if self.csvfile:
+			self.csvfile.close()
+					
 			
 	def get_restarted_reader(self):
 		if self.csvfile.closed:
 			self.reset_file()
 		self.csvfile.seek(0)
 		return self.reader
 		
@@ -109,14 +113,19 @@
 				self.csvInfoList.append(csvInfo)
 				self.csv_tables.append(csvInfo.tablename)
 				# append errors
 				for err in csvInfo.errors:
 					self.errors.append(err)
 					
 					
+	def close_csvs(self):
+		for csvInfo in self.csvInfoList:
+			csvInfo.closefile()
+					
+					
 	# get the csvinfo that matches this tablename
 	def get_csvInfo_by_tablename(self, tablename):
 		for csvInfo in self.csvInfoList:
 			if csvInfo.tablename == tablename:
 				return csvInfo
 		return None
 		
@@ -133,26 +142,27 @@
 			#       if just one return it
 			if len(buf) == 1:
 				self.base= re.findall(r'<([^>]+)>', ''.join(buf))[0]
 				
 	
 	def get_baseURI(self):
 		return self.base
-		
+	
+	'''	
 	def runSparql(self,qstring):
 		base = Namespace(URIRef(self.base))
 		
 		rr = Namespace("http://www.w3.org/ns/r2rml#")
 		#self.g.bind("base", base)
 		
 		self.g.namespace_manager.bind('', base)
 		q = sparql.prepareQuery(qstring,initNs= {"" : base,"xsd" : XSD, "rdf" : RDF, "rr" : rr})
 		
 		return self.g.query(q)
-		
+	'''	
 
 	def tmaps(self):
 		tmaps = {}
 		# for each triplemap add a list of dict for predicateObjectMaps called 'poms'
 		for tm, p, o in self.g.triples((None, RDF.type, URIRef(rr('TriplesMap')))):
 			tmaps[str(tm)] = {
 				'poms' : [],
@@ -409,14 +419,17 @@
 				# cols mentioned in template that are not cols in csv
 				self.errors.append('Fields are named in a template that are not columns in a CSV file.')
 		# add every namespace from rml file to outputted triple/quad file
 		for n in self.g.namespace_manager.namespaces():
 			self.triples.namespace_manager.bind(n[0],n[1])
 		self.triples.namespace_manager.bind('rdf', RDF)	
 	
+		# close any open input files
+		self.close_csvs()
+	
 	def get_literal(self, value, dateformat='%Y-%m-%d', lang=''):
 		
 		try:
 			dt = datetime.strptime(value,dateformat).date()
 			return Literal(dt, datatype=XSD.date)
 		except ValueError:
 			pass
@@ -481,11 +494,12 @@
 	try:
 	    s.write_file(outfile)
 	except Exception as err:
 	    print("Error outputting graph: {0}".format(err))
 	    raise
 	for e in s.errors:
 		print(e)
+		
 	
 if __name__ == "__main__":
 	process()
```

### Comparing `triplify_csv-0.2.1/setup.py` & `triplify_csv-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,185 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: triplify-csv
+Version: 0.2.2
+Summary: A tool to generate triples from CSV files according to a configuration file.
+Home-page: https://github.com/AAtley/triplify_csv
+License: BSD-3-Clause
+Author: Adrian Atley
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Project-URL: Repository, https://github.com/AAtley/triplify_csv
+Description-Content-Type: text/markdown
+
+triplify\_csv
+=============
+
+Features
+========
+
+Generates RDF triples or quads in Turtle or NQuad syntax from one or more CSV files and a configuration file.
+
+Installation
+============
+
+triplify\_csv can be installed from PyPI using 'pip':
+
+```
+pip install triplify_csv
+```
+
+Usage
+=====
+
+triplify\_csv installs as both a package and command line interface tool
+
+**Example of using the package**
+
+	from TriplifyCsv import Rml, CsvOptions
+	
+	# config mapping files are .ttl files
+	configfile = 'myconfig.ttl'
+	
+	# csv files should be .csv files
+	csvfile1, csvfile2 = 'mycsv1.csv', 'mycsv2.csv'
+	
+	# output file must have either a .ttl extension for turtle triples
+	# or a .nq extension for quads
+	outputfile = 'mytriples.ttl'
+	
+	rml = Rml()
+	
+	# default date format of dates in your CSV files is '%Y-%m-%d'
+	# default csv delimiter is ','
+	# override the defaults by setting options
+	options = CsvOptions(dateformat='%d/%m/%Y', delimiter='|')
+	
+	# load one rml and one or more csvs
+	rml.loadFile(configfile, [csvfile1,csvfile2], options)
+	 
+	rml.create_triples()
+	
+	# "nquads" for named graphs need a .nq extension
+	# here we are generating triples so .ttl for turtle syntax
+	rml.write_file(outputfile, format="ttl")
+
+
+
+**Example of CLI use - help text**
+
+To display full help text on the options enter the following at the command line
+
+```
+triplify_csv --help
+```
+
+
+**Example of CLI use - making triples** The same example as the one in code above as a CLI call instead ...
+
+```
+triplify_csv -m 'myconfig.ttl' -c 'mycsv1.csv' -c 'mycsv2.csv' -o 'mytriples.ttl'
+```
+
+**How to make your configuration file**
+
+The configuration file contains a set of mappings for triplify\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.
+
+R2RML was not designed for this purpose. R2RML is '.. a language for expressing customized mappings from relational databases to RDF datasets.' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using 'rr:logicalTable' this should be understood in the triplify\_csv use of R2RML as referring to the name (without '.csv') of a corresponding csv file. 'rr:sqlQuery', the term of the R2RML language that lets you express mappings from database queries to RDF isn't supported in the triplify\_csv usage. Also, there is no need to support 'rr:sqlVersion'.
+
+For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.2.0 the test cases supported are
+
+- R2RMLTC0007a - Typing resources by relying on rdf:type predicate
+- R2RMLTC0007b - Assigning triples to Named Graphs
+- R2RMLTC0007c - One column mapping, using rr:class
+- R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type
+- R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class
+- R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
+- R2RMLTC0007g - Assigning triples to the default graph
+- R2RMLTC0007h - Assigning triples to a non-IRI named graph
+- R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template
+- R2RMLTC0008b - Generation of triples referencing object map
+- R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap
+- R2RMLTC0009a - Generation of triples from foreign key relations
+- R2RMLTC0015a - Generation of language tags for plain literals from a CSV 'table' with language information
+	- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses 'rr:sqlQuery' to select tags in each language from a single table.
+
+Copyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from 'R2RML: RDB to RDF Mapping Language' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and 'R2RML and Direct Mapping Test Cases' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)
+
+**Simple config file example** Suppose you have a CSV file containing details of contacts (example CSV below) and you want to generate RDF data from this using FOAF, the R2RML config file might look like this ...
+
+	@prefix rr: <http://www.w3.org/ns/r2rml#> .
+	@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+	@prefix ex: <http://example.com/> .
+	@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+	@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+	@base <http://example.com/base/> .
+	
+	<TriplesMap1> a rr:TriplesMap;
+	rr:logicalTable [ rr:tableName "\"Contacts\"" ];
+	
+	rr:subjectMap [ rr:template "http://example.com/Contact/{\"ID\"}/{\"Name\"}";
+	 rr:class foaf:Person;
+	];
+	
+	rr:predicateObjectMap [ rr:predicate ex:id ;
+	 rr:objectMap [ rr:column "\"ID\"" ;  ] ;
+	];
+	
+	rr:predicateObjectMap [ rr:predicate foaf:name ;
+	 rr:objectMap [ rr:column "\"Name\"" ; ] ;
+	];
+	
+	rr:predicateObjectMap [ rr:predicate foaf:interest ;
+	  rr:objectMap [ rr:column "\"Interest\"" ; ] ;
+	];
+	
+	.
+
+
+
+Create a CSV file called 'Contacts.csv' using commas as delimiters between the following values (shown here in a table) ...
+
+ID  | Name | Interest
+:---- | :---- | :--------
+10 | John Smith | https://en.m.wikipedia.org/wiki/Tennis
+20 | Joe Bloggs | https://en.m.wikipedia.org/wiki/Golf
+30 | Mr Bun | https://en.m.wikipedia.org/wiki/Spam_(food) 
+
+
+Now, with triplify_csv installed save the R2RML config file as 'contactsmap.ttl' and the csv file as 'Contacts.csv' and generate the output containing your triples to a file called 'contactstriples.ttl' (for example) with the following command ...
+
+```
+triplify_csv -m 'contactsmap.ttl' -c 'Contacts.csv' -o 'contactstriples.ttl'
+```
+
+The resulting triples in turtle syntax in the 'contactstriples.ttl' file would look like this ...
+
+
+	@prefix ex: <http://example.com/> .
+	@prefix foaf: <http://xmlns.com/foaf/0.1/> .
+	@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
+	
+	<http://example.com/Contact/10/John%20Smith> a foaf:Person ;
+	    ex:id 10 ;
+	    foaf:interest "https://en.m.wikipedia.org/wiki/Tennis" ;
+	    foaf:name "John Smith" .
+	
+	<http://example.com/Contact/20/Joe%20Bloggs> a foaf:Person ;
+	    ex:id 20 ;
+	    foaf:interest "https://en.m.wikipedia.org/wiki/Golf" ;
+	    foaf:name "Joe Bloggs" .
+	
+	<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;
+	    ex:id 30 ;
+	    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\_(food)" ;
+	    foaf:name "Mr Bun" .
 
-packages = \
-['triplify_csv']
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['click>=8.0.3,<9.0.0', 'pytest>=6.2.5,<7.0.0', 'rdflib>=6.0.2,<7.0.0']
-
-entry_points = \
-{'console_scripts': ['triplify_csv = triplify_csv.triplify_csv:process']}
-
-setup_kwargs = {
-    'name': 'triplify-csv',
-    'version': '0.2.1',
-    'description': 'A tool to generate triples from CSV files according to a configuration file.',
-    'long_description': 'triplify\\_csv\n=============\n\nFeatures\n========\n\nGenerates RDF triples or quads in Turtle or NQuad syntax from one or more CSV files and a configuration file.\n\nInstallation\n============\n\ntriplify\\_csv can be installed from PyPI using \'pip\':\n\n```\npip install triplify_csv\n```\n\nUsage\n=====\n\ntriplify\\_csv installs as both a package and command line interface tool\n\n**Example of using the package**\n\n\tfrom TriplifyCsv import Rml, CsvOptions\n\t\n\t# config mapping files are .ttl files\n\tconfigfile = \'myconfig.ttl\'\n\t\n\t# csv files should be .csv files\n\tcsvfile1, csvfile2 = \'mycsv1.csv\', \'mycsv2.csv\'\n\t\n\t# output file must have either a .ttl extension for turtle triples\n\t# or a .nq extension for quads\n\toutputfile = \'mytriples.ttl\'\n\t\n\trml = Rml()\n\t\n\t# default date format of dates in your CSV files is \'%Y-%m-%d\'\n\t# default csv delimiter is \',\'\n\t# override the defaults by setting options\n\toptions = CsvOptions(dateformat=\'%d/%m/%Y\', delimiter=\'|\')\n\t\n\t# load one rml and one or more csvs\n\trml.loadFile(configfile, [csvfile1,csvfile2], options)\n\t \n\trml.create_triples()\n\t\n\t# "nquads" for named graphs need a .nq extension\n\t# here we are generating triples so .ttl for turtle syntax\n\trml.write_file(outputfile, format="ttl")\n\n\n\n**Example of CLI use - help text**\n\nTo display full help text on the options enter the following at the command line\n\n```\ntriplify_csv --help\n```\n\n\n**Example of CLI use - making triples** The same example as the one in code above as a CLI call instead ...\n\n```\ntriplify_csv -m \'myconfig.ttl\' -c \'mycsv1.csv\' -c \'mycsv2.csv\' -o \'mytriples.ttl\'\n```\n\n**How to make your configuration file**\n\nThe configuration file contains a set of mappings for triplify\\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.\n\nR2RML was not designed for this purpose. R2RML is \'.. a language for expressing customized mappings from relational databases to RDF datasets.\' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using \'rr:logicalTable\' this should be understood in the triplify\\_csv use of R2RML as referring to the name (without \'.csv\') of a corresponding csv file. \'rr:sqlQuery\', the term of the R2RML language that lets you express mappings from database queries to RDF isn\'t supported in the triplify\\_csv usage. Also, there is no need to support \'rr:sqlVersion\'.\n\nFor a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.2.0 the test cases supported are\n\n- R2RMLTC0007a - Typing resources by relying on rdf:type predicate\n- R2RMLTC0007b - Assigning triples to Named Graphs\n- R2RMLTC0007c - One column mapping, using rr:class\n- R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type\n- R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class\n- R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type\n- R2RMLTC0007g - Assigning triples to the default graph\n- R2RMLTC0007h - Assigning triples to a non-IRI named graph\n- R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template\n- R2RMLTC0008b - Generation of triples referencing object map\n- R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap\n- R2RMLTC0009a - Generation of triples from foreign key relations\n- R2RMLTC0015a - Generation of language tags for plain literals from a CSV \'table\' with language information\n\t- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses \'rr:sqlQuery\' to select tags in each language from a single table.\n\nCopyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from \'R2RML: RDB to RDF Mapping Language\' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and \'R2RML and Direct Mapping Test Cases\' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)\n\n**Simple config file example** Suppose you have a CSV file containing details of contacts (example CSV below) and you want to generate RDF data from this using FOAF, the R2RML config file might look like this ...\n\n\t@prefix rr: <http://www.w3.org/ns/r2rml#> .\n\t@prefix foaf: <http://xmlns.com/foaf/0.1/> .\n\t@prefix ex: <http://example.com/> .\n\t@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n\t@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n\t@base <http://example.com/base/> .\n\t\n\t<TriplesMap1> a rr:TriplesMap;\n\trr:logicalTable [ rr:tableName "\\"Contacts\\"" ];\n\t\n\trr:subjectMap [ rr:template "http://example.com/Contact/{\\"ID\\"}/{\\"Name\\"}";\n\t rr:class foaf:Person;\n\t];\n\t\n\trr:predicateObjectMap [ rr:predicate ex:id ;\n\t rr:objectMap [ rr:column "\\"ID\\"" ;  ] ;\n\t];\n\t\n\trr:predicateObjectMap [ rr:predicate foaf:name ;\n\t rr:objectMap [ rr:column "\\"Name\\"" ; ] ;\n\t];\n\t\n\trr:predicateObjectMap [ rr:predicate foaf:interest ;\n\t  rr:objectMap [ rr:column "\\"Interest\\"" ; ] ;\n\t];\n\t\n\t.\n\n\n\nCreate a CSV file called \'Contacts.csv\' using commas as delimiters between the following values (shown here in a table) ...\n\nID  | Name | Interest\n:---- | :---- | :--------\n10 | John Smith | https://en.m.wikipedia.org/wiki/Tennis\n20 | Joe Bloggs | https://en.m.wikipedia.org/wiki/Golf\n30 | Mr Bun | https://en.m.wikipedia.org/wiki/Spam_(food) \n\n\nNow, with triplify_csv installed save the R2RML config file as \'contactsmap.ttl\' and the csv file as \'Contacts.csv\' and generate the output containing your triples to a file called \'contactstriples.ttl\' (for example) with the following command ...\n\n```\ntriplify_csv -m \'contactsmap.ttl\' -c \'Contacts.csv\' -o \'contactstriples.ttl\'\n```\n\nThe resulting triples in turtle syntax in the \'contactstriples.ttl\' file would look like this ...\n\n\n\t@prefix ex: <http://example.com/> .\n\t@prefix foaf: <http://xmlns.com/foaf/0.1/> .\n\t@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n\t\n\t<http://example.com/Contact/10/John%20Smith> a foaf:Person ;\n\t    ex:id 10 ;\n\t    foaf:interest "https://en.m.wikipedia.org/wiki/Tennis" ;\n\t    foaf:name "John Smith" .\n\t\n\t<http://example.com/Contact/20/Joe%20Bloggs> a foaf:Person ;\n\t    ex:id 20 ;\n\t    foaf:interest "https://en.m.wikipedia.org/wiki/Golf" ;\n\t    foaf:name "Joe Bloggs" .\n\t\n\t<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;\n\t    ex:id 30 ;\n\t    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\\_(food)" ;\n\t    foaf:name "Mr Bun" .\n\n\n',
-    'author': 'Adrian Atley',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/AAtley/triplify_csv',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

