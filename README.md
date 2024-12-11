# Fuzzing
1. ffuf tool
     - -u + (site)/FUZZ -w wordlist for subdomains : seclist DNS / for directories : seclist webcontent
     - ffuf -u site.com/FUZZ/ABBDALLA -w file1.txt:FUZZ -w file2.txt:ABDALLA
     - for adding header -H "x-Forwarded-For : 127.0.0.1"
     - FFUF -u site.com?Fuzz=1 -w word list
2. dirsearch -u site -x 403 (exclude 403)  -i 200 (only 200 )
    - --full-url  (for full url )
    - dirsearch -l $(pwd)/file.txt -i 200
