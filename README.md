easyapache4-profiles
=============
This is based on CloudLinux + All PHP Options + ZendGuard cloudlinux profile and add extra mods.
Contains Apache 2.4, PHP 7.0, PHP 5.5, PHP 5.6, PHP 7.1, PHP 5.4, PHP 5.3, All PHP Opts, and mod_hostinglimits
Apache MPM: event 
Additional Mod: reqtimeout, env, ratelimit, cloudflare, proctitle, remoteip
Additional PHP Extensions: php70-php-ioncube6

Before using this profiles, we need to install cloudflare and protitle on easyapahce4.

Install cloudflare
-----------
CentOS 6:
```
wget -O /etc/yum.repos.d/EA4-Mod-Cloudflare.repo http://download.opensuse.org/repositories/home:/Jperkster:/EA4_Mod_Cloudflare/CentOS-6/home:Jperkster:EA4_Mod_Cloudflare.repo
yum install ea-apache24-mod_cloudflare
```
CentOS 7:
```
wget -O /etc/yum.repos.d/EA4-Mod-Cloudflare.repo http://download.opensuse.org/repositories/home:/Jperkster:/EA4_Mod_Cloudflare/CentOS-7/home:Jperkster:EA4_Mod_Cloudflare.repo
yum install ea-apache24-mod_cloudflare
```
-----------
Install proctitle
-----------
```
yum install ea-apache24-mod_proctitle
service httpd restart
```
-----------
