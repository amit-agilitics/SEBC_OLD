```
checked master

For Swappniess

[root@ip-172-31-1-176 etc]# cat /proc/sys/vm/swappiness
1
root@ip-172-31-1-176 etc]# df -aTH
Filesystem     Type         Size  Used Avail Use% Mounted on
/dev/xvde      ext4         8.5G  682M  7.4G   9% /
proc           proc            0     0     0    - /proc
sysfs          sysfs           0     0     0    - /sys
devpts         devpts          0     0     0    - /dev/pts
tmpfs          tmpfs        7.9G     0  7.9G   0% /dev/shm
none           binfmt_misc     0     0     0    - /proc/sys/fs/binfmt_misc

For Transparent hugepages

[root@ip-172-31-1-176 mm]# cat /etc/grub.conf
default=0
timeout=1

title CentOS-6.5-x86_64-GA-03 2.6.32-431.el6.x86_64
        root (hd0)
        kernel /boot/vmlinuz-2.6.32-431.el6.x86_64 root=LABEL=centos_root ro 
        initrd /boot/initramfs-2.6.32-431.el6.x86_64.img
transparent_hugepage=never


checking the network interface attributes

[root@ip-172-31-1-176 network-scripts]# cat ifcfg-eth0
DEVICE=eth0
BOOTPROTO=dhcp
ONBOOT=on


```
