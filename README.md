Threat Research Data
===============

## Statistics

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

*all_ips_sorted.txt* is a includes all IP addresses that have ever tried to login to any of my sensors. 

Here are the top 25:

```
  60914 103.41.124.42
  45382 103.41.124.13
  41735 103.41.124.20
  39348 103.41.124.30
  34275 103.41.124.15
  32655 103.41.124.34
  29735 103.41.124.33
  29063 103.41.124.31
  27718 103.41.124.27
  27545 103.41.124.45
  22388 103.41.124.24
  21126 103.41.124.37
  19166 103.41.124.53
  15171 103.41.124.49
  13925 103.41.124.59
  11790 103.41.124.14
  10552 103.41.124.35
  10356 103.41.124.43
  10149 103.41.124.54
   9522 60.173.10.177
   9235 103.41.124.36
   8874 202.109.143.89
   8537 103.41.124.25
   8308 103.41.124.12
   7636 111.74.238.152
```

*all_ranges_sorted.txt* contains all class C IP ranges that have ever attempted to login to any of my sensors. Please keep in mind that this may contain some benign hosts, as I'm aggregating based on range, not necessarily host. Also, I've removed any networks that include less than 100 total malicious attempts to filter out small fish. If you'd like access to the raw data, don't hesitate to contact me.

Here are the top 25:

```
 612166 103.41.124.0/24
  75657 122.225.109.0/24
  61914 202.109.143.0/24
  53218 117.21.191.0/24
  51994 111.74.238.0/24
  45076 222.186.34.0/24
  33536 117.21.225.0/24
  29921 115.239.248.0/24
  29283 220.177.198.0/24
  23773 117.21.226.0/24
  22346 122.225.97.0/24
  18533 111.74.239.0/24
  16308 222.186.56.0/24
  13694 222.186.58.0/24
  12812 117.21.224.0/24
  11779 183.57.57.0/24
  11216 61.174.51.0/24
   9522 60.173.10.0/24
   6979 218.2.0.0/24
   6531 61.174.50.0/24
   6137 60.173.9.0/24
   5454 222.186.38.0/24
   4973 222.186.55.0/24
   4677 117.27.158.0/24
   4332 222.186.40.0/24
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

## Groups

#### HKGroup

12/04/2014

Ongoing attack from Hong Kong targeting SSH servers on the open Internet. Attacks started at the end of November 2014 $

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




As always, feel free to contact me if you have any questions or feedback.  

andrew@morris.guru  
@andrew___morris  

