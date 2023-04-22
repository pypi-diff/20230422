# Comparing `tmp/aligo-5.5.8.tar.gz` & `tmp/aligo-5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-5.5.8.tar", last modified: Fri Jan 20 07:33:28 2023, max compression
+gzip compressed data, was "aligo-5.5.9.tar", last modified: Sat Feb  4 06:04:50 2023, max compression
```

## Comparing `aligo-5.5.8.tar` & `aligo-5.5.9.tar`

### file list

```diff
@@ -1,205 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.800696 aligo-5.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-20 07:33:25.000000 aligo-5.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-01-20 07:33:28.804695 aligo-5.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-01-20 07:33:25.000000 aligo-5.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.776696 aligo-5.5.8/aligo/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.780696 aligo-5.5.8/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.784696 aligo-5.5.8/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.784696 aligo-5.5.8/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.792696 aligo-5.5.8/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.796696 aligo-5.5.8/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.800696 aligo-5.5.8/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-20 07:33:25.000000 aligo-5.5.8/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:33:28.800696 aligo-5.5.8/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-20 07:33:28.000000 aligo-5.5.8/aligo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-20 07:33:25.000000 aligo-5.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-20 07:33:28.804695 aligo-5.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-04 06:04:45.000000 aligo-5.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-02-04 06:04:50.836366 aligo-5.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-02-04 06:04:45.000000 aligo-5.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.816366 aligo-5.5.9/aligo/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.828366 aligo-5.5.9/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.832366 aligo-5.5.9/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/DataClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-04 06:04:45.000000 aligo-5.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-04 06:04:50.836366 aligo-5.5.9/setup.cfg
```

### Comparing `aligo-5.5.8/LICENSE` & `aligo-5.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/PKG-INFO` & `aligo-5.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 5.5.8
+Version: 5.5.9
 Summary: aliyundrive apis package
 Home-page: https://github.com/foyoux/aligo
 Author: foyou
 Author-email: yimi.0822@qq.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
```

### Comparing `aligo-5.5.8/README.md` & `aligo-5.5.9/README.md`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Album.py` & `aligo-5.5.9/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Aligo.py` & `aligo-5.5.9/aligo/apis/Aligo.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             level: int = logging.DEBUG,
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
             email: Tuple[str, str] = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
-            login_timeout: float = None
+            login_timeout: float = None,
+            re_login: bool = True
     ):
         """
         Aligo
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
@@ -77,14 +78,15 @@
             关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
                         所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
             关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
                         所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
         :param request_failed_delay: (可选) 由于网络异常导致的 request 异常，等待多少秒后重试
         :param requests_timeout: (可选) 应网友提议，添加 requests timeout 参数
         :param login_timeout: (可选) 登录超时时间，单位：秒。
+        :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
 
         level, use_aria2, proxies, port, email 可以通过 配置文件 配置默认值，在 <用户家目录>/.aligo/config.json5 中
         ```json5
         {
           "level": 10,
           "use_aria2": false,
           "proxies": {
@@ -111,21 +113,24 @@
                 email = config.get('email')
             if request_failed_delay == 3:
                 requests_timeout = config.get('request_failed_delay', 3)
             if requests_timeout is None:
                 requests_timeout = config.get('requests_timeout')
             if requests_timeout is None:
                 login_timeout = config.get('login_timeout')
+            if re_login is True:
+                re_login = config.get('re_login')
 
         super().__init__(
             name,
             refresh_token,
             show,
             level,
             use_aria2,
             proxies,
             port,
             email,
             request_failed_delay,
             requests_timeout,
             login_timeout,
+            re_login,
         )
```

### Comparing `aligo-5.5.8/aligo/apis/Audio.py` & `aligo-5.5.9/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Compress.py` & `aligo-5.5.9/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Copy.py` & `aligo-5.5.9/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Create.py` & `aligo-5.5.9/aligo/apis/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/CustomShare.py` & `aligo-5.5.9/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Download.py` & `aligo-5.5.9/aligo/apis/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Drive.py` & `aligo-5.5.9/aligo/apis/Drive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """drive"""
 
 from aligo.core import *
+from aligo.core.Config import *
 from aligo.request import *
 from aligo.types import *
 
 
 class Drive(Core):
     """..."""
 
@@ -18,7 +19,12 @@
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.get_drive()
         >>> print(result)
         """
         body = GetDriveRequest(drive_id=drive_id)
         return self._core_get_drive(body)
+
+    def drive_capacity_details(self) -> DriveCapacityDetail:
+        """获取网盘容量详细信息"""
+        response = self._post(ADRIVE_V1_USER_DRIVECAPACITY_DETAILS)
+        return self._result(response, DriveCapacityDetail)
```

### Comparing `aligo-5.5.8/aligo/apis/Duplicate.py` & `aligo-5.5.9/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/File.py` & `aligo-5.5.9/aligo/apis/File.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Move.py` & `aligo-5.5.9/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Other.py` & `aligo-5.5.9/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Recyclebin.py` & `aligo-5.5.9/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Search.py` & `aligo-5.5.9/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Share.py` & `aligo-5.5.9/aligo/apis/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Star.py` & `aligo-5.5.9/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/SyncFolder.py` & `aligo-5.5.9/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Update.py` & `aligo-5.5.9/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/apis/Video.py` & `aligo-5.5.9/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Album.py` & `aligo-5.5.9/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Auth.py` & `aligo-5.5.9/aligo/core/Auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import coloredlogs
 import qrcode
 import qrcode_terminal
 import requests
 
 from aligo.core.Config import *
-from aligo.error import AligoStatus500
+from aligo.error import AligoStatus500, AligoRefreshFailed, AligoFatalError
 from aligo.types import *
 from aligo.types.Enum import *
 from .EMail import send_email
 from .LoginServer import LoginServer
 
 aligo_config_folder = Path.home().joinpath('.aligo')
 aligo_config_folder.mkdir(parents=True, exist_ok=True)
@@ -60,15 +60,16 @@
         self.log.warning(f'[method status_code] {r.method} {response.status_code}')
         self.log.warning(f'[url] {response.url}')
         self.log.warning(f'[response body] {response.text[:200]}')
 
     def error_log_exit(self, response: requests.Response):
         """打印错误日志并退出"""
         self.debug_log(response)
-        exit(-1)
+        # exit(-1)
+        raise AligoFatalError(response.text)
 
     @overload
     def __init__(
             self,
             name: str = 'aligo',
             show: Callable[[str], None] = None,
             level=logging.DEBUG,
@@ -102,14 +103,15 @@
             level: int = logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
             email: Tuple[str, str] = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
+            re_login: bool = True,
     ):
         """登录验证
 
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
@@ -117,24 +119,26 @@
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
             关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
                         所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
+        :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
         """
         self._name_name = name
         self._name = aligo_config_folder.joinpath(f'{name}.json')
         self._port = port
         self._webServer: HTTPServer = None  # type: ignore
         self._email = email
         self.log = logging.getLogger(f'{__name__}:{name}')
         self._request_failed_delay = request_failed_delay
         self._requests_timeout = requests_timeout
         self._login_timeout = LoginTimeout(login_timeout)
+        self._re_login = re_login
 
         fmt = f'%(asctime)s.%(msecs)03d {name}.%(levelname)s %(message)s'
 
         coloredlogs.install(
             level=level,
             logger=self.log,
             milliseconds=True,
@@ -291,16 +295,18 @@
             self.log.warning('刷新 token 失败')
             if loop_call:
                 # 从 _login 调用，则不继续调用 _login，防止循环调用
                 # 走到这里 说明 登录失败，则 退出
                 self.error_log_exit(response)
             else:
                 self.debug_log(response)
-                self._login()
-
+                if self._re_login:
+                    self._login()
+                else:
+                    raise AligoRefreshFailed('使用 refresh_token 刷新 token 失败，re_login=False，不继续（等待）登录')
         self.session.headers.update({
             'Authorization': self.token.access_token
         })
 
     _VERIFY_SSL = True
 
     def request(self, method: str, url: str, params: Dict = None,
```

### Comparing `aligo-5.5.8/aligo/core/BaseAligo.py` & `aligo-5.5.9/aligo/core/BaseAligo.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
             email: Tuple[str, str] = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
+            re_login: bool = True
     ):
         """
         BaseAligo
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
@@ -45,26 +46,28 @@
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
             关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
                         所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
+        :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
         """
         self._auth: Auth = Auth(  # type: ignore
             name=name,
             refresh_token=refresh_token,
             show=show,
             level=level,
             proxies=proxies,
             port=port,
             email=email,
             request_failed_delay=request_failed_delay,
             requests_timeout=requests_timeout,
             login_timeout=login_timeout,
+            re_login=re_login,
         )
         # 因为 self._auth.session 没有被重新赋值, 所以可以这么用
         self._session: requests.Session = self._auth.session
         # 在刷新 token 时, self._auth.token 被重新赋值, 而 self._token 却不会被更新
         # self._token: Token = self._auth.token
         self._user: Optional[BaseUser] = None
         self._personal_info: Optional[GetPersonalInfoResponse] = None
```

### Comparing `aligo-5.5.8/aligo/core/Compress.py` & `aligo-5.5.9/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Config.py` & `aligo-5.5.9/aligo/core/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 NEWLOGIN_QRCODE_QUERY_DO = '/newlogin/qrcode/query.do'
 NEWLOGIN_QRCODE_GENERATE_DO = '/newlogin/qrcode/generate.do'
 V2_OAUTH_TOKEN_LOGIN = '/v2/oauth/token_login'
 V2_OAUTH_AUTHORIZE = '/v2/oauth/authorize'
 V2_ACCOUNT_TOKEN = '/v2/account/token'
 TOKEN_REFRESH = '/token/refresh'
 TOKEN_GET = '/token/get'
+USERS_V1_USERS_DEVICE_RENEW_SESSION = '/users/v1/users/device/renew_session'
 
 # 基本信息
 V2_USER_GET = '/v2/user/get'
 ADRIVE_V1_USER_CONFIG_GET = '/adrive/v1/user_config/get'
 V2_DRIVE_GET = '/v2/drive/get'
 V2_DRIVE_GET_DEFAULT_DRIVE = '/v2/drive/get_default_drive'
 V2_DRIVE_LIST_MY_DRIVES = '/v2/drive/list_my_drives'
 V2_DATABOX_GET_PERSONAL_INFO = '/v2/databox/get_personal_info'
 V2_DATABOX_GET_AUDIO_PLAY_INFO = '/v2/databox/get_audio_play_info'
 V2_DATABOX_GET_VIDEO_PLAY_INFO = '/v2/databox/get_video_play_info'
 BUSINESS_V1_USERS_VIP_INFO = '/business/v1.0/users/vip/info'
+ADRIVE_V1_USER_DRIVECAPACITY_DETAILS = '/adrive/v1/user/driveCapacityDetails'
 
 #  文件操作
 V2_FILE_GET = '/v2/file/get'
 V2_FILE_LIST = '/v2/file/list'
 ADRIVE_V3_FILE_LIST = '/adrive/v3/file/list'
 V3_FILE_UPDATE = '/v3/file/update'
 V2_FILE_MOVE = '/v2/file/move'
```

### Comparing `aligo-5.5.8/aligo/core/Copy.py` & `aligo-5.5.9/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Core.py` & `aligo-5.5.9/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Create.py` & `aligo-5.5.9/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Download.py` & `aligo-5.5.9/aligo/core/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Drive.py` & `aligo-5.5.9/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Duplicate.py` & `aligo-5.5.9/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/EMail.py` & `aligo-5.5.9/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/File.py` & `aligo-5.5.9/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/LoginServer.py` & `aligo-5.5.9/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Move.py` & `aligo-5.5.9/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Recyclebin.py` & `aligo-5.5.9/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Search.py` & `aligo-5.5.9/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Share.py` & `aligo-5.5.9/aligo/core/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Star.py` & `aligo-5.5.9/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Update.py` & `aligo-5.5.9/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/User.py` & `aligo-5.5.9/aligo/core/User.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/core/Video.py` & `aligo-5.5.9/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/AlbumListFilesRequest.py` & `aligo-5.5.9/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/CreateFileRequest.py` & `aligo-5.5.9/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/CreateShareLinkRequest.py` & `aligo-5.5.9/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetFileListRequest.py` & `aligo-5.5.9/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetFileRequest.py` & `aligo-5.5.9/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetRecycleBinListRequest.py` & `aligo-5.5.9/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetShareFileListRequest.py` & `aligo-5.5.9/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-5.5.9/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetShareLinkListRequest.py` & `aligo-5.5.9/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/GetStarredListRequest.py` & `aligo-5.5.9/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/SearchFileRequest.py` & `aligo-5.5.9/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/UpdateFileRequest.py` & `aligo-5.5.9/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/UpdateShareLinkRequest.py` & `aligo-5.5.9/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/request/__init__.py` & `aligo-5.5.9/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/CreateFileResponse.py` & `aligo-5.5.9/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/CreateShareLinkResponse.py` & `aligo-5.5.9/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/DuplicateListResponse.py` & `aligo-5.5.9/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/GetShareInfoResponse.py` & `aligo-5.5.9/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/GetShareTokenResponse.py` & `aligo-5.5.9/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/UpdateShareLinkResponse.py` & `aligo-5.5.9/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/response/__init__.py` & `aligo-5.5.9/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/BaseAlbum.py` & `aligo-5.5.9/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/BaseDrive.py` & `aligo-5.5.9/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/BaseFile.py` & `aligo-5.5.9/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/BaseShareFile.py` & `aligo-5.5.9/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/BaseUser.py` & `aligo-5.5.9/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/DataClass.py` & `aligo-5.5.9/aligo/types/DataClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         hints = DataClass._get_hints(cls)
         params = {}
         for key, value in obj.items():
             if key in hints:
                 params[key] = value
             else:
                 if _ALIGO_DEBUG:
-                    _LOGGER.warning(f'{cls.__module__}({key} : {type(value).__name__} = {repr(value)[:100]})')
+                    _LOGGER.warning(
+                        f'{cls.__module__}.{cls.__name__}({key} : {type(value).__name__} = {repr(value)[:100]})')
         return cls(**params)
 
     def __post_init__(self):
         """序列化属性"""
         hints = DataClass._get_hints(self.__class__)
         for k, v in hints.items():
             origin = get_origin(v)
```

### Comparing `aligo-5.5.8/aligo/types/Enum.py` & `aligo-5.5.9/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/ImageMedia.py` & `aligo-5.5.9/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/ShareLinkSchema.py` & `aligo-5.5.9/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/Token.py` & `aligo-5.5.9/aligo/types/Token.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/UserConfig.py` & `aligo-5.5.9/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/VideoMedia.py` & `aligo-5.5.9/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/VideoPreview.py` & `aligo-5.5.9/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.8/aligo/types/VideoPreviewPlayInfo.py` & `aligo-5.5.9/aligo/types/VideoPreviewPlayInfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 # 导包基本原则
 # 1. 包内相对导入: from .DataClass import DataClass
 # 2. 包外包导入: from aligo.dataobj import xxx
 from dataclasses import dataclass, field
 from typing import List
 
-from .Enum import VideoTemplateID
 from .DataClass import DataClass
+from .Enum import VideoTemplateID
 
 
 @dataclass
 class LiveTranscodingMeta(DataClass):
     """..."""
     ts_segment: int = None
     ts_total_count: int = None
@@ -29,14 +29,17 @@
 @dataclass
 class LiveTranscodingTask(DataClass):
     """..."""
     template_id: VideoTemplateID = None
     status: str = None
     stage: str = None
     url: str = None
+    template_name: str = None
+    template_width: int = None
+    template_height: int = None
 
 
 @dataclass
 class VideoPreviewPlayInfo(DataClass):
     """..."""
     category: str = None
     meta: Meta = None
```

### Comparing `aligo-5.5.8/aligo/types/__init__.py` & `aligo-5.5.9/aligo/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .BaseDrive import BaseDrive
 from .BaseFile import BaseFile
 from .BaseShareFile import BaseShareFile
 from .BaseUser import BaseUser
 from .CroppingBoundary import CroppingBoundary
 from .CroppingSuggestionItem import CroppingSuggestionItem
 from .DataClass import DataClass
+from .DriveCapacityDetail import DriveCapacityDetail
 from .FaceThumbnail import FaceThumbnail
 from .ImageMedia import ImageMedia
 from .ImageQuality import ImageQuality
 from .ImageTag import ImageTag
 from .ListAlbumItem import ListAlbumItem
 from .LoginTimout import LoginTimeout
 from .MediaTransCodeTemplate import MediaTransCodeTemplate
```

### Comparing `aligo-5.5.8/aligo.egg-info/PKG-INFO` & `aligo-5.5.9/aligo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 5.5.8
+Version: 5.5.9
 Summary: aliyundrive apis package
 Home-page: https://github.com/foyoux/aligo
 Author: foyou
 Author-email: yimi.0822@qq.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
```

### Comparing `aligo-5.5.8/aligo.egg-info/SOURCES.txt` & `aligo-5.5.9/aligo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 ./aligo/types/BaseDrive.py
 ./aligo/types/BaseFile.py
 ./aligo/types/BaseShareFile.py
 ./aligo/types/BaseUser.py
 ./aligo/types/CroppingBoundary.py
 ./aligo/types/CroppingSuggestionItem.py
 ./aligo/types/DataClass.py
+./aligo/types/DriveCapacityDetail.py
 ./aligo/types/Enum.py
 ./aligo/types/FaceThumbnail.py
 ./aligo/types/FieldsInfo.py
 ./aligo/types/ImageMedia.py
 ./aligo/types/ImageQuality.py
 ./aligo/types/ImageTag.py
 ./aligo/types/ListAlbumItem.py
```

### Comparing `aligo-5.5.8/setup.cfg` & `aligo-5.5.9/setup.cfg`

 * *Files identical despite different names*

