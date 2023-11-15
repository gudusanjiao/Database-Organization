# A workbook for how I developed this tool
Nov. 8th, 2023
---

I will unmount the drive from Sphagnum. Here are some command lines I might use:
```bash
sudo mkdir /media/sphagnum_Nov8th2023
# check disk usage
du -sh

# unmount
sudo umount /media/johnsonseq

# Mount backup drive
sudo mount /dev/sdc2 /media/sphagnum_Nov8th2023_bak
sudo mount -o rw,auto,user,fmask=0022,dmask=0000,uid=1001,gid=1001 /dev/sdc1 /media/sphagnum_Nov8th2023_bak

  ## Remember to get into a screen session
sudo rsync -a /home /media/sphagnum_Nov8th2023_bak
sudo umount /media/sphagnum_Nov8th2023_bak

# Remount
sudo mount /dev/sdf1 /media/johnsonseq/
sudo mount -o rw,auto,user,fmask=0022,dmask=0000,uid=1001,gid=1001 /dev/sdc1 /media/johnsonseq/
```

On the other side, I will prepare the spreadsheet of the data we have - to link different data names together.

