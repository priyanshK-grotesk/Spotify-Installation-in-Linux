# Spotify Installation in linux


## Commands for Installation of Spotify in Linux Terminal

- [ ] curl -sS https://download.spotify.com/debian/pubkey_5E3C45D7B312C643.gpg | sudo apt-key add -
- [ ] echo "deb http://repository.spotify.com stable non-free" | sudo tee /etc/apt/sources.list.d/spotify.list
- [ ] sudo apt-get update && sudo apt-get install spotify-client

```
┌──(kali㉿kali)-[~]
└─$ curl -sS https://download.spotify.com/debian/pubkey_5E3C45D7B312C643.gpg | sudo apt-key add -

[sudo] password for kali:
Warning: apt-key is deprecated. Manage keyring files in trusted.gpg.d instead (see apt-key(8)).
OK

┌──(kali㉿kali)-[~]
└─$ echo "deb http://repository.spotify.com stable non-free" | sudo tee /etc/apt/sources.list.d/spotify.list

deb http://repository.spotify.com stable non-free

┌──(kali㉿kali)-[~]
└─$ sudo apt-get update && sudo apt-get install spotify-client

Get:1 http://repository.spotify.com stable InRelease [3,316 B]
Get:2 http://kali.cs.nctu.edu.tw/kali kali-rolling InRelease [30.6 kB]
Get:3 http://repository.spotify.com stable/non-free amd64 Packages [1,671 B]
Get:4 http://kali.cs.nctu.edu.tw/kali kali-rolling/main amd64 Packages [18.6 MB]
Get:5 http://kali.cs.nctu.edu.tw/kali kali-rolling/main amd64 Contents (deb) [43.3 MB]
Get:6 http://kali.cs.nctu.edu.tw/kali kali-rolling/contrib amd64 Packages [110 kB]
Get:7 http://kali.cs.nctu.edu.tw/kali kali-rolling/contrib amd64 Contents (deb) [161 kB]
Get:8 http://kali.cs.nctu.edu.tw/kali kali-rolling/non-free amd64 Packages [223 kB]
Get:9 http://kali.cs.nctu.edu.tw/kali kali-rolling/non-free amd64 Contents (deb) [895 kB]
Fetched 63.4 MB in 1min 6s (959 kB/s)
Reading package lists... Done
W: http://repository.spotify.com/dists/stable/InRelease: Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libaribb24-0 libopencore-amrnb0 libopencore-amrwb0 libx264-163
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  gconf-service gconf2-common libavcodec58 libavformat58 libavutil56
  libgconf-2-4 libsrt1.4-gnutls libswresample3
Suggested packages:
  libcuda1 libnvcuvid1 libnvidia-encode1
The following packages will be REMOVED:
  libavcodec-extra58
The following NEW packages will be installed:
  gconf-service gconf2-common libavcodec58 libavformat58 libgconf-2-4
  libsrt1.4-gnutls spotify-client
The following packages will be upgraded:
  libavutil56 libswresample3
2 upgraded, 7 newly installed, 1 to remove and 963 not upgraded.
Need to get 129 MB of archives.
After this operation, 310 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://repository.spotify.com stable/non-free amd64 spotify-client amd64 1:1.1.84.716.gc5f8b819 [120 MB]
Get:2 http://kali.cs.nctu.edu.tw/kali kali-rolling/main amd64 gconf2-common all 3.2.6-7 [1,039 kB]
Get:3 http://http.kali.org/kali kali-rolling/main amd64 libgconf-2-4 amd64 3.2.6-7+b1 [428 kB]
Get:4 http://http.kali.org/kali kali-rolling/main amd64 gconf-service amd64 3.2.6-7+b1 [416 kB]
Get:5 http://http.kali.org/kali kali-rolling/main amd64 libswresample3 amd64 7:4.4.2-1+b3 [103 kB]
Get:6 http://http.kali.org/kali kali-rolling/main amd64 libavutil56 amd64 7:4.4.2-1+b3 [307 kB]
Get:7 http://http.kali.org/kali kali-rolling/main amd64 libavcodec58 amd64 7:4.4.2-1+b3 [5,077 kB]
Get:8 http://http.kali.org/kali kali-rolling/main amd64 libsrt1.4-gnutls amd64 1.4.4-4+b1 [306 kB]
Get:9 http://http.kali.org/kali kali-rolling/main amd64 libavformat58 amd64 7:4.4.2-1+b3 [1,071 kB]
Fetched 129 MB in 1min 54s (1,131 kB/s)
(Reading database ... 338510 files and directories currently installed.)
Removing libavcodec-extra58:amd64 (7:4.4.2-1+b1) ...
Selecting previously unselected package gconf2-common.
(Reading database ... 338502 files and directories currently installed.)
Preparing to unpack .../0-gconf2-common_3.2.6-7_all.deb ...
Unpacking gconf2-common (3.2.6-7) ...
Selecting previously unselected package libgconf-2-4:amd64.
Preparing to unpack .../1-libgconf-2-4_3.2.6-7+b1_amd64.deb ...
Unpacking libgconf-2-4:amd64 (3.2.6-7+b1) ...
Selecting previously unselected package gconf-service.
Preparing to unpack .../2-gconf-service_3.2.6-7+b1_amd64.deb ...
Unpacking gconf-service (3.2.6-7+b1) ...
Preparing to unpack .../3-libswresample3_7%3a4.4.2-1+b3_amd64.deb ...
Unpacking libswresample3:amd64 (7:4.4.2-1+b3) over (7:4.4.2-1+b1) ...
Preparing to unpack .../4-libavutil56_7%3a4.4.2-1+b3_amd64.deb ...
Unpacking libavutil56:amd64 (7:4.4.2-1+b3) over (7:4.4.2-1+b1) ...
Selecting previously unselected package libavcodec58:amd64.
Preparing to unpack .../5-libavcodec58_7%3a4.4.2-1+b3_amd64.deb ...
Unpacking libavcodec58:amd64 (7:4.4.2-1+b3) ...
Selecting previously unselected package libsrt1.4-gnutls:amd64.
Preparing to unpack .../6-libsrt1.4-gnutls_1.4.4-4+b1_amd64.deb ...
Unpacking libsrt1.4-gnutls:amd64 (1.4.4-4+b1) ...
Selecting previously unselected package libavformat58:amd64.
Preparing to unpack .../7-libavformat58_7%3a4.4.2-1+b3_amd64.deb ...
Unpacking libavformat58:amd64 (7:4.4.2-1+b3) ...
Selecting previously unselected package spotify-client.
Preparing to unpack .../8-spotify-client_1%3a1.1.84.716.gc5f8b819_amd64.deb ...
Unpacking spotify-client (1:1.1.84.716.gc5f8b819) ...
Setting up libsrt1.4-gnutls:amd64 (1.4.4-4+b1) ...
Setting up libavutil56:amd64 (7:4.4.2-1+b3) ...
Setting up gconf2-common (3.2.6-7) ...

Creating config file /etc/gconf/2/path with new version
Setting up libswresample3:amd64 (7:4.4.2-1+b3) ...
Setting up libavcodec58:amd64 (7:4.4.2-1+b3) ...
Setting up libavformat58:amd64 (7:4.4.2-1+b3) ...
Processing triggers for sgml-base (1.30) ...
Processing triggers for kali-menu (2022.3.1) ...
Setting up libgconf-2-4:amd64 (3.2.6-7+b1) ...
Processing triggers for libc-bin (2.33-8) ...
Setting up spotify-client (1:1.1.84.716.gc5f8b819) ...
Setting up gconf-service (3.2.6-7+b1) ...

┌──(kali㉿kali)-[~]
└─$
```
