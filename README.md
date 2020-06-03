# kvsPMSIE
 Plex Media Server Import Export for watched metadata

This is a small script for KVIrc that will extract the watched movie/show data from the Plex Media Server database file.
You will need to do this if you install PMS onto another or a new machine and you want to retain all your watched metadata.

I don't know why Plex doesn't save watch metadata to the cloud anyway?

You will need KVIrc to use this script: http://kvirc.net/

This script provides a GUI to easily export metadata from your Plex Media Server database file. 
It is useful if or when you need to reinstall your PMS, or you create a new PMS and want to retain 
or restore the metadata of your media. Metadata here means the "watch data" for the media items, 
so that the PMS knows where to resume watching if you stopped an item midway through viewing, 
or if you have watched or not watched a movie or tv episode etc.
		
This utility makes it easier to do the process described at: 
https://support.plex.tv/articles/201154527-move-viewstate-ratings-from-one-install-to-another/
especially for Windows users. It offers a point and click approach.
		
I tried to add some nice progress bars when the utility does the import and export of the data, 
but for some reason the widgets don't update correctly in realtime and I couldn't work out how 
to fix it. If you click the LAUNCH button and it seems to be doing nothing or KVIrc goes into 
"Not Responding" just wait it out and a dialog will tell you when the process is finished.
		
To run this script, in KVIrc press Ctrl + Shift + X, select the classes.kvs file.
Then press Ctrl + Shift + S to open script tester and tpye in: 
			
				%kvsApp = $new(pmsimportexport::main)
		
Then press the Execute button.
