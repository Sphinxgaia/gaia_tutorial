# Manipulation package
## Author : Jérôme Masson <sphinxgaia@jeromemasson.fr>

## YUM
yum is command to install package

~~~bash
yum isntall
yum uninstall
~~~

## Found a package that provides a command
~~~bash
yum provides ifconfig
yum whatprovides ifconfig
~~~

## Repository

Import GPG Key ELrepo :

~~~bash
rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org
~~~

Add repository ELrepo :

~~~bash
rpm -Uvh http://www.elrepo.org/elrepo-release-7.0-3.el7.elrepo.noarch.rpm
~~~
