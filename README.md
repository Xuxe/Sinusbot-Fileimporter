# SinusBot - File Importer

A CLI Tool to Import audio files via the HTTP API. Written in Python.

## Usage:

- Non SSL -> ./sinusbot_uploader.py 123.124.125.1 8087 admin foobar /myfolder
- SSL -> ./sinusbot_uploader.py 123.124.125.1 8087 admin foobar /myfolder SSL

## Example:

```bash
xuxe@sinus:~$ python ./sinusbot_upload.py 127.0.0.1 8087 admin foobar /home/xuxe/test/
Success Authenticated!
Success uploaded: /home/xuxe/test/The+Echelon+Effect+-+Your+First+Light+My+Eventide.mp3
Success uploaded: /home/xuxe/test/subdir/Glowworm+-+Periphescence.mp3
Success uploaded: /home/xuxe/test/subdir/Death+Grips+-+Come+Up+and+Get+Me.mp3
Completed -> Uploaded 3 files with 0 errors.
```

## SUPPORTED FILE TYPES: 

`extensions=['mp3', 'mp4', 'wav', '3gp']`

I have added at the moment only mp3, mp4, wav and 3gp. If you need others you can add your own or report it and i will add it. 

I tested it only on Python 2.7 Debian & Ubuntu. 

If you encounter an issue open a Report here: [Report a bug](https://github.com/Xuxe/Sinusbot-File-Importer/issues/new) - Please apply the backtrace! :)
