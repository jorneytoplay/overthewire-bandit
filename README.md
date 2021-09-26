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



