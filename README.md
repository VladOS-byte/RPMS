# RPM

[collector/iRZ_Collector-3-2.noarch.rpm](collector/iRZ_Collector-3-2.noarch.rpm) - iRZ Collector version 3 and revision 2 for Fedora Kernel

You can install Collector by simple command:

~~~
yum install https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ_Collector-3-2.noarch.rpm
~~~

or

~~~
rpm --install https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ_Collector-3-2.noarch.rpm
~~~

# DEB

[collector/iRZ-Collector_3-2_all.deb](collector/iRZ-Collector_3-2_all.deb) - iRZ Collector version 3 and revision 2 for Debian Kernel

You can install Collector by multiple command:

~~~
TEMP_DEB="$(mktemp)" &&
wget -O "$TEMP_DEB" 'https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ-Collector_3-2_all.deb' &&
sudo dpkg --intsall "$TEMP_DEB" &&
rm -f "$TEMP_DEB"
~~~

... or use [lynx](https://linux.die.net/man/1/lynx)
~~~
lynx https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ-Collector_3-2_all.deb
dpkg --install irz-collector_3-2_all.deb
~~~

