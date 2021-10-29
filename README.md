# OWASP Juice Shop

## Task 4 Who broke my lock?!
Question #1: Bruteforce the Administrator account's password!
- Sem sel  na login page in vpisal admin@juice-sh.op in a kot geslo, prav tako pa sem intercept dal na on in stisnil na login.
- Nato sem request dal Intruderju in dal kot je v navodilih datoteko z gesli in pricel napad.
- Nato sem cakal da se konca (401 je error 200 je OK).
- Dobil geslo admin123 
- Flag: c2110d06dc6f81c67cd8099ff0ba601241f1ac0e

Question #2: Reset Jim's password!
- Kot po navodilih sem sel v Forget password in izpolnil ime za Jim.
- Nato sem tako kot je pisalo sel googlat Jim Star Trek in videl ime Samuel.
- Nato pa izpolnil vse.
- Flag: 094fbc9b48e525150ba97d05b942bbf114987257

## Task 5 AH! Don't look! 
Question #1: Access the Confidential Document!
- Sem sel na link tako kot pise in downloadal file
- Flag :edf9281222395a1c5fee9b89e32175f1ccf50c5b

Question #2: Log into MC SafeSearch's account!
- Se vpisal
- Flag: 66bdcffad9e698fd534003fbb3cc7e2b7b55d7f0

Question #3: Download the Backup file!
- wget http://10.10.246.8/ftp/package.json.bak%2500.md 
- Flag: bfc1e6b4a16579e85e06fee4c36ff8c02fb13795

## Task 6 Who's flying this thing? 
Question #1: Access the administration page!
- Najprej sem odprl Sources
- Refresh page in odprl main-es.js
- Poiskal admin in nasel tako kot v navodilih
- Se vpisal v admina in sel na stran
- Flag: 946a799363226a24822008503f5d1324536629a0

Question #2: View another user's shopping basket!
- Po navodilih kot admin pogledal kosarico
- Spremenil v Burp na id 2
- Flag: 41b997a36cc33fbe4f0ba018474e19ae5ce52121

Question #3: Remove all 5-star reviews!
- Sel na administration page in zbrisal 5 star 
- Flag: 50c97bcce0b895e446d61c83a21df371ac2266ef

## Task 7 Where did that come from? 
Question #1: Perform a DOM XSS!
- V search bar sem napisal: < iframe src="javascript:alert(`xss`)" > 
- Flag: 9aaf4bbea5c30d00a1f5bbcfce4db6d4b0efe0bf

Question #2: Perform a persistent XSS!
- Sledil navodilam
- Flag: 149aa8ce13d7a4a8a931472308e269c94dc5f156

Question #3: Perform a reflected XSS!
- V id v url kopiral < iframe src="javascript:alert(`xss`)" >
- Flag: 23cefee1527bde039295b2616eeb29e1edc660a0

## Task 8 Exploration! 
- Naredil in si pogledal dodatne izzive.



Use the bonus payload < iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/771984076&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe> in the DOM XSS challenge.
- Flag: 26bdee65430d102cf5f1d41046c2ff22c95811d3

You successfully solved a challenge: Zero Stars (Give a devastating zero-star feedback to the store.)
- Dal feedback toda v Burpu spremenil rating na 0.
- Flag: 88b7c1d1349d618f7f0e25563295543559d98d4f
