bandit0: 
	mdp :bandit0 
	cmd :ls 
	     cat readme
bandit1: 
	mdp :NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL 
	cmd :ls 
	     cat ./-
bandit2: 
	mdp :rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi 
	cmd :ls 
	     cat "spaces in this filename"
bandit3: 
	mdp :aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG 
	cmd :ls 
	     cd inhere 
	     ls -a 
	     cat .hidden 
bandit4: 
	mdp :2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe 
	cmd :ls 
  	     cd inhere 
             ls 
             cat ./-file07
bandit5: 
	mdp :lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR 
	cmd :ls 
             cd inhere 
	     ls 
             cat ./maybehere07/.file2
bandit6: 
	mdp :P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU 
	cmd :ls 
             find / -size 33c -user bandit7 -group bandit6 -type f 
             cat /var/lib/dpkg/info/bandit7.password
bandit7: 
	mdp :z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S 
	cmd :ls 
             cat data.txt | grep millionth
bandit8: 
	mdp :TESKZC0XvTetK0S9xNwm25STk5iWrBvP 
	cmd :ls 
             cat data.txt | sort | uniq -u
bandit9: 
	mdp :EN632PlfYiZbn3PhVK3XOGSlNInNE00t 
	cmd :ls 
             strings data.txt | grep ==
bandit10: 
	mdp :G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s 
	cmd :ls 
             cat data.txt | base64 -d
bandit11: 
	mdp :6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM 
	cmd :ls 
             cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
bandit12: 
	mdp :JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
	cmd :xxd -r data.txt data1
	     mv data1 data2.gz
             gzip -d data2.gz
             mv data2 data3.bz2
             bzip2 -d data3.bz2
             mv data3 data4.gz
             gzip -d data4.gz
             tar -xvf data4
             tar -xvf data5.bin
             mv data6.bin data7.bz2
             bzip2 -d data7.bz2
             tar -xvf data7
             mv data8.bin data9.gz
             gzip -d data9.gz
             cat data9
bandit13: 
	mdp :wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw 
	cmd :ls 
             ssh -i sshkey.private bandit14@localhost -p 2220
bandit14: 
	cmd : cd /etc/bandit_pass/ , cat bandit1 ,cat bandit14 ,echo fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq | nc localhost 30000
bandit15: 
	mdp :jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt 
	cmd :cat /etc/bandit_pass/bandit15 
             openssl s_client -connect localhost:30001
bandit16: 
	mdp :JQttfApK4SeyHwDlI9SXGR50qclOAil1
	cmd : ssh -T bandit18@bandit.labs.overthewire.org -p 2220
bandit17: 
	mdp :VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e
	cmd : diff passwords.new passwords.old
bandit18: 
	mdp :hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
	     glZreTEH1V3cGKL6g4conYqZqaEj0mte
	cmd :ssh -T bandit18@bandit.labs.overthewire.org -p 2220 
bandit19:
	mdp :awhqfNnAbc1naukrpqDYcF95h7HoMTrC
	cmd :ssh -T bandit18@bandit.labs.overthewire.org -p 2220 
bandit20: 
	mdp :VxCazJaVykI6W36BkBU0mJTCM8rR95XT 
	cmd : ssh bandit20@bandit.labs.overthewire.org -p 2220
	      ./bandit20-do cat /etc/bandit_pass/bandit20
