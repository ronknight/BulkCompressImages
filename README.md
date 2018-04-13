CompressImages
==============

Python script for automatically reducing size of all JPEG and PNG images in a directory.

Usage: `compressimages.py [-h] [--mode {compress,restorebackup,deletebackup}] path`

Positional arguments:  
  `path`                File or directory name

Optional arguments:  
  `-h, --help`          show this help message and exit  
  `--mode {compress,restorebackup,deletebackup}` Mode to run with (default: compress)  
  * `compress`: Compress the image(s).  
  * `restorebackup`: Restore the backup images (valid for directory path only).  
  * `deletebackup`: Delete the backup images (valid for directory path only).
  
      Example 1: Compress Images on SampleFolder 
      compressimages.py --mode compress SampleFolder


      Example 2: Restore backup images on SampleFolder 
      compressimages.py --mode restorebackup SampleFolder


      Example 3: Compress Images on SampleFolder 
      compressimages.py --mode deletebackup SampleFolder

Issues that may occur:

  ModuleNotFoundError: No module named 'PIL'
  Fix: Please ensure that you installed image using pip


Python 2.7 or later is required.

See [Using Python to Reduce JPEG and PNG Image File Sizes Without Loss of Quality (Softwariness.com)](https://www.softwariness.com/articles/reduce-image-file-sizes-using-python/) for more information.
