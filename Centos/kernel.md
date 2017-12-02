# Kernel Informations
## Author : Jérôme Masson <sphinxgaia@jeromemasson.fr>

## Found your kernel version

```bash
uname -sr
```

## Update your kernel

Import repository ELrepo :

~~~bash
rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org
rpm -Uvh http://www.elrepo.org/elrepo-release-7.0-3.el7.elrepo.noarch.rpm
~~~

Control your repo & list kernel :

~~~bash
yum --disablerepo="*" --enablerepo="elrepo-kernel" list available
~~~

Install the latest mainline kernel :

~~~bash
yum --enablerepo=elrepo-kernel install kernel-ml
~~~

## Update your GRUB

Edit your grub and change line `GRUB_DEFAULT` into `GRUB_DEFAULT=0`

Recreate Kernel configuration

~~~bash
grub2-mkconfig -o /boot/grub2/grub.cfg
~~~

Reboot to see change

~~~bash
reboot
~~~

## Greetings

[Gabriel Cánepa on Tecmint website](https://www.tecmint.com/install-upgrade-kernel-version-in-centos-7/)
