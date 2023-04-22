# Comparing `tmp/clibrary-1.7.2.tar.gz` & `tmp/clibrary-1.8.1.tar.gz`

## Comparing `clibrary-1.7.2.tar` & `clibrary-1.8.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.7.2/Makefile
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 clibrary-1.7.2/docs.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 clibrary-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 clibrary-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.7.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/__init__.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/__main__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/files.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/inputs.py
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/interface.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/outputs.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.7.2/src/CLIbrary/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.7.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.7.2/LICENSE
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 clibrary-1.7.2/README.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 clibrary-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 clibrary-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.8.1/Makefile
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 clibrary-1.8.1/docs/docs.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/__init__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/__main__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/files.py
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/inputs.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/interface.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/outputs.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.8.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.8.1/LICENSE
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 clibrary-1.8.1/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 clibrary-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 clibrary-1.8.1/PKG-INFO
```

### Comparing `clibrary-1.7.2/docs.md` & `clibrary-1.8.1/docs/docs.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 1. [Introduction](#introduction)
 	1. [CLIbrary](#clibrary)
 	2. [Handlers](#handlers)
 	3. [Settings](#settings)
 	4. [Import CLIbrary](#import-clibrary)
 2. [Interface](#interface)
 	1. [CLI](#cli)
-	2. [Help](#help)
-	3. [Help entries](#help-entries)
+	2. [Option parser](#option-parser)
+	3. [Help](#help)
+	4. [Help entries](#help-entries)
 3. [Files](#files)
 	1. [Loading](#loading)
 	2. [Dumping](#dumping)
 4. [Inputs](#inputs)
 	1. [Strings](#strings)
 	2. [Numbers](#numbers)
 	3. [Booleans](#booleans)
@@ -57,17 +58,18 @@
 Note that, although every function has a default handler, it is recommended to provide at least some options to achieve a better user experience.
 
 ### Settings
 
 As of version 1.2.1, CLIbrary has some "global options" to allow even more personalization.  
 Available options are:
 
-1. `CLIbrary.style.setting_darkMode`, bool: Enables global dark mode.
-2. `CLIbrary.style.setting_plainMode`, bool: Disables styling.
-3. `CLIbrary.data.setting_fileExtension`, str: Defines a file extension for *CLIbrary.aDump* and *CLIbrary.aLoad*. Default value based on Python's module *pickle*.
+1. `CLIbrary.style.setting_darkMode`, bool: Enables global dark mode. Dafault: `False`.
+2. `CLIbrary.style.setting_plainMode`, bool: Disables styling. Default: `False`.
+3. `CLIbrary.input.setting_caseSensitive`, bool: Enables case-sensitiveness. Default: `False`.
+4. `CLIbrary.data.setting_fileExtension`, str: Defines a file extension for *CLIbrary.aDump* and *CLIbrary.aLoad*. Default: `".pickle"`
 
 ### Import CLIbrary
 
 **CLIbrary** can be installed by:
 
 	python3 -m pip install --upgrade CLIbrary
 
@@ -118,62 +120,75 @@
 
 with no more than a single word for the command itself.
 
 [^1]: Colorama styling works best for styling inside **CLIbrary**.
 
 [^2]: The options get returned without the dashes.
 
+### Option parser
+
+``` python
+CLIbrary.optionParser(instructions: list) -> None
+```
+
+*optionParser* is a function that receives a list of strings and returns the single dash options sdOpts, a dictionary, and the double dash options, a list.
+
 ### Help
 
 ``` python
 CLIbrary.helpPrint(handler={}) -> None
 ```
 
 *helpPrint* is a function that reads and print the help JSON whose path gets passed to *cmdIn*.
-This function cannot be called manually as its calls are embedded inside *cmdIn*.
+There's no need to call this function manually as its calls are embedded inside *cmdIn*.
 
 ### Help entries
 
 A help entry must be formatted this way:
 
-	"command": {
-		"description": "Command description.",
-		"options": {"-sdOpt#": "VALUE_DESCRIPTION", "-sdOpt": "VALUE_DESCRIPTION", "--ddOpt": ""}
-	}
+``` json
+"command": {
+	"description": "Command description.",
+	"options": {"-sdOpt#": "VALUE_DESCRIPTION", "-sdOpt": "VALUE_DESCRIPTION", "--ddOpt": ""}
+}
+```
 
 where mandatory options get identified by a "#" and double-dash options don't require a value description.
 
 This is an example from **openBriefcase**'s accounts help JSON[^3]:
 
-	{
-		"exit": {
-			"description": "Exits the account environment."
-		},
-		"new": {
-			"description": "Creates a new movement."
-		},
-		"edit": {
-			"description": "Edits a movement's features specifying at least an attribute.",
-			"options": {"-q#": "MOVEMENT_QUERY", "--reason": "", "--amount": "", "--date": "", "--category": ""}
-		},
-		"remove": {
-			"description": "Removes a movement.",
-			"options": {"-c#": "MOVEMENT_QUERY"}
-		},
-		"summary": {
-			"description": "Prints a summary of the account's movements."
-		},
-		"load": {
-			"description": "Loads a set of movements from a file."
-		},
-		"dump": {
-			"description": "Dumps a set of movements to a file.",
-			"options": {"-s": "STARTING_TIME", "-e": "ENDING_TIME"}
-		}
+``` json
+{
+	"exit": {
+		"description": "Exits the account environment."
+	},
+	"new": {
+		"description": "Creates a new movement."
+	},
+	"edit": {
+		"description": "Edits a movement's features specifying at least an attribute.",
+		"options": {"-q#": "MOVEMENT_QUERY", "--reason": "", "--amount": "", "--date": "", "--category": ""}
+	},
+	"remove": {
+		"description": "Removes a movement.",
+		"options": {"-c#": "MOVEMENT_QUERY"}
+	},
+	"summary": {
+		"description": "Prints a summary of the account's movements."
+	},
+	"load": {
+		"description": "Loads a set of movements from a file."
+	},
+	"dump": {
+		"description": "Dumps a set of movements to a file.",
+		"options": {"-s": "STARTING_TIME", "-e": "ENDING_TIME"}
 	}
+}
+
+```
 
 [^3]: This example refers to the version 1.5.0 of openBriefcase. The updated file can be found on [GitHub](https://github.com/diantonioandrea/openBriefcase/blob/main/resources/openBriefcaseAccountHelp.json).
 
 ## Files
 
 [Go back to ToC](#table-of-contents)
```

#### html2text {}

```diff
@@ -5,41 +5,43 @@
 diantonioandrea). * [**openTree**](https://github.com/diantonioandrea/
 openTree), by [Andrea Di Antonio](https://github.com/diantonioandrea). *
 [**NBody**](https://github.com/diantonioandrea/NBody), by [Andrea Di Antonio]
 (https://github.com/diantonioandrea). Let_me_knowshould_you_want_your_project
 listed_here._##_Table_of_Contents_0._[Projects_built_with_CLIbrary](#projects-
 built-with-clibrary)_1._[Introduction](#introduction)_1._[CLIbrary](#clibrary)
 2._[Handlers](#handlers)_3._[Settings](#settings)_4._[Import_CLIbrary](#import-
-clibrary)_2._[Interface](#interface)_1._[CLI](#cli)_2._[Help](#help)_3._[Help
-entries](#help-entries)_3._[Files](#files)_1._[Loading](#loading)_2._[Dumping]
-(#dumping)_4._[Inputs](#inputs)_1._[Strings](#strings)_2._[Numbers](#numbers)
-3._[Booleans](#booleans)_4._[Dates](#dates)_5._[List_handling](#list-handling)
-5._[Outputs](#outputs)_1._[Output_function](#output-function)_##_Introduction
-###_CLIbrary_**CLIbrary**_is_*a_comprehensive_Python_library_of_standard_CLI
-utilities_for_convenient_command,_I/O,_and_file_handling*._This_means_it_is_a
-set_of_functions_that_simplifies_writing_programs_based_on_it_by_providing_a
-coherent_environment._**CLIbrary**_provides_functions_to:_*_Manage_a_CLI
-interface_through_command-and-options_handling._*_Easily_access_to_the
-program's_*help*._*_Seamlessly_load_and_dump_informations_to_files._*_Handle
-various_type_of_inputs_without_having_to_worry_about_consistency_and_errors._*
-Output_different_type_of_informations_such_as_errors_and_warnings._**CLIbrary**
-is_written_in_Python_and_developed_by_[Andrea_Di_Antonio](https://github.com/
-diantonioandrea)._###_Handlers_Handlers_play_an_important_role_inside
-**CLIbrary**._Every_function_accepts_only_a_handler_which_is_a_dictionary
-structured_as_{"option":_value}._Note_that,_although_every_function_has_a
-default_handler,_it_is_recommended_to_provide_at_least_some_options_to_achieve
-a_better_user_experience._###_Settings_As_of_version_1.2.1,_CLIbrary_has_some
-"global_options"_to_allow_even_more_personalization._Available_options_are:_1.
-`CLIbrary.style.setting_darkMode`,_bool:_Enables_global_dark_mode._2.
-`CLIbrary.style.setting_plainMode`,_bool:_Disables_styling._3.
-`CLIbrary.data.setting_fileExtension`,_str:_Defines_a_file_extension_for
-*CLIbrary.aDump*_and_*CLIbrary.aLoad*._Default_value_based_on_Python's_module
-*pickle*._###_Import_CLIbrary_**CLIbrary**_can_be_installed_by:_python3_-m_pip
-install_--upgrade_CLIbrary_verified_by:_python3_-m_CLIbrary_imported_by:_```
-python_import_CLIbrary_```_and_all_the_functions_can_be_accessed_by:_```_python
+clibrary)_2._[Interface](#interface)_1._[CLI](#cli)_2._[Option_parser](#option-
+parser)_3._[Help](#help)_4._[Help_entries](#help-entries)_3._[Files](#files)_1.
+[Loading](#loading)_2._[Dumping](#dumping)_4._[Inputs](#inputs)_1._[Strings]
+(#strings)_2._[Numbers](#numbers)_3._[Booleans](#booleans)_4._[Dates](#dates)
+5._[List_handling](#list-handling)_5._[Outputs](#outputs)_1._[Output_function]
+(#output-function)_##_Introduction_###_CLIbrary_**CLIbrary**_is_*a
+comprehensive_Python_library_of_standard_CLI_utilities_for_convenient_command,
+I/O,_and_file_handling*._This_means_it_is_a_set_of_functions_that_simplifies
+writing_programs_based_on_it_by_providing_a_coherent_environment._**CLIbrary**
+provides_functions_to:_*_Manage_a_CLI_interface_through_command-and-options
+handling._*_Easily_access_to_the_program's_*help*._*_Seamlessly_load_and_dump
+informations_to_files._*_Handle_various_type_of_inputs_without_having_to_worry
+about_consistency_and_errors._*_Output_different_type_of_informations_such_as
+errors_and_warnings._**CLIbrary**_is_written_in_Python_and_developed_by_[Andrea
+Di_Antonio](https://github.com/diantonioandrea)._###_Handlers_Handlers_play_an
+important_role_inside_**CLIbrary**._Every_function_accepts_only_a_handler_which
+is_a_dictionary_structured_as_{"option":_value}._Note_that,_although_every
+function_has_a_default_handler,_it_is_recommended_to_provide_at_least_some
+options_to_achieve_a_better_user_experience._###_Settings_As_of_version_1.2.1,
+CLIbrary_has_some_"global_options"_to_allow_even_more_personalization.
+Available_options_are:_1._`CLIbrary.style.setting_darkMode`,_bool:_Enables
+global_dark_mode._Dafault:_`False`._2._`CLIbrary.style.setting_plainMode`,
+bool:_Disables_styling._Default:_`False`._3.
+`CLIbrary.input.setting_caseSensitive`,_bool:_Enables_case-sensitiveness.
+Default:_`False`._4._`CLIbrary.data.setting_fileExtension`,_str:_Defines_a_file
+extension_for_*CLIbrary.aDump*_and_*CLIbrary.aLoad*._Default:_`".pickle"`_###
+Import_CLIbrary_**CLIbrary**_can_be_installed_by:_python3_-m_pip_install_--
+upgrade_CLIbrary_verified_by:_python3_-m_CLIbrary_imported_by:_```_python
+import_CLIbrary_```_and_all_the_functions_can_be_accessed_by:_```_python
 CLIbrary.FUNCTION_NAME()_```_##_Interface_[Go_back_to_ToC](#table-of-contents)
 ###_CLI_```_python_CLIbrary.cmdIn(commandHandler={})_->_dict_```_*cmdIn*_stands
 for_*Command_Input*_as_this_function_allows_the_user_to_input_command_as_in_a
 CLI_interface._The_handler_for_this_function_makes_use_of_the_following
 parameters:_*_request,_str:_The_prompt_to_the_user._*_added,_str:_A_set_of
 characters_to_be_automatically_added_to_the_prompt._Default_is_":_"._*_style,
 str[^1]:_A_particular_colour_style_to_be_applied_to_the_prompt._*_verbose,
@@ -47,40 +49,44 @@
 interface._*_helpPath,_str:_The_path_to_the_help_JSON._This_enables_the_*help*
 command._This_function_returns_a_dictionary_with_the_following_keys:_*_command,
 str:_The_command._*_sdOpts,_dict:_A_dictionary_containing_single-dash_options
 as_{"opts1":_"value1",_"opts2":_"value2",_...}[^2]._*_ddOpts,_list:_A_list
 containing_double-dash_options_as_[opts1,_opts2,_...][^2]._Commands_are_always
 structured_as:_command_-sdOpt_value_--ddOpt_with_no_more_than_a_single_word_for
 the_command_itself._[^1]:_Colorama_styling_works_best_for_styling_inside
-**CLIbrary**._[^2]:_The_options_get_returned_without_the_dashes._###_Help_```
-python_CLIbrary.helpPrint(handler={})_->_None_```_*helpPrint*_is_a_function
-that_reads_and_print_the_help_JSON_whose_path_gets_passed_to_*cmdIn*._This
-function_cannot_be_called_manually_as_its_calls_are_embedded_inside_*cmdIn*.
-###_Help_entries_A_help_entry_must_be_formatted_this_way:_"command":_
-{_"description":_"Command_description.",_"options":_{"-sdOpt#":
-"VALUE_DESCRIPTION",_"-sdOpt":_"VALUE_DESCRIPTION",_"--ddOpt":_""}_}_where
+**CLIbrary**._[^2]:_The_options_get_returned_without_the_dashes._###_Option
+parser_```_python_CLIbrary.optionParser(instructions:_list)_->_None_```
+*optionParser*_is_a_function_that_receives_a_list_of_strings_and_returns_the
+single_dash_options_sdOpts,_a_dictionary,_and_the_double_dash_options,_a_list.
+###_Help_```_python_CLIbrary.helpPrint(handler={})_->_None_```_*helpPrint*_is_a
+function_that_reads_and_print_the_help_JSON_whose_path_gets_passed_to_*cmdIn*.
+There's_no_need_to_call_this_function_manually_as_its_calls_are_embedded_inside
+*cmdIn*._###_Help_entries_A_help_entry_must_be_formatted_this_way:_```_json
+"command":_{_"description":_"Command_description.",_"options":_{"-sdOpt#":
+"VALUE_DESCRIPTION",_"-sdOpt":_"VALUE_DESCRIPTION",_"--ddOpt":_""}_}_```_where
 mandatory_options_get_identified_by_a_"#"_and_double-dash_options_don't_require
 a_value_description._This_is_an_example_from_**openBriefcase**'s_accounts_help
-JSON[^3]:_{_"exit":_{_"description":_"Exits_the_account_environment."_},_"new":
-{_"description":_"Creates_a_new_movement."_},_"edit":_{_"description":_"Edits_a
-movement's_features_specifying_at_least_an_attribute.",_"options":_{"-q#":
-"MOVEMENT_QUERY",_"--reason":_"",_"--amount":_"",_"--date":_"",_"--category":
-""}_},_"remove":_{_"description":_"Removes_a_movement.",_"options":_{"-c#":
-"MOVEMENT_QUERY"}_},_"summary":_{_"description":_"Prints_a_summary_of_the
-account's_movements."_},_"load":_{_"description":_"Loads_a_set_of_movements
-from_a_file."_},_"dump":_{_"description":_"Dumps_a_set_of_movements_to_a
-file.",_"options":_{"-s":_"STARTING_TIME",_"-e":_"ENDING_TIME"}_}_}_[^3]:_This
-example_refers_to_the_version_1.5.0_of_openBriefcase._The_updated_file_can_be
-found_on_[GitHub](https://github.com/diantonioandrea/openBriefcase/blob/main/
-resources/openBriefcaseAccountHelp.json)._##_Files_[Go_back_to_ToC](#table-of-
-contents)_**CLIbrary**_provides_two_functions_to_handle_files_loading_and
-dumping:_*aLoad*_and_*aDump*._These_functions_make_a_great_use_of_the_Python
-module_Pickle._###_Loading_```_python_CLIbrary.aLoad(fileHandler:_dict)_```
-*aLoad*_stands_for_*Automatic_Loading*_as_this_function_loads_informations_from
-files_without_user_confirmation._The_handler_for_this_function_makes_use_of_the
+JSON[^3]:_```_json_{_"exit":_{_"description":_"Exits_the_account_environment."
+},_"new":_{_"description":_"Creates_a_new_movement."_},_"edit":_
+{_"description":_"Edits_a_movement's_features_specifying_at_least_an
+attribute.",_"options":_{"-q#":_"MOVEMENT_QUERY",_"--reason":_"",_"--amount":
+"",_"--date":_"",_"--category":_""}_},_"remove":_{_"description":_"Removes_a
+movement.",_"options":_{"-c#":_"MOVEMENT_QUERY"}_},_"summary":_{_"description":
+"Prints_a_summary_of_the_account's_movements."_},_"load":_{_"description":
+"Loads_a_set_of_movements_from_a_file."_},_"dump":_{_"description":_"Dumps_a
+set_of_movements_to_a_file.",_"options":_{"-s":_"STARTING_TIME",_"-e":
+"ENDING_TIME"}_}_}_```_[^3]:_This_example_refers_to_the_version_1.5.0_of
+openBriefcase._The_updated_file_can_be_found_on_[GitHub](https://github.com/
+diantonioandrea/openBriefcase/blob/main/resources/
+openBriefcaseAccountHelp.json)._##_Files_[Go_back_to_ToC](#table-of-contents)
+**CLIbrary**_provides_two_functions_to_handle_files_loading_and_dumping:
+*aLoad*_and_*aDump*._These_functions_make_a_great_use_of_the_Python_module
+Pickle._###_Loading_```_python_CLIbrary.aLoad(fileHandler:_dict)_```_*aLoad*
+stands_for_*Automatic_Loading*_as_this_function_loads_informations_from_files
+without_user_confirmation._The_handler_for_this_function_makes_use_of_the
 following_parameters:_*_path,_str:_The_path_to_the_file._*_ignoreMissing,_bool:
 Whether_to_display_an_error_on_missing_files._###_Dumping_```_python
 CLIbrary.aDump(fileHandler:_dict)_->_None_```_*aDump*_stands_for_*Automatic
 Dumping*_as_this_function_dumps_informations_to_files_without_user
 confirmation._The_handler_for_this_function_makes_use_of_the_following
 parameters:_*_path,_str:_The_path_to_the_file._*_data:_The_data_to_be_dumped.
 ##_Inputs_[Go_back_to_ToC](#table-of-contents)_###_Strings_```_python
```

### Comparing `clibrary-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `clibrary-1.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `clibrary-1.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/.github/workflows/python-publish.yml` & `clibrary-1.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/src/CLIbrary/__main__.py` & `clibrary-1.8.1/src/CLIbrary/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 import pkg_resources
 
 from .outputs import *
 
 output({"type": "verbose", "string": "CLIbrary v" + pkg_resources.get_distribution("CLIbrary").version})
 print("A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.")
 print("Developed by " + Style.BRIGHT + Fore.CYAN + "Andrea Di Antonio" + Style.RESET_ALL + ", more on " + Style.BRIGHT + "https://github.com/diantonioandrea/CLIbrary" + Style.RESET_ALL)
-print("Documentation on " + Style.BRIGHT + "https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md" + Style.RESET_ALL)
+print("Documentation on " + Style.BRIGHT + "https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md" + Style.RESET_ALL)
 print("Bug tracker on " + Style.BRIGHT + "https://github.com/diantonioandrea/CLIbrary/issues" + Style.RESET_ALL)
```

### Comparing `clibrary-1.7.2/src/CLIbrary/files.py` & `clibrary-1.8.1/src/CLIbrary/files.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/src/CLIbrary/inputs.py` & `clibrary-1.8.1/src/CLIbrary/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from colorama import Fore, Back, Style
 from datetime import datetime
 
 from .outputs import *
-from .settings import *
+from .settings import style
 
 # INPUT HANDLING
 
-def strIn(stringHandler={}) -> str: # String input.
+def strIn(stringHandler={}) -> str: # String input.	
 	handler = {}
 
 	# Strings.
 	handler["request"] = "String: " # The input request.
 	handler["added"] = ": " # The set of added characters to the input request.
 
 	# Lists.
@@ -92,15 +92,18 @@
 	lengthString = ""
 	if handler["fixedLength"] > 0:
 		lengthStyle + "[" + str(handler["fixedLength"]) + "]" + Style.RESET_ALL + " "
 
 	# Input.
 	while True:
 		try:
-			answer = str(input(allowedString + lengthString + handler["request"] + handler["added"])).lower() # Non-sensitive.
+			answer = str(input(allowedString + lengthString + handler["request"] + handler["added"]))
+
+			if not style.setting_caseSensitive: # Case-sensitiveness.
+				answer = answer.lower()
 
 			if handler["verbose"]: # Verbosity.
 				output({"type": "verbose", "string": "VERBOSE, INPUT: " + answer})
 
 			if handler["fixedLength"] != 0 and len(answer) != handler["fixedLength"]: # Checks length.
 				output({"type": "error", "string": "LENGTH ERROR"})
 				continue
```

### Comparing `clibrary-1.7.2/src/CLIbrary/interface.py` & `clibrary-1.8.1/src/CLIbrary/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,65 +51,52 @@
 
 	# Plain style.
 	if style.setting_plainMode:
 		handler["style"] = ""
 
 	while True:
 		try:
-			rawAnswer = str(input(handler["style"] + handler["request"] + Style.RESET_ALL + handler["added"] + Style.RESET_ALL)).lower()
+			rawAnswer = str(input(handler["style"] + handler["request"] + Style.RESET_ALL + handler["added"] + Style.RESET_ALL))
+
+			if not style.setting_caseSensitive: # Case-sensitiveness.
+				rawAnswer = rawAnswer.lower()
 			
 			if handler["verbose"]:
 				output({"type": "verbose", "string": "VERBOSE, INPUT: " + rawAnswer})
 
 			instructions = rawAnswer.split(" ")
 
-			# OPTIONS: SINGLE DASH [{(-)key1: value1}, ...] AND DOUBLE DASH [(--)key1, ...]
-
-			sdOpts = {}
-			ddOpts = []
-
 			if "-" not in instructions[0]: # Checks the first word.
 				answer["command"] = instructions[0]
 
 			else:
 				output({"type": "error", "string": "SYNTAX ERROR"})
 				continue
 
 			if answer["command"] not in handler["allowedCommands"] and rawAnswer != "": # Checks the commands list.
 				output({"type": "error", "string": "UNKNOWN OR UNAVAILABLE COMMAND"})
 				continue
 
 			if answer["command"] == "help": # Prints the help.
 				helpPrint(handler)
 				continue
-
-			for inst in instructions: # Parses the options.
-				if "--" in inst:
-					ddOpts.append(inst.replace("--", ""))
-				
-				elif inst[0] == "-":
-					try:
-						if type(float(inst)) == float:
-							pass
-
-					except(ValueError):
-						sdOpts[inst.replace("-", "")] = instructions[instructions.index(inst) + 1]
 		
 		except(IndexError):
 			output({"type": "error", "string": "SYNTAX ERROR"})
 			continue
 
 		except(EOFError, KeyboardInterrupt): # Handles keyboard interruptions.
 			output({"type": "error", "string": "KEYBOARD ERROR"})
 			continue
 			
-		answer["sdOpts"] = sdOpts
-		answer["ddOpts"] = ddOpts
+		answer["sdOpts"], answer["ddOpts"] = optionsParser(instructions)
 		return answer
 
+# UTILITIES
+
 def helpPrint(handler={}) -> None: # Prints the help.
 	from .settings import style
 
 	try:
 		helpFile = open(handler["helpPath"], "r")
 		helpJson = json.load(helpFile)
 		helpFile.close()
@@ -181,8 +168,28 @@
 		
 		print("\n\n".join(helpElements)) if len(helpElements) else output({"type": "warning", "string": "NO HELP FOR CURRENTLY AVAILABLE COMMANDS", "before": "\n"})
 		
 	except(FileNotFoundError):
 		output({"type": "error", "string": "HELP FILE ERROR"})
 	
 	except:
-		output({"type": "error", "string": "HELP ERROR"})
+		output({"type": "error", "string": "HELP ERROR"})
+
+def optionsParser(instructions: list) -> dict: # Parses the options contained in a list of strings.
+	# OPTIONS: SINGLE DASH [{(-)key1: value1}, ...] AND DOUBLE DASH [(--)key1, ...]
+
+	sdOpts = dict()
+	ddOpts = list()
+
+	for inst in instructions:
+		if "--" in inst:
+			ddOpts.append(inst.replace("--", ""))
+		
+		elif inst[0] == "-":
+			try:
+				if type(float(inst)) == float:
+					pass
+
+			except(ValueError):
+				sdOpts[inst.replace("-", "")] = instructions[instructions.index(inst) + 1]
+
+	return sdOpts, ddOpts
```

### Comparing `clibrary-1.7.2/src/CLIbrary/outputs.py` & `clibrary-1.8.1/src/CLIbrary/outputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/LICENSE` & `clibrary-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clibrary-1.7.2/README.md` & `clibrary-1.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CLIbrary
 
 A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.  
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md)
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md) and at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md).
 
 ## Installation
 
 ### Installing CLIbrary
 
 **CLIbrary** can be installed from [PyPI](https://pypi.org) by:
```

### Comparing `clibrary-1.7.2/pyproject.toml` & `clibrary-1.8.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling", "colorama", "datetime", "setuptools"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CLIbrary"
-version = "1.7.2"
+version = "1.8.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/diantonioandrea/CLIbrary"
-"Documentation" = "https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md"
+"Documentation" = "https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md"
 "Bug Tracker" = "https://github.com/diantonioandrea/CLIbrary/issues"
```

### Comparing `clibrary-1.7.2/PKG-INFO` & `clibrary-1.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: CLIbrary
-Version: 1.7.2
+Version: 1.8.1
 Summary: A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.
 Project-URL: Homepage, https://github.com/diantonioandrea/CLIbrary
-Project-URL: Documentation, https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md
+Project-URL: Documentation, https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/CLIbrary/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CLIbrary
 
 A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.  
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md)
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md) and at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md).
 
 ## Installation
 
 ### Installing CLIbrary
 
 **CLIbrary** can be installed from [PyPI](https://pypi.org) by:
```

