# rsync

Below is a list of commands for rsync.

## Simple Folder Sync

This example is for a Windows mount point.

```
rsync -rlptDvih --size-only --stats --progress --delete /home/peter/pictures/* /mnt/smb/
```
