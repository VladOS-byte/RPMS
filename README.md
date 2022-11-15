# NEWS

iRZ Collector 3.3 added. You can download it using tutorial with changing version - revision index (3.2 -> 3.3).

# RPM

[collector/iRZ_Server-3-2.noarch.rpm](collector/iRZ_Server-3-2.noarch.rpm) - iRZ Collector Server version 3 and revision 2 for Fedora Kernel

You can install Server by simple command:

~~~
yum install https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ_Server-3-2.noarch.rpm
~~~

or

~~~
rpm --install https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ_Server-3-2.noarch.rpm
~~~

or

~~~
wget https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ_Server-3-2.noarch.rpm
rpm --install iRZ_Server-3-2.noarch.rpm
~~~

# DEB

[collector/iRZ-Server_3-2_all.deb](collector/iRZ-Server_3-2_all.deb) - iRZ Collector Server version 3 and revision 2 for Debian Kernel

You can install Server by multiple command:

~~~
TEMP_DEB="$(mktemp)" &&
wget -O "$TEMP_DEB" 'https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ-Server_3-2_all.deb' &&
sudo dpkg --intsall "$TEMP_DEB" &&
rm -f "$TEMP_DEB"
~~~

... or use [lynx](https://linux.die.net/man/1/lynx)
~~~
lynx https://github.com/VladOS-byte/RPMS/raw/main/collector/iRZ-Server_3-2_all.deb
dpkg --install irz-server_3-2_all.deb
~~~

After create link for collector server access
~~~
ln -s /usr/local/iRZ_Server/dist/configurator.sh /usr/local/bin/collector
~~~

# Dependencies
Please, install dependencies.
You can see requirements after running <code>configurator.sh</code> script.
Use your package manager to install it.

# Usage
*need root rights.

~~~
collector
~~~ 

If pseudo is broken, use
~~~
bash /usr/local/iRZ_Server/dist/configurator.sh
~~~

In the second usage You can use option <code>--hard</code> to ignore check any unsupported requirements.

More information about iRZ Collector You can find on https://www.radiofid.ru

