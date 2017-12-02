# Vmware Guest Companion

## Install VMware tool
~~~bash
yum install open-vm-tools
~~~

or

~~~bash
yum install perl

mkdir /mnt/cdrom

mount /dev/cdrom /mnt/cdrom

cd /tmp

cp /mnt/cdrom/VMwareTools-x.x.x-yyyy.tar.gz

tar zxpf /tmp/VMwareTools-x.x.x-yyyy.tar.gz

umount /dev/cdrom

cd vmware-tools-distrib
./vmware-install.pl
~~~
