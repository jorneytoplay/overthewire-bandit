# overthewire-bandit
Answers to bandit questions:

<details>
  <summary>
    Start
  </summary>
  ekrem@ekremHP:~$ ssh bandit0@bandit.labs.overthewire.org -p 2220
  </details>
  
  <details>
  <summary>
    Level 0 → Level 1
  </summary>
  cat readme   
  <br>boJ9jbbUNNfktd78OOpsqOltutMc3MY1</br>
</details>

 <details>
  <summary>
    Level 1 → Level 2
  </summary>
  bandit1@bandit:~$ cat ./-
<br>CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9</br>
  </details>
  
   <details>
  <summary>
    Level 2 → Level 3
  </summary>
  bandit2@bandit:~$ cat "spaces in this filename"
<br>UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK</br>

  </details>
  
   <details>
  <summary>
    Level 3 → Level 4
  </summary>
  bandit3@bandit:~/inhere$ ls -a
<br>bandit3@bandit:~/inhere$ cat ".hidden"</br>
<br>pIwrPrtPN36QITSp3EQaw936yaFoFgAB</br>
  </details>
  
   <details>
  <summary>
    Level 4 → Level 5
  </summary>
  bandit4@bandit:~/inhere$ cat ./-file07
<br>koReBOKuIDDepwhWk7jZC0RTdopnAYKh</br>
  </details>
  
   <details>
  <summary>
    Level 5 → Level 6
  </summary>
  bandit5@bandit:~$ find -size 1033c
<br>./inhere/maybehere07/.file2</br>
<br>DXjZPULLxYr17uwoI01bNLQbtFemEgo7</br>
  </details>

  <details>
  <summary>
    Level 6 → Level 7
  </summary>
  bandit6@bandit:/$ find -user bandit7 -group bandit6 -size 33c
<br>bandit6@bandit:/$ cd ./var/lib/dpkg/info/</br>
<br>bandit6@bandit:/var/lib/dpkg/info$ cat bandit7.password</br>
<br>HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs</br>
  </details>
  
  <details>  
  <summary>
    Level 7 → Level 8
  </summary>
  bandit7@bandit:~$ grep millionth data.txt
  <br> millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV</br>
  </details>
  
  <details>  
  <summary>
    Level 8 → Level 9
  </summary>
  bandit8@bandit:~$ sort data.txt | uniq -u
<br>UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR</br>
  </details>

<details>  
  <summary>
    Level 9 → Level 10
  </summary>
  strings data.txt | grep -E "=="
========== the*2i"4
========== password
Z)========== is
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
  <br>truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk</br>
  </details>
  
  
<details>  
  <summary>
    Level 10 → Level 11
  </summary>
  bandit10@bandit:~$ base64 --decode data.txt
  <br>The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR</br>
  </details>

<details>  
  <summary>
    Level 11 → Level 12
  </summary>
  bandit11@bandit:~$  cat data.txt |tr'[a-z]''[n-za-m]'|tr'[A-Z]''[N-ZA-M]'
  <br>The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu</br>
  </details>
  
  <details>  
  <summary>
    Level 12 → Level 13
  </summary>
  <br>mkdir /tmp/mynam</br>
  <br>cp data.txt /tmp/mynam</br>
  <br><xxd -r data.txt pass1</br>
  <br>mv pass1 pass1.gz</br>
  <br>gzip -d pass1.gz</br>
  <br>bzip2 -d pass1</br>
  <br>zcat pass1.out>pass2</br>
  <br>tar -xvf pass2</br>
  <br>tar -xvf data5.bin</br>
  <br>bzip2 -d data6.bin</br>
  <br>tar -xvf data6.bin.out</br>
  <br>zcat data8.bin>pass3</br>
  <br>cat pass3</br>
  <br>The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL</br>
  </details>
  
  <details>  
  <summary>
    Level 13 → Level 14
  </summary>
  <br>cat sshkey.private</br>
  <br>ssh bandit14@localhost -i sshkey.private</br>
  <br>cd /etc/bandit_pass</br>
  <br>cat bandit14</br>
  <br>4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e</br>
  </details>


  <details>  
  <summary>
    Level 14 → Level 15
  </summary>
  <br>nc localhost 30000 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e</br>
  <br>Correct! BfMYroe26WYalil77FoDi9qh59eK5xNr</br>
  </details>
  
  
  <details>  
  <summary>
    Level 15 → Level 16
  </summary>
  <br>openssl s_client -connect localhost:30001</br>
  <br>BfMYroe26WYalil77FoDi9qh59eK5xNr</br>
  <br>Correct! cluFn7wTiGryunymYOu4RcffSxQluehd</br>
  </details>

 <details>  
  <summary>
    Level 16 → Level 17
  </summary>
  <br>nmap -p 31000-32000 localhost</br>
  <br>openssl s_client -connect localhost:31790 -quiet > pass17 </br>
  <br>chmod 700 pass17</br>
  <br>ssh bandit17@localhost -i pass17</br>
  </details>
  
  <details>  
  <summary>
    Level 17 → Level 18
  </summary>
  <br>diff passwords.new passwords.old</br>
  <br>kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd</br>>
  </details>
  
  <details>  
  <summary>
    Level 18 → Level 19
  </summary>
  <br>ssh bandit18@bandit.labs.overthewire.org -p 2220</br>
  <br>cat ~/readme</br>
  <br>IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x</br>
  </details>
  
  <details>  
  <summary>
    Level 19 → Level 20
  </summary>
  <br>ssh bandit19@bandit.labs.overthewire.org -p 2220</br>
  <br>./bandit20-do</br>
  <br>./bandit20-do id</br>
  <br>./bandit20-do cat /etc/bandit_pass/bandit20</br>
  </details>
  
  <details>  
  <summary>
    Level 20 → Level 21
  </summary>
  <br>echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -l localhost -p 10000</br>
  <br>./suconnect 10000</br>
  <br>gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr</br>
  </details>
  
  <details>  
  <summary>
    Level 21 → Level 22
  </summary>
  <br>ssh bandit19@bandit.labs.overthewire.org -p 2220</br>
  <br>./bandit20-do</br>
  <br>./bandit20-do id</br>
  <br>./bandit20-do cat /etc/bandit_pass/bandit20</br>
  </details>
  
  <details>  
  <summary>
    Level 22 → Level 23
  </summary>
  <br>cd /etc/cron.d</br>
  <br>cat /etc/cron.d/cronjob_bandit22</br>
  <br> cat /usr/bin/cronjob_bandit22.sh</br>
  <br>cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv</br>
  <br>Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI</br>
  </details>


