# overthewire-bandit
Answers to bandit questions:

0.ekrem@ekremHP:~$ ssh bandit0@bandit.labs.overthewire.org -p 2220
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit0@bandit.labs.overthewire.org's password: 
Linux bandit.otw.local 5.4.8 x86_64 GNU/Linux

1.cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1

2.bandit1@bandit:~$ cat ./-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

3.bandit2@bandit:~$ cat "spaces in this filename"
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

4.bandit3@bandit:~/inhere$ ls -a
.  ..  .hidden
bandit3@bandit:~/inhere$ cat ".hidden"
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

5.bandit4@bandit:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh

6.bandit5@bandit:~$ find -size 1033c
./inhere/maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

7.bandit6@bandit:/$ find -user bandit7 -group bandit6 -size 33c
bandit6@bandit:/$ cd ./var/lib/dpkg/info/
bandit6@bandit:/var/lib/dpkg/info$ cat bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

8.bandit7@bandit:~$ grep millionth data.txt
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV

9.bandit8@bandit:~$ sort data.txt | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
