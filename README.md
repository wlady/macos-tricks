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
brew link php@7.1
````
