# Sinusbot - File Importer
A CLI Tool to Import audio files via the HTTP API. Written in Python.

# Usage:

- Non SSL -> ./sinusbot_uploader.py 123.124.125.1 8087 admin foobar /myfolder
- SSL -> ./sinusbot_uploader.py 123.124.125.1 8087 admin foobar /myfolder SSL

# Result:

xuxe@sinus:~$ python ./sinusbot_upload.py 127.0.0.1 8087 admin foobar /home/xuxe/test/ </br>
Success Authenticated! </br>
Success uploaded: /home/xuxe/test/The+Echelon+Effect+-+Your+First+Light+My+Eventide.mp3 </br>
Success uploaded: /home/xuxe/test/subdir/Glowworm+-+Periphescence.mp3 </br>
Success uploaded: /home/xuxe/test/subdir/Death+Grips+-+Come+Up+and+Get+Me.mp3 </br>
Completed -> Uploaded 3 files with 0 errors. </br>

# Specify Folder:
You need the folder UUID to specify a folder.
To get this, when viewing a folder i.e. http://127.0.0.1:8087/play/list/6167f60e-acd0-4e84-b5c0-d2e102d951c3, the 6167f60e-acd0-4e84-b5c0-d2e102d951c3 on the end would be the UUID
Examples:
- **Basic ->** ./sinusbot_uploader.py 127.0.0.1 8087 admin foober /myfolder 6167f60e-acd0-4e84-b5c0-d2e102d951c3
- **Recursive ->** ./sinusbot_uploader.py 127.0.0.1 8087 admin foobar /myfolder 6167f60e-acd0-4e84-b5c0-d2e102d951c3 -R
- **Recurisve + SSL ->** ./sinusbot_uploader.py 127.0.0.1 8087 admin foobar /myfolder 6167f60e-acd0-4e84-b5c0-d2e102d951c3 -R SSL
- **SSL ->** ./sinusbot_uploader.py 127.0.0.1 8087 admin foobar /myfolder 6167f60e-acd0-4e84-b5c0-d2e102d951c3 SSL
- **SSL + Recursive ->** ./sinusbot_uploader.py 127.0.0.1 8087 admin foobar /myfolder 6167f60e-acd0-4e84-b5c0-d2e102d951c3 SSL -R

**You can still use the original way specified in the Usage**



SUPPORTED FILE TYPES: extensions=['mp3', 'mp4', 'wav', '3gp'] - i have added at the moment only mp3, mp4, wav and 3gp. If you need others you can add your own or report it and i will add it! 

I tested it only on Python 2.7 Debian & Ubuntu. 

If you encounter an issue open a Report here: [Report a bug] (https://github.com/Xuxe/Sinusbot-File-Importer/issues/new) - Please apply the backtrace! :)
