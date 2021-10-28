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




