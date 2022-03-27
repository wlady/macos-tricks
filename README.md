# macos-tricks
A few my own tricks made my life easier in MacOS

# Write data to NTFS disk

To mount NTFS disk in write mode:

```sh
diskutil list
sudo mkdir /Volumes/ntfs
sudo mount -o rw,nobrowse -t ntfs /dev/disk4s1 /Volumes/ntfs
```
