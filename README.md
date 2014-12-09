Threat Research Data
===============

## Summary

This page contains data I've collected over the past several months using a network of 10-20 SSH honeypots. If you have any questions or feedback, please don't hesitate to reach out and contact me. 

Credit to Robin Wood (Digininja) for building Pipal, the tool I used for statistical analysis on the passwords.  

Email:    andrew@morris.guru  
Twitter:  https://twitter.com/andrew___morris

## Statistics

#### Versions

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

#### Attacker IP Addresses

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

#### Usernames
*all_usernames_sorted.txt* contains a sorted list of all usernames ever attempted on any of my sensors.

Here are the top 25:
```
1181501 root  
  48138 admin
    308 www
    292 support
    243 test
    199 user
    199 guest
    189 ubnt
    161 ftpuser
    145 pi
    129 vyatta
    122 oracle
     88 ftp
     78 PlcmSpIp
     30 nagios
     30 adm
     29 alex
     27 postgres
     25 mysql
     23 info
     22 library
     22 adam
     20 backup
     19 mike
     18 uucp
```

#### Passwords

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

## Password Analysis

Total entries = 1231041  

Total unique entries = 203074

#### Top 10 passwords
```
admin = 5315 (0.43%)
- = 4377 (0.36%)
root = 4374 (0.36%)
_ = 1713 (0.14%)
123456 = 1524 (0.12%)
666666 = 1404 (0.11%)
888888 = 1251 (0.1%)
123456789 = 1242 (0.1%)
password = 1192 (0.1%)
12345 = 1082 (0.09%)
```
#### Top 10 base words
```
admin = 17153 (1.39%)
root = 11512 (0.94%)
password = 6471 (0.53%)
abcd = 3794 (0.31%)
p@ssw0rd = 3030 (0.25%)
passw0rd = 2701 (0.22%)
qwer = 2604 (0.21%)
test = 2389 (0.19%)
qazxsw = 2271 (0.18%)
qwerty = 2221 (0.18%)
```
#### Password length (length ordered)
```
1 = 7707 (0.63%)
2 = 4763 (0.39%)
3 = 19048 (1.55%)
4 = 77799 (6.32%)
5 = 104517 (8.49%)
6 = 253938 (20.63%)
7 = 190083 (15.44%)
8 = 246335 (20.01%)
9 = 130317 (10.59%)
10 = 82876 (6.73%)
11 = 41028 (3.33%)
12 = 28799 (2.34%)
13 = 12862 (1.04%)
14 = 10153 (0.82%)
15 = 6280 (0.51%)
16 = 7063 (0.57%)
17 = 1952 (0.16%)
18 = 1536 (0.12%)
19 = 486 (0.04%)
20 = 760 (0.06%)
21 = 413 (0.03%)
22 = 277 (0.02%)
23 = 608 (0.05%)
24 = 72 (0.01%)
25 = 148 (0.01%)
26 = 64 (0.01%)
27 = 429 (0.03%)
28 = 19 (0.0%)
29 = 16 (0.0%)
30 = 7 (0.0%)
31 = 73 (0.01%)
32 = 265 (0.02%)
33 = 63 (0.01%)
34 = 10 (0.0%)
35 = 6 (0.0%)
36 = 140 (0.01%)
38 = 2 (0.0%)
39 = 1 (0.0%)
41 = 53 (0.0%)
45 = 67 (0.01%)
48 = 6 (0.0%)
```
#### Password length (count ordered)
```
6 = 253938 (20.63%)
8 = 246335 (20.01%)
7 = 190083 (15.44%)
9 = 130317 (10.59%)
5 = 104517 (8.49%)
10 = 82876 (6.73%)
4 = 77799 (6.32%)
11 = 41028 (3.33%)
12 = 28799 (2.34%)
3 = 19048 (1.55%)
13 = 12862 (1.04%)
14 = 10153 (0.82%)
1 = 7707 (0.63%)
16 = 7063 (0.57%)
15 = 6280 (0.51%)
2 = 4763 (0.39%)
17 = 1952 (0.16%)
18 = 1536 (0.12%)
20 = 760 (0.06%)
23 = 608 (0.05%)
19 = 486 (0.04%)
27 = 429 (0.03%)
21 = 413 (0.03%)
22 = 277 (0.02%)
32 = 265 (0.02%)
25 = 148 (0.01%)
36 = 140 (0.01%)
31 = 73 (0.01%)
24 = 72 (0.01%)
45 = 67 (0.01%)
26 = 64 (0.01%)
33 = 63 (0.01%)
41 = 53 (0.0%)
28 = 19 (0.0%)
29 = 16 (0.0%)
34 = 10 (0.0%)
30 = 7 (0.0%)
35 = 6 (0.0%)
48 = 6 (0.0%)
38 = 2 (0.0%)
39 = 1 (0.0%)
```
```
      | |                                                               
      | |                                                               
      | |                                                               
      | |                                                               
      |||                                                               
      |||                                                               
      |||                                                               
      ||||                                                              
      ||||                                                              
     |||||                                                              
     ||||||                                                             
    |||||||                                                             
    |||||||                                                             
    ||||||||                                                            
   ||||||||||                                                           
|||||||||||||||||||||||||||||||||||||||||||||||||                       
0000000000111111111122222222223333333333444444444
0123456789012345678901234567890123456789012345678
```
```
One to six characters = 467772 (38.0%)
One to eight characters = 904190 (73.45'%)
More than eight characters = 326851 (26.55%)
```
```
Only lowercase alpha = 573318 (46.57%)
Only uppercase alpha = 10308 (0.84%)
Only alpha = 583626 (47.41%)
Only numeric = 132800 (10.79%)
```
```
First capital last symbol = 4447 (0.36%)
First capital last number = 23727 (1.93%)
```
```
Single digit on the end = 70548 (5.73%)
Two digits on the end = 40963 (3.33%)
Three digits on the end = 89652 (7.28%)
```
#### Last number
```
0 = 40457 (3.29%)
1 = 81857 (6.65%)
2 = 32058 (2.6%)
3 = 85484 (6.94%)
4 = 35586 (2.89%)
5 = 31688 (2.57%)
6 = 41747 (3.39%)
7 = 26156 (2.12%)
8 = 35182 (2.86%)
9 = 31178 (2.53%)

 | |                                                                    
 | |                                                                    
 | |                                                                    
 | |                                                                    
 | |                                                                    
 | |                                                                    
 | |                                                                    
 | |                                                                    
|| |  |                                                                 
||||| | |                                                               
||||||| ||                                                              
||||||||||                                                              
||||||||||                                                              
||||||||||                                                              
||||||||||                                                              
||||||||||                                                              
0123456789
```
#### Last digit
```
3 = 85484 (6.94%)
1 = 81857 (6.65%)
6 = 41747 (3.39%)
0 = 40457 (3.29%)
4 = 35586 (2.89%)
8 = 35182 (2.86%)
2 = 32058 (2.6%)
5 = 31688 (2.57%)
9 = 31178 (2.53%)
7 = 26156 (2.12%)
```
#### Last 2 digits (Top 10)
```
23 = 60693 (4.93%)
56 = 19453 (1.58%)
21 = 12441 (1.01%)
34 = 11732 (0.95%)
11 = 10763 (0.87%)
12 = 9981 (0.81%)
88 = 9526 (0.77%)
00 = 9488 (0.77%)
89 = 9424 (0.77%)
45 = 9290 (0.75%)
```
#### Last 3 digits (Top 10)
```
123 = 57236 (4.65%)
456 = 16931 (1.38%)
234 = 10791 (0.88%)
321 = 7323 (0.59%)
789 = 6579 (0.53%)
345 = 5727 (0.47%)
888 = 5137 (0.42%)
000 = 5010 (0.41%)
111 = 4753 (0.39%)
520 = 4632 (0.38%)
```
#### Last 4 digits (Top 10)
```
3456 = 14418 (1.17%)
1234 = 10075 (0.82%)
2345 = 5514 (0.45%)
2008 = 4099 (0.33%)
6789 = 3513 (0.29%)
1314 = 3273 (0.27%)
4321 = 3123 (0.25%)
4567 = 2868 (0.23%)
1111 = 2771 (0.23%)
3123 = 2524 (0.21%)
```

#### Last 5 digits (Top 10)
```
23456 = 14059 (1.14%)
12345 = 5282 (0.43%)
56789 = 3323 (0.27%)
34567 = 2677 (0.22%)
23123 = 2356 (0.19%)
54321 = 2095 (0.17%)
23445 = 2077 (0.17%)
11111 = 1835 (0.15%)
45678 = 1783 (0.14%)
88888 = 1742 (0.14%)
```
#### Character sets
```
loweralpha: 573318 (46.57%)
loweralphanum: 340639 (27.67%)
numeric: 132800 (10.79%)
loweralphaspecialnum: 40906 (3.32%)
mixedalpha: 30414 (2.47%)
mixedalphanum: 21435 (1.74%)
loweralphaspecial: 16936 (1.38%)
mixedalphaspecialnum: 12193 (0.99%)
upperalphanum: 11058 (0.9%)
upperalpha: 10308 (0.84%)
specialnum: 8651 (0.7%)
special: 7638 (0.62%)
mixedalphaspecial: 2926 (0.24%)
upperalphaspecialnum: 2174 (0.18%)
upperalphaspecial: 1933 (0.16%)
```
#### Character set ordering
```
allstring: 614040 (49.88%)
stringdigit: 255448 (20.75%)
alldigit: 132800 (10.79%)
othermask: 113919 (9.25%)
digitstring: 39414 (3.2%)
stringdigitstring: 30224 (2.46%)
stringspecialdigit: 12542 (1.02%)
stringspecialstring: 9118 (0.74%)
allspecial: 7638 (0.62%)
digitstringdigit: 7062 (0.57%)
stringspecial: 6014 (0.49%)
specialstring: 1959 (0.16%)
specialstringspecial: 863 (0.07%)
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

