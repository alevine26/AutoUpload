# AutoUpload
Personal project to automatically handle converting xbox dvr clips to gifs and automatically uploading them to giphy. Written in Python 2.7.

## Requirements
* [ffmpeg](https://ffmpeg.org/) installed on your machine (and added to path for Windows users)
* [watchdog](https://pypi.python.org/pypi/watchdog) == 0.8.3
* [requests](http://docs.python-requests.org/en/master/) == 2.13.0
* [pyperclip](https://pypi.python.org/pypi/pyperclip) == 1.5.27

TEST!

All of these can be installed with **pip** and the given **requirements.txt** with the command:
  
pip install -r requirements.txt

## Usage
This script current can work in two ways. It can either be run through the command line with the following command:

python autoupload.py **PATH_TO_CAPTURE_FOLDER**

Or, by running the GUI which will allow you to select a folder and start/stop the script.

If a path isn't given, the current directory will be used instead.

## Known Issues
One current problem is the speed of the POST request to giphy. It currently takes ~15s to completely upload the gif. This is most likely due
to the size of the gif currently generated by ffmpeg. I will look into reducing file size and see if that could speed it up.
