# Comparing `tmp/ytmusic_deleter-2.1.0.tar.gz` & `tmp/ytmusic_deleter-2.1.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.1.0.tar", last modified: Thu Mar 21 03:30:27 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.1.2a2.tar", last modified: Tue Apr  2 03:06:29 2024, max compression
```

## Comparing `ytmusic_deleter-2.1.0.tar` & `ytmusic_deleter-2.1.2a2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     3576 2024-03-20 06:12:37.035802 ytmusic_deleter-2.1.0/../../README.md
--rw-r--r--   0        0        0        0 2024-03-11 00:07:50.511456 ytmusic_deleter-2.1.0/__init__.py
--rw-r--r--   0        0        0     1198 2024-03-19 04:40:21.078366 ytmusic_deleter-2.1.0/auth.py
--rw-r--r--   0        0        0    15180 2024-03-19 04:40:21.078366 ytmusic_deleter-2.1.0/cli.py
--rw-r--r--   0        0        0      174 2024-03-19 04:40:21.078366 ytmusic_deleter-2.1.0/constants.py
--rw-r--r--   0        0        0      303 2024-03-19 04:40:21.078366 ytmusic_deleter-2.1.0/progress.py
--rw-r--r--   0        0        0      487 2024-03-21 03:30:27.788479 ytmusic_deleter-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     9518 2024-03-19 04:40:21.078366 ytmusic_deleter-2.1.0/uploads.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 ytmusic_deleter-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-03 22:51:33.484508 ytmusic_deleter-2.1.2a2/LICENSE
+-rw-r--r--   0        0        0     5003 2024-04-02 02:38:58.336925 ytmusic_deleter-2.1.2a2/cli/README.md
+-rw-r--r--   0        0        0      168 2024-03-23 01:15:00.755947 ytmusic_deleter-2.1.2a2/cli/constants.py
+-rw-r--r--   0        0        0     1270 2024-04-02 02:50:10.180112 ytmusic_deleter-2.1.2a2/cli/src/auth.py
+-rw-r--r--   0        0        0    15552 2024-04-02 02:50:10.180112 ytmusic_deleter-2.1.2a2/cli/src/cli.py
+-rw-r--r--   0        0        0      319 2024-04-02 01:18:46.035488 ytmusic_deleter-2.1.2a2/cli/src/progress.py
+-rw-r--r--   0        0        0     9424 2024-04-02 02:50:10.180112 ytmusic_deleter-2.1.2a2/cli/src/uploads.py
+-rw-r--r--   0        0        0     4318 2024-04-02 02:51:40.843465 ytmusic_deleter-2.1.2a2/cli/tests/conftest.py
+-rw-r--r--   0        0        0     1872 2024-04-02 03:00:09.911903 ytmusic_deleter-2.1.2a2/cli/tests/test_cli.py
+-rw-r--r--   0        0        0     1153 2024-04-02 03:06:29.921230 ytmusic_deleter-2.1.2a2/pyproject.toml
+-rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 ytmusic_deleter-2.1.2a2/PKG-INFO
```

### Comparing `ytmusic_deleter-2.1.0/auth.py` & `ytmusic_deleter-2.1.2a2/cli/src/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import logging
-from json import JSONDecodeError
-from pathlib import Path
-
-import constants as const
-import ytmusicapi
-from ytmusicapi import YTMusic
-
-
-def ensure_auth(credential_dir) -> YTMusic:
-    """
-    Checks for an existing oauth.json file to authenticate with.
-    If one does not exist, prompt the user on the console to authenticate to
-    generate one.
-
-    See https://ytmusicapi.readthedocs.io/en/stable/setup/oauth.html
-    """
-    oauth_file_path: str = str(Path(credential_dir) / const.OAUTH_FILENAME)
-    yt_auth = None
-    try:
-        logging.info(f"Attempting authentication with: {oauth_file_path}")
-        yt_auth = YTMusic(oauth_file_path)
-        logging.info(f'Authenticated with: {oauth_file_path}"')
-    except JSONDecodeError:
-        logging.info(f"Creating file: {const.OAUTH_FILENAME}")
-        ytmusicapi.setup_oauth(filepath=oauth_file_path, open_browser=True)
-        yt_auth = YTMusic(oauth_file_path)
-        logging.info(f'Created: {oauth_file_path}"')
-    finally:
-        if yt_auth:
-            logging.info(
-                f"Logged in as {yt_auth.get_account_info().get('accountName')!r}"
-            )
-    return yt_auth
+import logging
+from json import JSONDecodeError
+from pathlib import Path
+
+from .. import constants as const
+import ytmusicapi
+from ytmusicapi import YTMusic
+
+
+def ensure_auth(credential_dir) -> YTMusic:
+    """
+    Checks for an existing oauth.json file to authenticate with.
+    If one does not exist, prompt the user on the console to authenticate to
+    generate one.
+
+    See https://ytmusicapi.readthedocs.io/en/stable/setup/oauth.html
+    """
+    oauth_file_path: str = str(Path(credential_dir) / const.OAUTH_FILENAME)
+    yt_auth = None
+    try:
+        logging.info(f"Attempting authentication with: {oauth_file_path}")
+        yt_auth = YTMusic(oauth_file_path)
+        logging.info(f'Authenticated with: {oauth_file_path}"')
+    except JSONDecodeError:
+        logging.info(f"Creating file: {const.OAUTH_FILENAME}")
+        ytmusicapi.setup_oauth(filepath=oauth_file_path, open_browser=True)
+        yt_auth = YTMusic(oauth_file_path)
+        logging.info(f'Created: {oauth_file_path}"')
+    finally:
+        if yt_auth:
+            try:
+                logging.info(f"Logged in as {yt_auth.get_account_info().get('accountName')!r}")
+            except KeyError:
+                logging.error("Unable to get account name of logged-in user")
+    return yt_auth
```

### Comparing `ytmusic_deleter-2.1.0/uploads.py` & `ytmusic_deleter-2.1.2a2/cli/src/uploads.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,206 @@
-import logging
-import re
-from typing import Dict
-from typing import List
-from typing import TypedDict
-
-import constants as const
-from click import Context
-from progress import manager
-from progress import update_progress
-from thefuzz import fuzz
-from thefuzz import process
-from ytmusicapi import YTMusic
-
-
-def maybe_delete_uploaded_albums(ctx: Context, youtube_auth: YTMusic) -> tuple[int, int]:
-    """
-    Retrieve all of the uploaded songs, then filter the list to just songs from unique albums.
-    Iterate over each album-unique song. If `add_to_library` is true, search the YTM online catalog
-    using "<artist> <album_title>" and see if there's an album that matches it. If a match is found,
-    add the album to the library and delete the entire uploaded album that it's from. If a match wasn't
-    found, keep the uploaded album. If `add_to_library` is false, delete the uploaded album that the
-    song is from (or just the song if it wasn't part of an album).
-
-    `Returns`: a tuple of the number of albums deleted, and the total album count
-    """
-    logging.info("Retrieving all uploaded songs...")
-    albums_deleted = 0
-    uploaded_songs = youtube_auth.get_library_upload_songs(limit=None)
-    if not uploaded_songs:
-        return (albums_deleted, 0)
-    logging.info(f"Retrieved {len(uploaded_songs)} uploaded songs from your library.")
-
-    album_unique_songs = list(
-        {v["album"]["id"] if v.get("album") else v["entityId"]: v for v in uploaded_songs}.values()
-    )
-    progress_bar = manager.counter(
-        total=len(album_unique_songs),
-        desc="Albums Processed",
-        unit="albums",
-        enabled=not ctx.obj["STATIC_PROGRESS"],
-    )
-    for song in album_unique_songs:
-        artist = (
-            song["artists"][0]["name"]
-            if song.get("artists")  # Using `get` ensures key exists and isn't []
-            else const.UNKNOWN_ARTIST
-        )
-        album_title = song["album"]["name"] if song.get("album") else const.UNKNOWN_ALBUM
-        logging.info(f"Processing album: {artist} - {album_title}")
-        if ctx.params["add_to_library"]:
-            if artist == const.UNKNOWN_ARTIST or album_title == const.UNKNOWN_ALBUM:
-                if artist == const.UNKNOWN_ARTIST:
-                    logging.warn("\tSong is missing artist metadata.")
-                if album_title == const.UNKNOWN_ALBUM:
-                    logging.warn("\tSong is missing album metadata.")
-                logging.warn("\tSkipping match search and will not delete.")
-                update_progress(ctx, progress_bar)
-                continue
-            elif not add_album_to_library(ctx, youtube_auth, artist, album_title):
-                logging.warn(
-                    f"\tNo album was added to library for '{artist} - {album_title}'. Will not delete from uploads."
-                )
-                update_progress(ctx, progress_bar)
-                continue
-        response = youtube_auth.delete_upload_entity(song["album"]["id"] if song.get("album") else song["entityId"])
-        if response == "STATUS_SUCCEEDED":
-            logging.info("\tDeleted album from uploads.")
-            albums_deleted += 1
-        else:
-            logging.error("\tFailed to delete album from uploads")
-        update_progress(ctx, progress_bar)
-    return (albums_deleted, len(album_unique_songs))
-
-
-def add_album_to_library(ctx: Context, youtube_auth: YTMusic, upload_artist, upload_title) -> bool:
-    """
-    Search for "<artist> <album title>" in the YTM online catalog.
-
-    `Return`: `True` if an album was added to library, `False` otherwise
-    """
-    logging.info(f"\tSearching YT Music for albums like: '{upload_artist} - {upload_title}'")
-    search_results = youtube_auth.search(f"{upload_artist} {upload_title}", filter="albums")
-    if not search_results:
-        logging.info("No search results were found. It's possible Google is limiting your requests. Try again later.")
-        return False
-    logging.info(f"\tThere were {len(search_results)} album results.")
-
-    # collect all search results into a simplified list
-    search_results = simplify_album_results(search_results)
-
-    def artist_is_correct(search_result):
-        return fuzz.partial_ratio(upload_artist, search_result["artist"]) >= const.ARTIST_NAME_SCORE_CUTOFF
-
-    # filter out results where the artist name is not a good match
-    search_results = list(filter(artist_is_correct, search_results))
-    if not search_results:
-        logging.info("\tNone of the search results had the correct artist name.")
-        return False
-
-    if ctx.params["fuzzy"]:
-
-        def scorer(query, choice):
-            return fuzz.partial_ratio(query, choice)
-
-        # Find the best match for the album title among the search results
-        match, score = process.extractOne(
-            upload_title, search_results, processor=lambda x: x["title"] if isinstance(x, dict) else x, scorer=scorer
-        )
-
-        # Make sure this result at least passes the score cutoff
-        if score < ctx.params["score_cutoff"]:
-            logging.info(
-                f"\tThe best search result '{match['artist']} - {match['title']}' had a match score of {score} which does not pass the score cutoff of {ctx.params['score_cutoff']}."  # noqa: B950
-            )
-            return False
-
-        # Add the match to the library
-        logging.info(
-            f"\tFound match: '{match['artist']} - {match['title']}' with a matching score of {score}. Adding to library..."
-        )
-    else:
-        # TODO fix up fuzzy matching algorithms enough to the point where we don't need this anymore
-        match = None
-        for search_result in search_results:
-            search_result_artist = search_result["artist"]
-            search_result_title = search_result["title"]
-            if upload_title in search_result_title:
-                match = search_result
-                logging.info(f"\tFound match: '{match['artist']} - {match['title']}'. Adding to library...")
-                break
-            else:
-                # Try again but strip out parenthetical expressions at the end of the title, and all symbols
-                sanitze_regex = r"\s*\([^)]*\)$|\s*\[[^)]*\]$|[^\w\s]"
-                extra_whitespace_regex = r"\s+"
-                upload_title = re.sub(sanitze_regex, "", upload_title).strip()
-                upload_title = re.sub(extra_whitespace_regex, " ", upload_title)
-                search_result_title = re.sub(sanitze_regex, "", search_result_title).strip()
-                search_result_title = re.sub(extra_whitespace_regex, " ", search_result_title)
-                logging.info(f"\t\tSanitized upload is: {upload_artist} - {upload_title}")
-                logging.info(f"\t\tSanitized match is:  {search_result_artist} - {search_result_title}")
-                if upload_title in search_result_title:
-                    match = search_result
-                    logging.info(f"\tFound match: '{match['artist']} - {match['title']}'. Adding to library...")
-                    break
-            logging.info(f"\t\tThis {'IS' if match else 'is NOT'} a match")
-        if not match:
-            logging.info(f"No matches were found in YTM for `{upload_artist} - {upload_title}`")
-            return False
-
-    catalog_album = youtube_auth.get_album(match["browseId"])
-    success = youtube_auth.rate_playlist(catalog_album["audioPlaylistId"], const.LIKE)
-    if success:
-        logging.info("\tAdded album to library.")
-        return True
-    else:
-        logging.error("\tFailed to add album to library")
-        return False
-
-
-class SearchResult(TypedDict):
-    artist: str
-    title: str
-    browseId: str
-
-
-def simplify_album_results(album_results: List[Dict]) -> List[SearchResult]:
-    """
-    Take the search results response object from YTM and return a simplified list
-    of results that just has the artist, album title, and browseId.
-    Example: [
-        {"artist": "Metallica", "title": "Load", "browseId": "abcdef"},
-        {"artist": "Metallica", "title": "Reload", "browseId": "fedcba"},
-    ]
-    """
-    simplified_results: List[SearchResult] = []
-    missing_metadata_count = 0
-    for album_result in album_results:
-        search_result_artist = album_result.get("artist")
-        if not search_result_artist:
-            if not album_result.get("artists") or not isinstance(album_result.get("artists"), list):
-                missing_metadata_count += 1
-                continue
-            for artist in album_result.get("artists"):
-                if artist.get("name") and artist.get("id"):
-                    search_result_artist = artist.get("name")
-            if not search_result_artist:
-                missing_metadata_count += 1
-                continue
-        if album_result.get("title"):
-            search_result_title = album_result.get("title")
-        if not search_result_title:
-            missing_metadata_count += 1
-            continue
-
-        simplified_results.append(
-            SearchResult(artist=search_result_artist, title=search_result_title, browseId=album_result["browseId"])
-        )
-
-    if missing_metadata_count > 0:
-        logging.info(
-            f"\t{missing_metadata_count} of the results were missing artist or title metadata and were skipped."
-        )
-    return simplified_results
+import logging
+import re
+from typing import Dict
+from typing import List
+from typing import TypedDict
+
+from .. import constants as const
+from click import get_current_context
+from .progress import manager
+from .progress import update_progress
+from thefuzz import fuzz
+from thefuzz import process
+from ytmusicapi import YTMusic
+
+
+def maybe_delete_uploaded_albums() -> tuple[int, int]:
+    """
+    Retrieve all of the uploaded songs, then filter the list to just songs from unique albums.
+    Iterate over each album-unique song. If `add_to_library` is true, search the YTM online catalog
+    using "<artist> <album_title>" and see if there's an album that matches it. If a match is found,
+    add the album to the library and delete the entire uploaded album that it's from. If a match wasn't
+    found, keep the uploaded album. If `add_to_library` is false, delete the uploaded album that the
+    song is from (or just the song if it wasn't part of an album).
+
+    `Returns`: a tuple of the number of albums deleted, and the total album count
+    """
+    logging.info("Retrieving all uploaded songs...")
+    albums_deleted = 0
+    yt_auth: YTMusic = get_current_context().obj["YT_AUTH"]
+    uploaded_songs = yt_auth.get_library_upload_songs(limit=None)
+    if not uploaded_songs:
+        return (albums_deleted, 0)
+    logging.info(f"Retrieved {len(uploaded_songs)} uploaded songs from your library.")
+
+    album_unique_songs = list(
+        {v["album"]["id"] if v.get("album") else v["entityId"]: v for v in uploaded_songs}.values()
+    )
+    progress_bar = manager.counter(
+        total=len(album_unique_songs),
+        desc="Albums Processed",
+        unit="albums",
+        enabled=not get_current_context().obj["STATIC_PROGRESS"],
+    )
+    for song in album_unique_songs:
+        artist = (
+            song["artists"][0]["name"]
+            if song.get("artists")  # Using `get` ensures key exists and isn't []
+            else const.UNKNOWN_ARTIST
+        )
+        album_title = song["album"]["name"] if song.get("album") else const.UNKNOWN_ALBUM
+        logging.info(f"Processing album: {artist} - {album_title}")
+        if get_current_context().params["add_to_library"]:
+            if artist == const.UNKNOWN_ARTIST or album_title == const.UNKNOWN_ALBUM:
+                if artist == const.UNKNOWN_ARTIST:
+                    logging.warn("\tSong is missing artist metadata.")
+                if album_title == const.UNKNOWN_ALBUM:
+                    logging.warn("\tSong is missing album metadata.")
+                logging.warn("\tSkipping match search and will not delete.")
+                update_progress(progress_bar)
+                continue
+            elif not add_album_to_library(yt_auth, artist, album_title):
+                logging.warn(
+                    f"\tNo album was added to library for '{artist} - {album_title}'. Will not delete from uploads."
+                )
+                update_progress(progress_bar)
+                continue
+        response = yt_auth.delete_upload_entity(song["album"]["id"] if song.get("album") else song["entityId"])
+        if response == "STATUS_SUCCEEDED":
+            logging.info("\tDeleted album from uploads.")
+            albums_deleted += 1
+        else:
+            logging.error("\tFailed to delete album from uploads")
+        update_progress(progress_bar)
+    return (albums_deleted, len(album_unique_songs))
+
+
+def add_album_to_library(upload_artist, upload_title) -> bool:
+    """
+    Search for "<artist> <album title>" in the YTM online catalog.
+
+    `Return`: `True` if an album was added to library, `False` otherwise
+    """
+    logging.info(f"\tSearching YT Music for albums like: '{upload_artist} - {upload_title}'")
+    yt_auth: YTMusic = get_current_context().obj["YT_AUTH"]
+    search_results = yt_auth.search(f"{upload_artist} {upload_title}", filter="albums")
+    if not search_results:
+        logging.info("No search results were found. It's possible Google is limiting your requests. Try again later.")
+        return False
+    logging.info(f"\tThere were {len(search_results)} album results.")
+
+    # collect all search results into a simplified list
+    search_results = simplify_album_results(search_results)
+
+    def artist_is_correct(search_result):
+        return fuzz.partial_ratio(upload_artist, search_result["artist"]) >= const.ARTIST_NAME_SCORE_CUTOFF
+
+    # filter out results where the artist name is not a good match
+    search_results = list(filter(artist_is_correct, search_results))
+    if not search_results:
+        logging.info("\tNone of the search results had the correct artist name.")
+        return False
+
+    if get_current_context().params["fuzzy"]:
+
+        def scorer(query, choice):
+            return fuzz.partial_ratio(query, choice)
+
+        # Find the best match for the album title among the search results
+        match, score = process.extractOne(
+            upload_title, search_results, processor=lambda x: x["title"] if isinstance(x, dict) else x, scorer=scorer
+        )
+
+        # Make sure this result at least passes the score cutoff
+        if score < get_current_context().params["score_cutoff"]:
+            logging.info(
+                f"\tThe best search result '{match['artist']} - {match['title']}' had a match score of {score} which does not pass the score cutoff of {get_current_context().params['score_cutoff']}."  # noqa: B950
+            )
+            return False
+
+        # Add the match to the library
+        logging.info(
+            f"\tFound match: '{match['artist']} - {match['title']}' with a matching score of {score}. Adding to library..."
+        )
+    else:
+        # TODO fix up fuzzy matching algorithms enough to the point where we don't need this anymore
+        match = None
+        for search_result in search_results:
+            search_result_artist = search_result["artist"]
+            search_result_title = search_result["title"]
+            if upload_title in search_result_title:
+                match = search_result
+                logging.info(f"\tFound match: '{match['artist']} - {match['title']}'. Adding to library...")
+                break
+            else:
+                # Try again but strip out parenthetical expressions at the end of the title, and all symbols
+                sanitze_regex = r"\s*\([^)]*\)$|\s*\[[^)]*\]$|[^\w\s]"
+                extra_whitespace_regex = r"\s+"
+                upload_title = re.sub(sanitze_regex, "", upload_title).strip()
+                upload_title = re.sub(extra_whitespace_regex, " ", upload_title)
+                search_result_title = re.sub(sanitze_regex, "", search_result_title).strip()
+                search_result_title = re.sub(extra_whitespace_regex, " ", search_result_title)
+                logging.info(f"\t\tSanitized upload is: {upload_artist} - {upload_title}")
+                logging.info(f"\t\tSanitized match is:  {search_result_artist} - {search_result_title}")
+                if upload_title in search_result_title:
+                    match = search_result
+                    logging.info(f"\tFound match: '{match['artist']} - {match['title']}'. Adding to library...")
+                    break
+            logging.info(f"\t\tThis {'IS' if match else 'is NOT'} a match")
+        if not match:
+            logging.info(f"No matches were found in YTM for `{upload_artist} - {upload_title}`")
+            return False
+
+    catalog_album = yt_auth.get_album(match["browseId"])
+    success = yt_auth.rate_playlist(catalog_album["audioPlaylistId"], const.LIKE)
+    if success:
+        logging.info("\tAdded album to library.")
+        return True
+    else:
+        logging.error("\tFailed to add album to library")
+        return False
+
+
+class SearchResult(TypedDict):
+    artist: str
+    title: str
+    browseId: str
+
+
+def simplify_album_results(album_results: List[Dict]) -> List[SearchResult]:
+    """
+    Take the search results response object from YTM and return a simplified list
+    of results that just has the artist, album title, and browseId.
+    Example: [
+        {"artist": "Metallica", "title": "Load", "browseId": "abcdef"},
+        {"artist": "Metallica", "title": "Reload", "browseId": "fedcba"},
+    ]
+    """
+    simplified_results: List[SearchResult] = []
+    missing_metadata_count = 0
+    for album_result in album_results:
+        search_result_artist = album_result.get("artist")
+        if not search_result_artist:
+            if not album_result.get("artists") or not isinstance(album_result.get("artists"), list):
+                missing_metadata_count += 1
+                continue
+            for artist in album_result.get("artists"):
+                if artist.get("name") and artist.get("id"):
+                    search_result_artist = artist.get("name")
+            if not search_result_artist:
+                missing_metadata_count += 1
+                continue
+        if album_result.get("title"):
+            search_result_title = album_result.get("title")
+        if not search_result_title:
+            missing_metadata_count += 1
+            continue
+
+        simplified_results.append(
+            SearchResult(artist=search_result_artist, title=search_result_title, browseId=album_result["browseId"])
+        )
+
+    if missing_metadata_count > 0:
+        logging.info(
+            f"\t{missing_metadata_count} of the results were missing artist or title metadata and were skipped."
+        )
+    return simplified_results
```

