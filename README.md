# MacOS Tricks
A few my own tricks made my life easier in MacOS

## Write data to NTFS disk

To mount NTFS disk in write mode:

```sh
diskutil list
sudo mkdir /Volumes/ntfs
sudo mount -o rw,nobrowse -t ntfs /dev/disk4s1 /Volumes/ntfs
```
## PHP multiple versions

You can install multiple versions of PHP with **brew** and switch between them with:

```sh
brew unlink php@8.1
brew link php@7.4
````

## Screencast with FFMPEG

List available devices

```sh
ffmpeg -f avfoundation -list_devices true -i ""
```

Various screencan modes

```sh
ffmpeg -f avfoundation -i 1:0 -r 30 test.mp4
ffmpeg -capture_cursor 1 -capture_mouse_clicks 1 -f avfoundation -i 1:0 -r 30 test.mp4
ffmpeg -capture_cursor 1 -capture_mouse_clicks 1 -f avfoundation -i 1:0 -r 30 -s 1280x720 test.mp4

```
