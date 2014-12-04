Threat Research Data
===============

#### HKGroup

12/04/2014

Ongoing attack from Hong Kong targeting SSH servers on the open Internet. Attacks started at the end of November 2014 and are still going through early December 2014.

Attacks are originating from the 103.41.124.0/24 range.

Here are the top 25 passwords being used:

```
    196 
    143 123456
    142 ,.
    108 123
     87 hoang
     87 hitech
     87 hemmelig
     87 heeralal
     87 Hedwig
     87 harry123
     87 harper
     87 hamid
     87 guests
     87 guessit
     87 guess
     87 gratis
     87 grateful
     87 google.com
     87 goodday
     87 girlpower
     87 gigi
     87 ggggggg
     87 getout
     87 getlost123
     87 gerhard
```
(the sorting is kind of weird because multiple machines are using the same wordlist, and I have a bunch of honeypots)

*hkgroup_passwords_sorted.txt* includes all password attempts. The file contains roughly 26,000 unique passwords.

#### Statistics

*versions.txt* is a running list of all SSH versions I've seen connecting to my sensors.

Here are the top 10:

```
 205755 SSH-2.0-PUTTY
  29350 SSH-2.0-libssh2_1.4.2
  16103 SSH-2.0-libssh2_1.4.3
   3045 SSH-2.0-PuTTY_Release_0.63
   2387 SSH-2.0-JSCH-0.1.51
    771 SSH-2.0-libssh2_1.4.1
    390 SSH-2.0-paramiko_1.8.1
    214 SSH-2.0-libssh2_1.0
    213 SSH-2.0-Granados-1.0
    157 SSH-2.0-OpenSSH_5.2
```

*all_passwords_sorted.txt* contains a sorted list of all passwords ever attempted against any of my sensors.

Here are the top 25:

```
   5315 admin
   4377 -
   4374 root
   1792 
   1713 _
   1524 123456
   1404 666666
   1251 888888
   1242 123456789
   1192 password
   1082 12345
   1041 1234
    982 123123
    934 1qaz2wsx
    932 1234567890
    930 admin123
    926 test
    922 12345678
    901 qwe123
    881 P@ssw0rd
    879 root123
    877 qweasd
    861 toor
    834 passw0rd
    833 123abc
```


As always, feel free to contact me if you have any questions or feedback.  

andrew@morris.guru  
@andrew___morris  

