Offlickr is a command-line backup tool for Flickr. It allows you to download photos, videos, metadata (title, tags, description, geotags, notes, comments), and photosets.

It is written in Python and uses [Beej's Python Flickr API](http://stuvel.eu/projects/flickrapi).

<pre>
Usage: Offlickr.py -i <flickr Id><br>
Backs up Flickr photos and metadata<br>
Options:<br>
-f <date>	beginning of the date range<br>
(default: since you started using Flickr)<br>
-t <date>	end of the date range<br>
(default: until now)<br>
-d <dir>	directory for saving files (default: ./dst)<br>
-l <level>	levels of directory hashes (default: 0)<br>
-p		back up photos in addition to photo metadata<br>
-n		do not redownload anything which has already been downloaded (only jpg checked)<br>
-o		overwrite photo, even if it already exists<br>
-L		back up human-readable photo locations and permissions to separate files<br>
-s		back up all photosets (time range is ignored)<br>
-w		use wget instead of internal Python HTTP library<br>
-c <threads>	number of threads to run to backup photos (default: 1)<br>
-v		verbose output<br>
-N		dry run<br>
-h		this help message<br>
<br>
Dates are specified in unixtime (seconds since the Epoch (00:00:00 UTC, January 1, 1970)).<br>
</pre>