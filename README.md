Find Dialogue
=============

Find Dialogue is a web application that lets you search the transcripts of Big Bang Theory (season 1-5). For more details visit [GitHub page](http://nitishsp.github.com/FindDialogue/) or [the application](http://finddialogue.appspot.com/).


Setup
=======

## Install Dependencies

[Beautiful soup](http://www.crummy.com/software/BeautifulSoup/#Download)


## Fetch Transcripts

    python crawler.py

    python parser.py

Remove 6th season's transcripts from fetched_content directory if crawler.py fails
[Issue](https://github.com/nitishsp/FindDialogue/issues/1)

## Generate csv files

    python transcripts_to_csv.py

    python index_to_csv.py


## Bulkupload

  Use the bulkloader.yaml and csv files to upload data to development or production datastore using [GAE bulkloader](https://developers.google.com/appengine/docs/python/tools/uploadingdata).
You may find command.txt in Index Bulk Loader and Transcipt Bulk Loader helpful. Bulkloading search index takes a while (~20-30min).


## Launch Application

Point App Engine Launcher to the Dialogue Finder directory to run/deploy the application

