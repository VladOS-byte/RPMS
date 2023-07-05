# About

What's app! There are a lot of options to download [iRZ Collector](https://www.radiofid.ru/programmnoe-obespechenie/irz-collector/) Software.

# NEWS

📣 iRZ Collector 4.2 added. You can download iRZ Collector Server ([RPM](collector/Server/4/2/iRZ_Server-4-2.noarch.rpm) or [DEB](collector/Server/4/2/iRZ-Server_4-2_all.deb)), and iRZ Dispatcher ([RPM](collector/Dispatcher/4/2/iRZ_Dispatcher-4-2.noarch.rpm) or [DEB](collector/Dispatcher/4/2/iRZ-Dispatcher_4-2_all.deb)) using tutorial with changing version - revision index (3.2 -> 4.2).

📣 iRZ Collector 4.1 added. You can download iRZ Collector Server ([RPM](collector/Server/4/1/iRZ_Server-4-1.noarch.rpm) or [DEB](collector/Server/4/1/iRZ-Server_4-1_all.deb)), and iRZ Dispatcher ([RPM](collector/Dispatcher/4/1/iRZ_Dispatcher-4-1.noarch.rpm) or [DEB](collector/Dispatcher/4/1/iRZ-Dispatcher_4-1_all.deb)) using tutorial with changing version - revision index (3.2 -> 4.1).

📣 iRZ Collector 4.0 added. You can download iRZ Collector Server ([RPM](collector/Server/4/0/iRZ_Server-4-0.noarch.rpm) or [DEB](collector/Server/4/0/iRZ-Server_4-0_all.deb)), and iRZ Dispatcher ([RPM](collector/Dispatcher/4/0/iRZ_Dispatcher-4-0.noarch.rpm) or [DEB](collector/Dispatcher/4/0/iRZ-Dispatcher_4-0_all.deb)) using tutorial with changing version - revision index (3.2 -> 4.0).

📣 iRZ Collector Server 3.3 added. You can download it ([RPM](collector/Server/3/3/iRZ_Server-3-3.noarch.rpm) or [DEB](collector/Server/3/3/iRZ-Server_3-3_all.deb)) using tutorial with changing version - revision index (3.2 -> 3.3).

📣 iRZ Dispatcher 3.3 added. You can download it ([RPM](collector/Dispatcher/3/3/iRZ_Dispatcher-3-3.noarch.rpm) or [DEB](collector/Dispatcher/3/3/iRZ-Dispatcher_3-3_all.deb)) using tutorial with changing file name (Server -> Dispatcher) and version - revision index (3.2 -> 3.3).

📣 Add tar.gz archives for all repos.

# TAR

You can use <code>tar</code> utility in your terminal for unzip archive and use it by command:

~~~
tar -xzvf iRZ_Server-3.2.tar.gz
~~~

You can create link or use <code>configurator.sh</code> script native.

# RPM

[collector/Server/3/2/iRZ_Server-3-2.noarch.rpm](collector/Server/3/2/iRZ_Server-3-2.noarch.rpm) - iRZ Collector Server version 3 and revision 2 for Fedora Kernel

You can install Server by simple command:

~~~
yum install https://github.com/VladOS-byte/RPMS/raw/main/collector/Server/3/2/iRZ_Server-3-2.noarch.rpm
~~~

or

~~~
rpm --install https://github.com/VladOS-byte/RPMS/raw/main/collector/Server/3/2/iRZ_Server-3-2.noarch.rpm
~~~

or

~~~
wget https://github.com/VladOS-byte/RPMS/raw/main/collector/Server/3/2/iRZ_Server-3-2.noarch.rpm
rpm --install iRZ_Server-3-2.noarch.rpm
~~~

# DEB

[collector/iRZ-Server_3-2_all.deb](collector/Server/3/2/iRZ-Server_3-2_all.deb) - iRZ Collector Server version 3 and revision 2 for Debian Kernel

You can install Server by multiple command:

~~~
TEMP_DEB="$(mktemp)" &&
wget -O "$TEMP_DEB" 'https://github.com/VladOS-byte/RPMS/raw/main/collector/Server/3/2/iRZ-Server_3-2_all.deb' &&
sudo dpkg --install "$TEMP_DEB" &&
rm -f "$TEMP_DEB"
~~~

... or use [lynx](https://linux.die.net/man/1/lynx)
~~~
lynx https://github.com/VladOS-byte/RPMS/raw/main/collector/Server/3/2/iRZ-Server_3-2_all.deb
dpkg --install irz-server_3-2_all.deb
~~~

After create link for collector server access
~~~
ln -s -f /usr/local/iRZ_Server/configurator.sh /usr/local/bin/collector
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

... or <code>bash collector</code>. You can use <code>dispatcher</code> too.

If pseudo is broken, use
~~~
bash /usr/local/iRZ_Server/configurator.sh
~~~
or
~~~
bash /usr/local/iRZ_Server/dispatcher.sh
~~~

In the second usage You can use option <code>--hard</code> to ignore check any unsupported requirements.

More information about iRZ Collector You can find on https://www.radiofid.ru

