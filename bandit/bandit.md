# Over The Wire - Bandit
```text
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
```

Faced a bit of trouble with the levels marked `(*)` 
I did them easily and learnt something new using the docs for levels marked with `(!)`

## Navigation

- [Level 0](#level-0)
- [Level 0 -> Level 1](#level-0---level-1)
- [Level 1 -> Level 2](#level-1---level-2)
- [Level 2 -> Level 3](#level-2---level-3)
- [Level 3 -> Level 4](#level-3---level-4)
- [Level 4 -> Level 5](#level-4---level-5)
- [Level 5 -> Level 6](#level-5---level-6)
- [Level 6 -> Level 7](#level-6---level-7)
- [Level 7 -> Level 8](#level-7---level-8)
- [Level 8 -> Level 9](#level-8---level-9)
- [Level 9 -> Level 10](#level-9---level-10)
- [Level 10 -> Level 11](#level-10---level-11)
- [Level 11 -> Level 12](#level-11---level-12)
- [Level 12 -> Level 13](#level-12---level-13)
- [Level 13 -> Level 14](#level-13---level-14)
- [Level 14 -> Level 15](#level-14---level-15)
- [Level 15 -> Level 16](#level-15---level-16)
- [Level 16 -> Level 17](#level-16---level-17)
- [Level 17 -> Level 18](#level-17---level-18)
- [Level 18 -> Level 19](#level-18---level-19)
- [Level 19 -> Level 20](#level-19---level-20)
- [Level 20 -> Level 21](#level-20---level-21)
- [Level 21 -> Level 22](#level-21---level-22)
- [Level 22 -> Level 23](#level-22---level-23)
- [Level 23 -> Level 24](#level-23---level-24)
- [Level 24 -> Level 25](#level-24---level-25)
- [Level 25 -> Level 26](#level-25---level-26)
- [Level 26 -> Level 27](#level-26---level-27)
- [Level 27 -> Level 28](#level-27---level-28)
- [Level 28 -> Level 29](#level-28---level-29)
- [Level 29 -> Level 30](#level-29---level-30)
- [Level 30 -> Level 31](#level-30---level-31)
- [Level 31 -> Level 32](#level-31---level-32)
- [Level 32 -> Level 33](#level-32---level-33)

## Level 0

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit0
```

I used the passwrod: bandit0

![level 0](./l0.png "Level 0")

## Level 0 -> Level 1

```bash
bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat readme
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit1
```
 
I used the password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

## Level 1 -> Level 2

`cat -` doesn't work because `-` as an argument refers to stdin and stdout

```bash
bandit1@bandit:~$ ls
-
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit2
```
 
I used the password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

## Level 2 -> Level 3

```bash
bandit2@bandit:~$ ls
--spaces in this filename--
bandit2@bandit:~$ cat ./--spaces\ in\ this\ filename--
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit3
```

I used the password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## Level 3 -> Level 4

```bash
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -la
total 12
drwxr-xr-x 2 root    root    4096 Aug 15 13:16 .
drwxr-xr-x 3 root    root    4096 Aug 15 13:16 ..
-rw-r----- 1 bandit4 bandit3   33 Aug 15 13:16 ...Hiding-From-You
bandit3@bandit:~/inhere$ cat ./...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit4
```

I used the password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

## Level 4 -> Level 5

```bash
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ cat ./-file00
��w��f�y�k��KSv�m�/��DGo��XI'bandit4@bandit:~/inhere$ cat ./-file01
�v��`�Rg.��v0>Oh        �]r�թ�i�L_ �Lbandit4@bandit:~/inhere$ cat ./-file02
����J��x"�.x�����l�x��mbandit4@bandit:~/inhere$ cat ./-file03
|�g򸌎�TU��uhjaW1���dS>�G��ycbandit4@bandit:~/inhere$ cat ./-file04
YQ�P��P���;�z�[;��ն�ë␦␦�bandit4@bandit:~/inhere$ cat ./-file05
����o�xv��y�0lkG�N��J4"��R&�bandit4@bandit:~/inhere$ cat ./-file06
1D��d
     ��M�l���1��nq�)�йbandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit5
```

I used the password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## Level 5 -> Level 6

```bash
bandit5@bandit:~/inhere$ cd ..
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ find ./ --size 1033c
find: unknown predicate `--size'
bandit5@bandit:~/inhere$ find ./ -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cd ./maybehere07/
bandit5@bandit:~/inhere/maybehere07$ cat ./.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit6
```

I used the password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Level 6 -> Level 7

```bash
bandit6@bandit:~$ find / -size 33c -user bandit7 -group bandit6
...
find: ‘/var/lib/polkit-1’: Permission denied
/var/lib/dpkg/info/bandit7.password
find: ‘/var/spool/bandit24’: Permission denied
...
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit7
```

I used the password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Level 7 -> Level 8

```bash
bandit7@bandit:~$ ls
data.txt
bandit7@bandit:~$ grep millionth data.txt
millionth       dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit8
```

I used the password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## Level 8 -> Level 9

```bash
bandit8@bandit:~$ ls
data.txt
bandit8@bandit:~$ sort data.txt | uniq -u
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit9
```

I used the password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## Level 9 -> Level 10

```bash
bandit9@bandit:~$ strings data.txt | grep ==
========== theg
========== password
========== is
========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit10
```

I used the password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## Level 10 -> Level 11

```bash
bandit10@bandit:~$ cat data.txt | base64 -d
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit11
```

I used the password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

## Level 11 -> Level 12

```bash
bandit11@bandit:~$ cat data.txt | tr A-Za-z N-ZA-Mn-za-m
The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit12
```

I used the password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

## Level 12 -> Level 13

```bash
bandit12@bandit:~$ mktemp -d
/tmp/tmp.rPJyL9mOHg
bandit12@bandit:~$ cp data.txt /tmp/tmp.rPJyL9mOHg/
bandit12@bandit:~$ cd /tmp/tmp.rPJyL9mOHg
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv data.txt hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd -r hexd compd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd compd | head -n 1
00000000: 1f8b 0808 0933 9f68 0203 6461 7461 322e  .....3.h..data2.
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv compd compd.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ gzip -d compd.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd compd | head -n 1
00000000: 425a 6839 3141 5926 5359 be9d 9d96 0000  BZh91AY&SY......
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv compd compd.bz2
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ bzip2 -d compd.bz2
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd compd | head -n 1
00000000: 1f8b 0808 0933 9f68 0203 6461 7461 342e  .....3.h..data4.
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv compd compd.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ gzip -d compd.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd compd | head -n 1
00000000: 6461 7461 352e 6269 6e00 0000 0000 0000  data5.bin.......
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv compd compd.tar
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ tar -xf compd.tar
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd.tar  data5.bin  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd data5.bin | head -n 1
00000000: 6461 7461 362e 6269 6e00 0000 0000 0000  data6.bin.......
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ tar -xf data5.bin
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd.tar  data5.bin  data6.bin  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd data6.bin | head -n 1
00000000: 425a 6839 3141 5926 5359 715d fde3 0000  BZh91AY&SYq]....
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ bzip2 -d data6.bin
bzip2: Can't guess original name for data6.bin -- using data6.bin.out
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd.tar  data5.bin  data6.bin.out  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd data6.bin.out | head -n 1
00000000: 6461 7461 382e 6269 6e00 0000 0000 0000  data8.bin.......
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ tar -xf data6.bin.out
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd.tar  data5.bin  data6.bin.out  data8.bin  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd data8.bin | head -n 1
00000000: 1f8b 0808 0933 9f68 0203 6461 7461 392e  .....3.h..data9.
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ mv data8.bin data8.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ gzip -d data8.gz
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ ls
compd.tar  data5.bin  data6.bin.out  data8  hexd
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ xxd data8 | head -n 1
00000000: 5468 6520 7061 7373 776f 7264 2069 7320  The password is
bandit12@bandit:/tmp/tmp.rPJyL9mOHg$ cat data8
The password is FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit13
```

I used the password: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

## Level 13 -> Level 14

```bash
bandit13@bandit:~$ ls
sshkey.private
bandit13@bandit:~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit14 -i sshkey.private
```

## Level 14 -> Level 15

```bash
bandit14@bandit:~$ ls
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
bandit14@bandit:~$ nc localhost 30000
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
Correct!
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit15
```

I used the password: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

## Level 15 -> Level 16 (*)

```bash
bandit15@bandit:~$ openssl s_client -connect localhost:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = SnakeOil
...
---
read R BLOCK
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
Correct!
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

closed
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit16
```

I used the password: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

## Level 16 -> Level 17 (*)

```bash
bandit16@bandit:~$ nmap -sV -T4 -p 31000-32000 localhost
Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-10-01 10:54 UTC
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00025s latency).
Not shown: 996 closed tcp ports (conn-refused)
PORT      STATE SERVICE     VERSION
31046/tcp open  echo
31518/tcp open  ssl/echo
31691/tcp open  echo
31790/tcp open  ssl/unknown
31960/tcp open  echo
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port31790-TCP:V=7.94SVN%T=SSL%I=7%D=10/1%Time=68DD087E%P=x86_64-pc-linu
SF:x-gnu%r(GenericLines,32,"Wrong!\x20Please\x20enter\x20the\x20correct\x2
SF:0current\x20password\.\n")%r(GetRequest,32,"Wrong!\x20Please\x20enter\x
SF:20the\x20correct\x20current\x20password\.\n")%r(HTTPOptions,32,"Wrong!\
SF:x20Please\x20enter\x20the\x20correct\x20current\x20password\.\n")%r(RTS
SF:PRequest,32,"Wrong!\x20Please\x20enter\x20the\x20correct\x20current\x20
SF:password\.\n")%r(Help,32,"Wrong!\x20Please\x20enter\x20the\x20correct\x
SF:20current\x20password\.\n")%r(FourOhFourRequest,32,"Wrong!\x20Please\x2
SF:0enter\x20the\x20correct\x20current\x20password\.\n")%r(LPDString,32,"W
SF:rong!\x20Please\x20enter\x20the\x20correct\x20current\x20password\.\n")
SF:%r(SIPOptions,32,"Wrong!\x20Please\x20enter\x20the\x20correct\x20curren
SF:t\x20password\.\n");

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 141.18 seconds
bandit16@bandit:~$ openssl s_client --connect localhost:31790
...
---
read R BLOCK
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
KEYUPDATE
^C
bandit16@bandit:~$ openssl s_client --connect localhost:31790 -quiet
Can't use SSL_get_servername
depth=0 CN = SnakeOil
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = SnakeOil
verify return:1
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
Correct!
-----BEGIN RSA PRIVATE KEY-----
...
-----END RSA PRIVATE KEY-----
```

Instead of a password we get a RSA key which we use to log in to 17th challange as follows

```bash
bandit16@bandit:~$ mkdir /tmp/bandit0707
bandit16@bandit:~$ cd /tmp/bandit0707
bandit16@bandit:/tmp/bandit0707$ ls
bandit16@bandit:/tmp/bandit0707$ touch key.private
bandit16@bandit:/tmp/bandit0707$ vi key.private
bandit16@bandit:/tmp/bandit0707$ chmod 400 key.private
bandit16@bandit:/tmp/bandit0707$ ssh -i key.private bandit17@localhost -p 2220
```

## Level 17 -> Level 18

```bash
bandit17@bandit:~$ cat /etc/bandit_pass/bandit17
EReVavePLFHtFlFsjn3hyzMlvSuSAcRD
bandit17@bandit:~$ ls
passwords.new  passwords.old
bandit17@bandit:~$ diff passwords.old passwords.new
42c42
< gvE89l3AhAhg3Mi9G2990zGnn42c8v20
---
> x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit18
```

I used the password: x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

But I wasn't able to use the connection it closed and showed Byebye! (this is rel to bandit19)

## Level 18 -> Level 19 (*)

We are not able to login due to the .bashrc file so we just force another shell to start with no rc

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit18 -t "bash -norc"
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit18@bandit.labs.overthewire.org's password:
bash-5.2$ ls
readme
bash-5.2$ cd readme
bash: cd: readme: Not a directory
bash-5.2$ cat readme
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```

Then we just login to level 19

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit19
```

I used the password: cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

## Level 19 -> Level 20

```bash
bandit19@bandit:~$ ls
bandit20-do
bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```

here bandit20-do is a setuid bin

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit20
```

I used the password: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## Level 20 -> Level 21 (*)

SHELL 1
```bash
bandit20@bandit:~$ ls
suconnect
bandit20@bandit:~$ ./suconnect
Usage: ./suconnect <portnumber>
This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.
bandit20@bandit:~$ nmap localhost
Starting Nmap 7.94SVN ( https://nmap.org ) at 2025-10-01 18:09 UTC
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00010s latency).
Not shown: 992 closed tcp ports (conn-refused)
PORT      STATE SERVICE
22/tcp    open  ssh
1111/tcp  open  lmsocialserver
1840/tcp  open  netopia-vo2
4321/tcp  open  rwhois
8000/tcp  open  http-alt
12345/tcp open  netbus
30000/tcp open  ndmps
50001/tcp open  unknown
bandit20@bandit:~$ ./suconnect 12345
Read: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Password matches, sending next password
```

SHELL 2
```bash
bandit20@bandit:~$ nc -lvp 12345
Listening on 0.0.0.0 12345
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Connection received on localhost 44398
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit21
```

I used the password: EeoULMCra2q0dSkYj561DX7s1CpBuOBt

## Level 21 -> Level 22

```bash
bandit21@bandit:~$ ls /etc/cron.d
behemoth4_cleanup  cronjob_bandit22  cronjob_bandit24  leviathan5_cleanup    otw-tmp-dir
clean_tmp          cronjob_bandit23  e2scrub_all       manpage3_resetpw_job  sysstat
bandit21@bandit:~$ cat /etc/cron.d/cronjob_bandit22
@reboot bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
* * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
bandit21@bandit:~$ cat /dev/null
bandit21@bandit:~$ /usr/bin/cronjob_bandit22.sh
chmod: changing permissions of '/tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv': Operation not permitted
/usr/bin/cronjob_bandit22.sh: line 3: /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv: Permission denied
bandit21@bandit:~$ cat /usr/bin/cronjob_bandit22.sh
#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
bandit21@bandit:~$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit22
```

I used the password: tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

## Level 22 -> Level 23

```bash
bandit22@bandit:~$
bandit22@bandit:~$ ls -la /etc/cron.d
total 60
drwxr-xr-x   2 root root  4096 Aug 15 13:19 .
drwxr-xr-x 128 root root 12288 Aug 20 16:10 ..
-r--r-----   1 root root    47 Aug 15 13:16 behemoth4_cleanup
-rw-r--r--   1 root root   123 Aug 15 13:09 clean_tmp
-rw-r--r--   1 root root   120 Aug 15 13:16 cronjob_bandit22
-rw-r--r--   1 root root   122 Aug 15 13:16 cronjob_bandit23
-rw-r--r--   1 root root   120 Aug 15 13:16 cronjob_bandit24
-rw-r--r--   1 root root   201 Apr  8  2024 e2scrub_all
-r--r-----   1 root root    48 Aug 15 13:17 leviathan5_cleanup
-rw-------   1 root root   138 Aug 15 13:17 manpage3_resetpw_job
-rwx------   1 root root    52 Aug 15 13:19 otw-tmp-dir
-rw-r--r--   1 root root   102 Mar 31  2024 .placeholder
-rw-r--r--   1 root root   396 Jan  9  2024 sysstat
bandit22@bandit:~$ cat /etc/cron.d/cronjob_bandit23
@reboot bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null
* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null
bandit22@bandit:~$ cat usr/bin/cronjob_bandit23.sh
cat: usr/bin/cronjob_bandit23.sh: No such file or directory
bandit22@bandit:~$ cat /usr/bin/cronjob_bandit23.sh
#!/bin/bash

myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

cat /etc/bandit_pass/$myname > /tmp/$mytarget
bandit22@bandit:~$ echo $mytarget

bandit22@bandit:~$ echo I am user bandit23 | md5sum | cut -d ' ' -f 1
8ca319486bfbbc3663ea0fbe81326349
bandit22@bandit:~$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit23
```

I used the password: 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

## Level 23 -> Level 24

```bash
bandit23@bandit:~$ cat /etc/cron.d/
behemoth4_cleanup     cronjob_bandit23      leviathan5_cleanup    .placeholder
clean_tmp             cronjob_bandit24      manpage3_resetpw_job  sysstat
cronjob_bandit22      e2scrub_all           otw-tmp-dir
bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24
@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.sh
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname/foo
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" ./$i)"
        if [ "${owner}" = "bandit23" ]; then
            timeout -s 9 60 ./$i
        fi
        rm -f ./$i
    fi
done

bandit23@bandit:~$ ls /var/spool/bandit24/foo
ls: cannot open directory '/var/spool/bandit24/foo': Permission denied
bandit23@bandit:~$ cd /var/spool/bandit24/
bandit23@bandit:/var/spool/bandit24$ ls
foo
bandit23@bandit:/var/spool/bandit24$ cd foo/
bandit23@bandit:/var/spool/bandit24/foo$ ls
ls: cannot open directory '.': Permission denied
bandit23@bandit:/var/spool/bandit24/foo$ ls -la
ls: cannot open directory '.': Permission denied
```

So the cronjob exec all shell scripts in `/var/spool/bandit24/foo` and then deletes them as user `bandit24` hence we can get the password as follows

```bash
bandit23@bandit:/var/spool/bandit24/foo$ mkdir /tmp/pass09
bandit23@bandit:/var/spool/bandit24/foo$ touch /tmp/pass09/pass
bandit23@bandit:/var/spool/bandit24/foo$ chmod 777 /tmp/pass09
bandit23@bandit:/var/spool/bandit24/foo$ cd /tmp/pass09/
bandit23@bandit:/tmp/pass09$ touch pass.sh
bandit23@bandit:/tmp/pass09$ vim pass.sh
bandit23@bandit:/tmp/pass09$ chmod 777 pass.sh
bandit23@bandit:/tmp/pass09$ cp pass.sh /var/spool/bandit24/foo/
bandit23@bandit:/tmp/pass09$ cat pass
bandit23@bandit:/tmp/pass09$ cron
cron: can't open or create /var/run/crond.pid: Permission denied
bandit23@bandit:/tmp/pass09$ cat pass
bandit23@bandit:/tmp/pass09$ chmod 777 pass
bandit23@bandit:/tmp/pass09$ cron
cron: can't open or create /var/run/crond.pid: Permission denied
bandit23@bandit:/tmp/pass09$ cat pass
bandit23@bandit:/tmp/pass09$ cat pass
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
```

pass.sh
```bash
#!/bin/bash

cat /etc/bandit_pass/bandit24 > /tmp/pass09/pass
echo "executed!"
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit24
```

I used the password: gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

## Level 24 -> Level 25

```bash
bandit24@bandit:~$ nc localhost 3002
bandit24@bandit:~$ nc localhost 30002
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 0000
Wrong! Please enter the correct current password and pincode. Try again.
^C
bandit24@bandit:~$ echo "gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 0000" | nc localhost 30002
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
Wrong! Please enter the correct current password and pincode. Try again.
^C
```

So we can create a bash script to generate passcodes

```bash
bandit24@bandit:~$ touch codes.sh
touch: cannot touch 'codes.sh': Permission denied
bandit24@bandit:~$ touch /tmp/codes.sh
bandit24@bandit:~$ vim /tmp/codes.sh
bandit24@bandit:~$ chmod 777 /tmp/codes.sh
```

codes.sh
```bash
#!/bin/bash

pass24=gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

for pin in {0000..9999}; do
        echo "$pass24 $pin"
done | nc localhost 30002
```

and get the pass by running the codes.sh file

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit25
```

I used the password: iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

## Level 25 -> Level 26 (*)

```bash
bandit25@bandit:~$ ls
bandit26.sshkey
bandit25@bandit:~$ ssh -i bandit26.sshkey localhost -l bandit26 -p 2220
...
Connection to localhost closed.
bandit25@bandit:~$ cat /etc/shells
# /etc/shells: valid login shells
/bin/sh
/usr/bin/sh
/bin/bash
/usr/bin/bash
/bin/rbash
/usr/bin/rbash
/usr/bin/dash
/usr/bin/screen
/usr/bin/tmux
/usr/bin/showtext
bandit25@bandit:~$ cat /etc/passwd | grep bandit26
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext
bandit25@bandit:~$ cat /usr/bin/showtext
#!/bin/sh

export TERM=linux

exec more ~/text.txt
exit 0
```

I thought of using `-t` with `ssh` but it didn't work

To break the given shell we could decrease our window size to the point that the text from text.txt doesn't fit in 1vh of our screen so that we can use vim mode execution of more using the keypress `v` and then exec `:e /etc/bandit_pass/bandit26`

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit26
```

I used the password: s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ

still the thing troubling us isn't done troubling us. It still exits so we need to change the shell which we can do using the vim mode execution like this: `:set shell=/bin/bash`

## Level 26 -> Level 27

we just use the new setted shell to get the password as follows from the vim console

```bash
:! ls
bandit27-do  text.txt
:!./bandit27-do cat /etc/bandit_pass/bandit27
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit27
```

I used the password: upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

## Level 27 -> Level 28

```bash
bandit27@bandit:~$ mkdir /tmp/bitf1ip
bandit27@bandit:~$ cd /tmp/bitf1ip
bandit27@bandit:/tmp/bitf1ip$ git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
...
!!! You are trying to log into this SSH server on port 22, which is not intended.
!!! If you are trying to log in to an OverTheWire game, use the port mentioned in
!!! the "SSH Information" on that game's webpage (in the top left corner).
...
bandit27@bandit:/tmp/bitf1ip$ git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
Cloning into 'repo'...
...
Receiving objects: 100% (3/3), done.
bandit27@bandit:/tmp/bitf1ip$ ls
repo
bandit27@bandit:/tmp/bitf1ip$ cd repo/
bandit27@bandit:/tmp/bitf1ip/repo$ ls
README
bandit27@bandit:/tmp/bitf1ip/repo$ cat README
The password to the next level is: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit28
```

I used the password: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

## Level 28 -> Level 29

```bash
bandit28@bandit:~$ mkdir /tmp/bitf1ip
mkdir: cannot create directory ‘/tmp/bitf1ip’: File exists
bandit28@bandit:~$ mkdir /tmp/bitf1ip01
bandit28@bandit:~$ cd /tmp/bitf1ip01
bandit28@bandit:/tmp/bitf1ip01$ git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
Cloning into 'repo'...
...
Resolving deltas: 100% (2/2), done.
bandit28@bandit:/tmp/bitf1ip01$ cd repo/
bandit28@bandit:/tmp/bitf1ip01/repo$ ls
README.md
bandit28@bandit:/tmp/bitf1ip01/repo$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx

bandit28@bandit:/tmp/bitf1ip01/repo$ git log
commit 710c14a2e43cfd97041924403e00efb00b3a956e (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Aug 15 13:16:10 2025 +0000

    fix info leak

commit 68314e012fbaa192abfc9b78ac369c82b75fab8f
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Aug 15 13:16:10 2025 +0000

    add missing data

commit a158f9a82c29a16dcea474458a5ccf692a385cd4
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Aug 15 13:16:10 2025 +0000
    initial commit of README.md
bandit28@bandit:/tmp/bitf1ip01/repo$ git checkout 68314e012fbaa192abfc9b78ac369c82b75fab8f
HEAD is now at 68314e0 add missing data
bandit28@bandit:/tmp/bitf1ip01/repo$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit29
```

I used the password: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7

## Level 29 -> Level 30

```bash
bandit29@bandit:~$ mkdir /tmp/bitf1ip02
bandit29@bandit:~$ cd /tmp/bitf1ip02
bandit29@bandit:/tmp/bitf1ip02$ git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
Cloning into 'repo'...
...
Resolving deltas: 100% (2/2), done.
bandit29@bandit:/tmp/bitf1ip02$ cd repo/
bandit29@bandit:/tmp/bitf1ip02/repo$ ls
README.md
bandit29@bandit:/tmp/bitf1ip02/repo$ cat README.md
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: <no passwords in production!>

bandit29@bandit:/tmp/bitf1ip02/repo$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/dev
  remotes/origin/master
  remotes/origin/sploits-dev
bandit29@bandit:/tmp/bitf1ip02/repo$ git checkout dev
branch 'dev' set up to track 'origin/dev'.
Switched to a new branch 'dev'
bandit29@bandit:/tmp/bitf1ip02/repo$ ls
code  README.md
bandit29@bandit:/tmp/bitf1ip02/repo$ cat README.md
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit30
```

I used the password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

## Level 30 -> Level 31 (!)

```bash
bandit30@bandit:~$ mkdir /tmp/bitf1ip03
bandit30@bandit:~$ cd /tmp/bitf1ip03
bandit30@bandit:/tmp/bitf1ip03$ git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo
Cloning into 'repo'...
...
Receiving objects: 100% (4/4), done.
bandit30@bandit:/tmp/bitf1ip03$ cd repo/
bandit30@bandit:/tmp/bitf1ip03/repo$ ls
README.md
bandit30@bandit:/tmp/bitf1ip03/repo$ cat README.md
just an epmty file... muahaha
bandit30@bandit:/tmp/bitf1ip03/repo$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/master
bandit30@bandit:/tmp/bitf1ip03/repo$ git log
commit de654f201881f820c364f176ffcdea2876431bee (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Aug 15 13:16:14 2025 +0000

    initial commit of README.md
bandit30@bandit:/tmp/bitf1ip03/repo$ ls -la
total 16
drwxrwxr-x 3 bandit30 bandit30 4096 Oct  1 20:49 .
drwxrwxr-x 3 bandit30 bandit30 4096 Oct  1 20:49 ..
drwxrwxr-x 8 bandit30 bandit30 4096 Oct  1 20:49 .git
-rw-rw-r-- 1 bandit30 bandit30   30 Oct  1 20:49 README.md
bandit30@bandit:/tmp/bitf1ip03/repo$ cd .git/
bandit30@bandit:/tmp/bitf1ip03/repo/.git$ ls
branches  config  description  HEAD  hooks  index  info  logs  objects  packed-refs  refs
bandit30@bandit:/tmp/bitf1ip03/repo/.git$ cd ..
bandit30@bandit:/tmp/bitf1ip03/repo$ git tag
secret
bandit30@bandit:/tmp/bitf1ip03/repo$ git show secret
fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit31
```

I used the password: fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy

*note:* I could've also used the command `git log --online --decorate --graph`

## Level 31 -> Level 32

```bash
bandit31@bandit:~$ mkdir /tmp/bitf1ip04 && cd /tmp/bitf1ip04 && git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
Cloning into 'repo'...
...
Receiving objects: 100% (4/4), 382 bytes | 382.00 KiB/s, done.
bandit31@bandit:/tmp/bitf1ip04$ cd repo/ && ls -la
total 20
drwxrwxr-x 3 bandit31 bandit31 4096 Oct  1 21:02 .
drwxrwxr-x 3 bandit31 bandit31 4096 Oct  1 21:02 ..
drwxrwxr-x 8 bandit31 bandit31 4096 Oct  1 21:02 .git
-rw-rw-r-- 1 bandit31 bandit31    6 Oct  1 21:02 .gitignore
-rw-rw-r-- 1 bandit31 bandit31  147 Oct  1 21:02 README.md
bandit31@bandit:/tmp/bitf1ip04/repo$ cat .gitignore
*.txt
bandit31@bandit:/tmp/bitf1ip04/repo$ cat README.md
This time your task is to push a file to the remote repository.

Details:
    File name: key.txt
    Content: 'May I come in?'
    Branch: master

bandit31@bandit:/tmp/bitf1ip04/repo$ touch key.txt
bandit31@bandit:/tmp/bitf1ip04/repo$ vi key.txt
bandit31@bandit:/tmp/bitf1ip04/repo$ vi key.txt
bandit31@bandit:/tmp/bitf1ip04/repo$ rm .gitignore
bandit31@bandit:/tmp/bitf1ip04/repo$ git add key.txt && git commit -m "added key.txt" && git push origin master
[master 431a09f] added key.txt
 1 file changed, 1 insertion(+)
 create mode 100644 key.txt
...
Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: ### Attempting to validate files... ####
remote:
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote:
remote: Well done! Here is the password for the next level:
remote: 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K
remote:
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote:
To ssh://localhost:2220/home/bandit31-git/repo
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://localhost:2220/home/bandit31-git/repo'
```

```bash
~$ ssh -p 2220 bandit.labs.overthewire.org -l bandit32
```

I used the password: 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K

## Level 32 -> Level 33 (*)

```bash
WELCOME TO THE UPPERCASE SHELL
>> $0
$ ls
uppershell
$ export SHELL=/bin/bash
$ $SHELL
bandit33@bandit:~$ ls
uppershell
bandit33@bandit:~$ cat /etc/bandit_pass/bandit33
tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0
```

IMPORTANT: The shell was initially using `bourne shell` (the positional parameter was 1 initially)

```text
______________ ______________ ___________ _______  ________   
\__    ___/   |   \_   _____/ \_   _____/ \      \ \______ \  
  |    | /    ~    \    __)_   |    __)_  /   |   \ |    |  \ 
  |    | \    Y    /        \  |        \/    |    \|    `   \
  |____|  \___|_  /_______  / /_______  /\____|__  /_______  /
                \/        \/          \/         \/        \/ 
```
