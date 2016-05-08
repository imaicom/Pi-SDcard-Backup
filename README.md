# Raspberry-Pi-SDcard-Backup for Mac

1. Put a copy the original SD card
2. Start the Terminal application
3. diskutil list
4. Check the device of the SD card ( maybe 3 )
5. diskutil unmountDisk /dev/disk3
6. sudo dd if=/dev/disk3 of=~/Desktop/raspi.dmg bs=1m
7. type "control-T"
8. Confirmation of remaining 
9. 32GB , Calculated as follows: ? byte / 32*10^9
10. end of copy
11. diskutil unmountDisk /dev/disk3
12. Put the copy destination SD card
13. diskutil unmountDisk /dev/disk3
14. sudo newfs_msdos -F 16 /dev/disk3
15. sudo dd if=~/Desktop/raspi.dmg of=/dev/rdisk3 bs=1m
16. type "control-T"
17. 32GB , Calculated as follows: ? byte / 32*10^9
18. end of copy
19. 11. diskutil unmountDisk /dev/disk3
