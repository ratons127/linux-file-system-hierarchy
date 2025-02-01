# linux-file-system-hierarchy
linux file system hierarchy and all directorys 
# Linux-system
lunux-system all cmd and user manual

## 1. / (Root Directory)
The top-level directory from which all other directories branch out.
<br>
Contains essential system directories like bin, etc, home, var, etc.
<br>
Mounted as the primary filesystem at boot.
## 2. /boot
Contains files needed for the system to boot, including:
<br>
Linux kernel (vmlinuz or bzImage).
Bootloader files (GRUB or LILO).
<br>
Initial RAM disk (initrd or initramfs).
## 3. /root
Home directory for the root (superuser) account.
<br>
Only accessible by the root user.
## 4. /bin (Binary)
Contains essential user binaries (commands) required for system operation.
<br>
Common commands: ls, cp, mv, rm, cat, echo, mkdir, etc.
## 5. /sbin (System Binaries)
Contains essential system binaries for administrative tasks.
<br>
Common commands: shutdown, mount, fsck, iptables, etc.
<br>
Typically requires root privileges to execute most commands.
## 6. /media
Mount point for removable media (USB drives, CDs, DVDs, etc.).
<br>
When a USB drive or CD is inserted, it is automatically mounted here.
## 7. /mnt
Temporary mount point for manually mounted filesystems.
<br>
Used when manually mounting an external drive, network share, or another partition.
## 8. /dev (Devices)
Contains device files representing hardware components (not actual files).
<br>
Examples:
<br>
/dev/sda – First hard disk.
<br>
/dev/tty – Terminal devices.
<br>
/dev/null – Null device (data sent here is discarded).
## 9. /etc (Configuration Files)
Stores system-wide configuration files.
Examples:
<br>
/etc/passwd – User account details.
<br>
/etc/shadow – Encrypted passwords.
<br>
/etc/hosts – Static hostname resolution.
<br>
/etc/network/interfaces – Network configuration.
## 10. /usr (User Programs)
Contains user binaries, libraries, and shared data.
<br>
Subdirectories:
<br>
/usr/bin – Non-essential user binaries (vim, nano, wget, etc.).
<br>
/usr/sbin – Non-essential system binaries (apache2, cron, etc.).
<br>
/usr/lib – Libraries for installed applications.
<br>
/usr/share – Shared data like icons, documentation, and localization files.
## 11. /var (Variable Data)
Stores variable (frequently changing) files.
<br>
Common subdirectories:
<br>
/var/log – System logs (e.g., syslog, auth.log).
<br>
/var/spool – Queued jobs (e.g., print jobs, mail).
<br>
/var/cache – Cached data from applications.
<br>
/var/lib – Application state information.
## 12. /tmp (Temporary Files)
Stores temporary files created by applications.
<br>
Cleared on reboot.
## 13. /home (User Home Directories)
Contains personal files, settings, and configurations for users.
<br>
Each user gets a directory, e.g., /home/user1, /home/user2.
<br>
## 14. /opt (Optional Software)
Used for installing third-party software packages.
<br>
The system package manager does not manage applications installed here.
## 15. /proc (Process Information)
Virtual filesystem that provides system and process information.
<br>
Example files:
<br>
/proc/cpuinfo – CPU details.
<br>
/proc/meminfo – Memory usage.
## 16. /sys (System Information)
Provides a way to interact with the kernel and hardware.
<br>
Used for dynamic device and kernel parameter management.
<br>
## 17. /lib (System Libraries)
Contains shared libraries required by binaries in /bin and /sbin.
<br>
Example: /lib/modules/ stores kernel modules.
## 18. /srv (Service Data)
Stores data for system services (e.g., web server, FTP).
<br>
Example: /srv/www might contain website data.
## 19. /run (Runtime Data)
Stores volatile runtime data like process IDs (/run/lock for lock files).
<br>
Data is cleared at reboot.
