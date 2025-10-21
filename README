1. Download firmware.bz and scp to /tmp

2. SSH to openwrt and check current boot partition
   ```fw_printenv -n boot_part```

3. Write stock firmware to the other side partition
   if you got 1 from last step then run
   ```mtd -e kernel2 -r write /tmp/FW_WRT32X_1.0.180404.58.img kernel2```
   otherwise, run
   ```mtd -e kernel1 -r write /tmp/FW_WRT32X_1.0.180404.58.img kernel1```

4. System will reboot after run last step. ssh to openwrt and set the boot partition to burned partition
   ```fw_setenv boot_part <side partition number>```
   ```reboot```

5. Reboot

