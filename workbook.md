# A workbook for how I developed this tool
Nov. 8th, 2023
---

I will unmount the drive from Sphagnum. Here are some command lines I might use:
```bash
sudo mkdir /media/sphagnum_Nov8th2023
umounts /media/johnsonseq
sudo mount /dev/sdf1 /media/johnsonseq/
sudo mount -o rw,auto,user,fmask=0022,dmask=0000,uid=1001,gid=1001 /dev/sdc1 /media/johnsonseq/

```