---
description: Here is the complete write-up for the bandit war games for all levels (0-34)
cover: >-
  https://images.unsplash.com/photo-1588450248442-1c8357368dba?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwxfHx3YXJnYW1lc3xlbnwwfHx8fDE2ODMwMzE2NzI&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🧨 Bandit Wargames

To get started with each level we need to login through SSH and try to crack password for each next level using the password found in current level.

## Level 0

**Username:** bandit0**, Password:** bandit0

```
$ ssh bandit0@bandit.labs.overthewire.org -p 2220
PASSWORD: bandit0

bandit0@bandit$ cat readme
NH2SXQwc-------
```

## Level 1

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is **bandit.labs.overthewire.org**, on port 2220. The username is **bandit0** and the password is **bandit0**. Once logged in, go to the [Level 1](https://overthewire.org/wargames/bandit/bandit1.html) page to find out how to beat Level&#x20;

```
bandit1@bandit:~$ cat ./-
rRGizSaX8--------
```

## Level 2

```
bandit2@bandit:~$ cat spaces\ in\ this\ filename
aBZ0W5EmUf-------
```

## Level 3

```
bandit3@bandit:~$ cat ./inhere/.hidden
2EW7BBsr6a-------
```

## Level 4

```
bandit4@bandit:~$ file ./inhere/*
./inhere/-file00: data
./inhere/-file01: data
./inhere/-file02: data
./inhere/-file03: data
./inhere/-file04: data
./inhere/-file05: data
./inhere/-file06: data
./inhere/-file07: ASCII text
./inhere/-file08: data
./inhere/-file09: Non-ISO extended-ASCII text, with no line terminators
bandit4@bandit:~$ cat ./inhere/-file07
lrIWWI6bB--------
```

## Level 5

```
bandit5@bandit:~/inhere$ du ./ -ab | grep 1033
1033    ./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
P4L4vucdm-------
```

## Level 6

```
bandit6@bandit:~$ mkdir /tmp/tmpdir
bandit6@bandit:~$ find / -user bandit7 -group bandit6  2>/tmp/tmpdir/temp
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
z7WtoNQ----------
```

## Level 7

```
bandit7@bandit:~$ head data.txt
Worcester's     fyKdWWh7VVgusiIKPygHJe6TlkDHhLHl
arousal r8mfBurE2OvHu8NFQc7mJ2x14iNjwkin
counterespionage's      4jmzYqFkqwciprPrJleFCI9tyjbXBtdt
Willard's       ctbhPNPRDGAll4Whhsrz3Mwv6qJHM8Et
midwife Kk9VZkoTUNUfmIa031vovUN2UKksZ56S
rookie  LVU5eslJrzjrXQh4SsuSL07f7zQbwuDu
fezes   Twv6nvASc3pqIHLO9jEvrsYSKbHpSr6H
east    3iBmPOvNXWLs8L6OuLCUGQ37SEQdM8K7
preeminence's   qmAHcCxMawJxe3vHBFhL9eNWtErnoSHS
stirred rsR2z31uFFiYWll1W1kGr38wLN6FAHgN
bandit7@bandit:~$ grep millionth data.txt
millionth       TESKZC0XvTe-------------

```

## Level 8

```
bandit8@bandit:~$ ls
data.txt
bandit8@bandit:~$ cat data.txt | sort | uniq -u
EN632Plf--------
```

## Level 9

```
bandit9@bandit:~$ ls
data.txt
bandit9@bandit:~$ strings data.txt | grep ===
4========== the#
========== password
========== is
========== G7w8LIi6J3kT-------------
```

## Level 10

```
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt
VGhlIHBhc3N3b3JkIGlzIDZ6UGV6aUxkUjJSS05kTllGTmI2blZDS3pwaGxYSEJNCg==
bandit10@bandit:~$ base64 -d data.txt
The password is 6zPeziLdR2-------------

```

## Level 11

```
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi
bandit11@bandit:~$ cat data.txt  | tr 'A-Za-z'  'N-ZA-Mn-za-m'
The password is JVNBBFSmZwKK-------------

```

## Level 12

```
bandit12@bandit:~$ ls
data.txt
bandit12@bandit:~$ mkdir /tmp/testme
bandit12@bandit:~$ cp data.txt /tmp/testme
bandit12@bandit:~$ cd /tmp/testme
bandit12@bandit:/tmp/testme$ ls
data.txt
bandit12@bandit:/tmp/testme$ cat data.txt
00000000: 1f8b 0808 2773 4564 0203 6461 7461 322e  ....'sEd..data2.
00000010: 6269 6e00 0145 02ba fd42 5a68 3931 4159  bin..E...BZh91AY
00000020: 2653 597b 4f96 5f00 0018 ffff fd6f e7ed  &SY{O._......o..
00000030: bff7 bef7 9fdb d7ca ffbf edff 8ded dfd7  ................
00000040: bfe7 bbff bfdb fbff ffbf ff9f b001 3b56  ..............;V
00000050: 0400 0068 0064 3400 d341 a000 0680 0699  ...h.d4..A......
00000060: 0000 69a0 0000 1a00 1a0d 0034 0034 d3d4  ..i........4.4..
00000070: d1a3 d464 6834 6403 d469 b422 0d00 3400  ...dh4d..i."..4.
00000080: 1a68 068d 3403 4d06 8d00 0c80 00f5 0003  .h..4.M.........
00000090: 4031 3119 00d0 1a68 1a34 c86d 4640 00d0  @11....h.4.mF@..
000000a0: 0007 a80d 000d 00e9 a340 d034 0341 a000  .........@.4.A..
000000b0: 0699 07a9 881e a0d0 da80 6834 0c43 4068  ..........h4.C@h
000000c0: 6432 0340 0c80 6800 0346 8006 8000 d034  d2.@..h..F.....4
000000d0: 0001 f0e1 810e 1958 b7a4 92c7 640e 421a  .......X....d.B.
000000e0: a147 6142 a67e 3603 a756 3ba9 1b08 e034  .GaB.~6..V;....4
000000f0: 41fd 1247 661d b380 00b7 cd8c b23e b6b2  A..Gf........>..
00000100: 1947 e803 0be5 6077 a542 e9ea 7810 29f0  .G....`w.B..x.).
00000110: 429d e1d7 ad8b 0b78 056b e37c 06df 4917  B......x.k.|..I.
00000120: 9b46 f69d 4473 80b4 edc2 ee10 04e3 3e52  .F..Ds........>R
00000130: dd34 2244 08cb 5e64 9314 9521 505e e767  .4"D..^d...!P^.g
00000140: 9021 d029 85e7 9ce2 d1ce d44f 5ec5 f6d6  .!.).......O^...
00000150: d918 de31 f1f5 d149 4695 0937 d06b f046  ...1...IF..7.k.F
00000160: 789d 1bd0 ca69 11eb 2c9a 3290 3d9e 0511  x....i..,.2.=...
00000170: 6cad 205b edc8 c4b5 4691 379a 5978 58c3  l. [....F.7.YxX.
00000180: 4846 a4a0 3ba5 a89a a794 1f93 c588 8160  HF..;..........`
00000190: 016e 2504 2c74 643b 5046 4154 751c 33b1  .n%.,td;PFATu.3.
000001a0: c3e5 53d8 a959 5fdc 6c12 f2bd 02f3 2d83  ..S..Y_.l.....-.
000001b0: b965 3188 0d3c b097 4156 e950 9d49 64f6  .e1..<..AV.P.Id.
000001c0: da4a 2db5 a4ea 5365 27c0 1e79 8109 5f31  .J-...Se'..y.._1
000001d0: c184 46c9 74a5 f923 5ea1 6861 f058 226c  ..F.t..#^.ha.X"l
000001e0: 3df6 5d10 d11f d966 77c9 e488 448c 5a6f  =.]....fw...D.Zo
000001f0: 2c10 410b 4280 140a 0818 8afa 0cfa 8bf7  ,.A.B...........
00000200: ad34 3308 4077 6552 9849 378e 7d85 1fd8  .43.@weR.I7.}...
00000210: f287 1238 7639 11e2 f1e6 483b 7548 25e2  ...8v9....H;uH%.
00000220: 7de4 24ff 1a69 0b85 4b4c ebd0 1231 a512  }.$..i..KL...1..
00000230: f9fb 109c e7ea d932 98fd eb76 f4f8 fa29  .......2...v...)
00000240: 967c e152 9c69 c607 6207 eaef 2095 9441  .|.R.i..b... ..A
00000250: a64e 9ffc 5dc9 14e1 4241 ed3e 597c 9f2e  .N..]...BA.>Y|..
00000260: f0c8 4502 0000                           ..E...
bandit12@bandit:/tmp/testme$ xxd -r data.txt > data01
bandit12@bandit:/tmp/testme$ file data01
data01: gzip compressed data, was "data2.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix, original size modulo 2^32 581
bandit12@bandit:/tmp/testme$ gunzip -N data01
gzip: data01: unknown suffix -- ignored
bandit12@bandit:/tmp/testme$ ls
data01  data.txt
bandit12@bandit:/tmp/testme$ gunzip -c data01 > data02
bandit12@bandit:/tmp/testme$ file data02
data02: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/testme$ ls
data01  data02  data.txt
bandit12@bandit:/tmp/testme$ bunzip2 -c data02 > data03
bandit12@bandit:/tmp/testme$ file data03
data03: gzip compressed data, was "data4.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix, original size modulo 2^32 20480
bandit12@bandit:/tmp/testme$ gunzip -c data03 > data04
bandit12@bandit:/tmp/testme$ file data04
data04: POSIX tar archive (GNU)
bandit12@bandit:/tmp/testme$ tar -xf data04
bandit12@bandit:/tmp/testme$ ls
data01  data02  data03  data04  data5.bin  data.txt
bandit12@bandit:/tmp/testme$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@bandit:/tmp/testme$ tar -xf data5.bin
bandit12@bandit:/tmp/testme$ ls
data01  data02  data03  data04  data5.bin  data6.bin  data.txt
bandit12@bandit:/tmp/testme$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/testme$ bunzip2 -c data6.bin > data07
bandit12@bandit:/tmp/testme$ file data07
data07: POSIX tar archive (GNU)
bandit12@bandit:/tmp/testme$ tar -xf data07
bandit12@bandit:/tmp/testme$ ls
data01  data02  data03  data04  data07  data5.bin  data6.bin  data8.bin  data.txt
bandit12@bandit:/tmp/testme$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix, original size modulo 2^32 49
bandit12@bandit:/tmp/testme$ gunzip -c data8.bin > data09
bandit12@bandit:/tmp/testme$ file data09
data09: ASCII text
bandit12@bandit:/tmp/testme$ cat data09
The password is wbWdlBxEir4-----------
```

## Level 13

```
```

## Level 14

```
```

## Level 15

```
```

## Level 16

```
```

## Level 17

```
```

## Level 18

```
```

## Level 19

```
```

## Level 20

```
```

## Level 21

```
```

## Level 22

```
```

## Level 23

```
```

## Level 24

```
```

## Level 25

```
```

## Level 26

```
```

## Level 27

```
```

## Level 28

```
```

## Level 29

```
```

## Level 30

```
```

## Level 31

```
```

## Level 32

```
```

## Level 33

```
```

