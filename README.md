# oth

## Level 0

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
# use bandit0 as a password as well
```

```text
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
```

## Level 0 → 1

```bash
cat readme
```

```text
6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
```

## Level 1 → 2

```bash
cat ./-
```

```text
PK8fYLZg2hnHSz83plBL1iEPKdD3QToB
```

## Level 2 → 3

```bash
cat  ./--spaces\ in\ this\ filename--
```

```text
7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
```

## Level 3 → 4

```bash
cd inhere/
ls -all
cat ...Hiding-From-You
```

```text
xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq
```

## Level 4 → 5

```bash
cd inhere/
file ./*
cat ./-file07
```

```text
6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG
```

## Level 5 → 6

```bash
find . -size 1033c -readable ! -executable
cat ./inhere/maybehere07/.file2
```

```text
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
```

## Level 6 → 7

```bash
find . -type f -size 33c -user bandit7 -group bandit6
```

```text
Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3
```

## Level 7 → 8

```bash
cat data.txt | grep millionth
```

```text
VR1ljMayciFxbnUokuQmJFw6QC9VKtub
```

> A | jelet pipe-nak hívják. Úgy működik, mint egy cső két parancs között: az első parancs kimenetét közvetlenül a második parancs bemenetébe vezeti, ahelyett hogy kiírná a képernyőre.
> Altgr + w

## Level 8 → 9

```bash
sort data.txt | uniq -u
```

```text
EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl
```

## Level 9 → 10

```bash
strings data.txt | grep ====
```

```text
B0s2khmbT9u0geKuOoVGW3JZKhndE3BG
```

## Level 10 → 11

```bash
base64 -d data.txt
```

```text
pYfOY6HwUsDj5rL9UvyhU7MCmv8vN5Ro
```

## Level 11 → 12

```bash
cat data.txt | tr "A-Za-z" "N-ZA-Mn-za-m"
```

```text
GROozWPO8QyN0mGrjUkID0WCYkZiQxrN
```

## Level 12 → 13

```bash
xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | cat
```

```text
       -x, --extract, --get
              Extract files from an archive.  Arguments are optional.
              When given, they specify names of the archive members to be
              extracted.
       -O, --to-stdout
              Extract files to standard output.
```

```text
qQYQiHOBPR8zR61qxYqX45quvihF2uzk
```

## Level 13 → 14

```bash
scp -P 2220 bandit13@bandit.labs.overthewire.org:/home/bandit13/sshkey.private .
chmod 700 ./sshkey.private
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit14
```

```text
aaWecNkG4FhxJQxz07uiwzVP6bJiYS65
```

## Level 14 → 15

```bash
nc localhost 30000
```

```text
pbLYuZtTg4MgaqfJx8jbA9gKKGqM68A7
```

## Level 15 → 16

```text
     s_client      This  implements  a  generic  SSL/TLS client which can establish a transparent connection to a remote server speaking SSL/TLS. It's intended for testing purposes only and provides only rudimentary interface functionality but internally uses mostly all functionality of the
           OpenSSL ssl library.
```

```bash
openssl s_client localhost:30001
```

```text
kS0Hf0u5HiXFwKMKFqXvPdOTNGGa0X8V
```

## Level 16 → 17

```text
 SERVICE/VERSION DETECTION:
           -sV: Probe open ports to determine service/version info

```

```bash
nmap -p 31000-32000 localhost
cat /etc/bandit_pass/bandit16 | openssl s_client  -connect localhost:31790 -quiet
```

```text
-----BEGIN OPENSSH PRIVATE KEY-----
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
-----END OPENSSH PRIVATE KEY-----
```

## Level 17 → 18

```bash
diff passwords.new passwords.old
```

```text
OQxXZjELndr90zuhOTDYBEomI0SZITXI
```

## Level 18 → 19

```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme
```

```text
KpsOfPkcP7i1FlIExk2QEjyt6dw8dxZI
```

## Level 19 → 20

```bash
./bandit20-do cat /etc/bandit_pass/bandit20
```

```text
4pIjcunZ0fK2vmp3IwfG8Vf7VhxD6pOA
```
## Level 20 → 21

```text
       -n     do not output the trailing newline

       -l      Listen for an incoming connection rather than initiating a connection to a remote host.
       -p source_port       Specify the source port nc should use, subject to privilege restrictions and availability.
       & sends it to the background
```


```bash
echo -n '4pIjcunZ0fK2vmp3IwfG8Vf7VhxD6pOA' | nc -l -p 1234 &
./suconnect 1234
```

```text
bW9kBv5WC3P4yoDyf12LSdGuNz5ka6hY
```

## Level 21 → 22

```bash
cat /etc/cron.d/cronjob_bandit22
cat  /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```

```text
RYVux2rHEm9tiXHmLFzuR7Vhx6AZQMEz
```

## Level 22 → 23

```bash
cat /etc/cron.d/cronjob_bandit23
cat  /usr/bin/cronjob_bandit23.sh
echo I am user bandit23 | md5sum | cut -d ' ' -f 1
cat /tmp/8ca319486bfbbc3663ea0fbe81326349
```

```text
gKXDTAXnIz3OBxiPjRZ2uqutUlPZrBsw
```

## Level 23 → 24

```bash
cat /etc/cron.d/cronjob_bandit24

cat /usr/bin/cronjob_bandit24.sh

mktemp -d

chmod 777 /tmp/tmp.NJjseRy9cK

job.sh

#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/tmp.NJjseRy9cK/result

chmod 755 /tmp/tmp.NJjseRy9cK/job.sh
cp /tmp/tmp.NJjseRy9cK/job.sh /var/spool/bandit24/foo/job.sh

sleep 65

cat /tmp/tmp.NJjseRy9cK/result

```

```text
hVQMk3lJNsmQ7VF3ubyrNNBom7BOgVXv
```

## Level 24 → 25

```text
       -v, --invert-match
              Invert the sense of matching, to select non-matching lines.

```


```bash
nc localhost 30002

#!/bin/bash

for i in {0000..9999};
do
	echo "hVQMk3lJNsmQ7VF3ubyrNNBom7BOgVXv $i"
done | nc localhost 30002 | grep -v Wrong
```

```text
SoHfqMOEqIX2IYKVciZxvgpR9a2Djx4P
```

## Level 25 → 26


```bash
yk just a priv key
```

```text
26: jHdv2ELQhT22BkprMNDjybZDAkw1zeBJ
```


## Level 26 → 27

```text

v visual mode
```

```bash
small terminal
v to visual mode
:set shell=/bin/bash
:shell
cat /etc/bandit_pass/bandit26
./bandit27-do cat /etc/bandit_pass/bandit27
```

```text
27: STJLJBRRphMxKB392CT4iOr5CbzPU9ER
```

## Level 27 → 28

```bash
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
cd repo/
cat README
```

```text
y8Yd2ssKcpHpud7UvOSOxwamRMzIGIeQ
```

## Level 28 → 29

```bash
git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo
cd repo/
git log
git checkout df10da19c2625f7c59e071e16030bd587d8c409d
cat README.md
```

```text
Em7eGtqaMySwNFjCpwzzHhLhospOcdt0
```

## Level 29 → 30

```bash
git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo
cd repo/
git branch -r
git checkout origin/dev
cat README.md
```

```text
jq9Dfg2rXsfYsWMgFuKlXhphjdH7USgX
```

## Level 30 → 31

```bash
git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo
cd repo/
git tag
git show secret
```

```text
82NkymblpGBYmIXG6ZQ8YldBYstHpfUf
```

## Level 31 → 32

```bash
git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo
cd repo/
ls -all
cat README.md
cat .gitignore
echo "May I come in?" > key.txt
git add key.txt -f
git commit -m "asd"
```

```text
pWuj5jBQ6IgV0NXwiH6g1pXRF8S1YvbT
```

## Level 32 → 33

```text
A little bit of Theory
Linux has Variables called local variables (valid in current shell), shell variables (set up by shell) and environment variables (valid systemwide). These variables have their names in uppercase only. They are defined by writing VAR_NAME=var_value in the command line. To see the content of a variable, you can write echo $VAR_NAME.

To print all environment variables, you can use printenv.

Some common that are good to know are:

TERM -  current terminal emulation
HOME - the path to home directory of currently logged in user
LANG - current locales settings
PATH - directory list to be searched when executing commands
PWD - pathname of the current working directory
SHELL/0 - the path of the current user’s shell
USER - currently logged-in user
```


```bash
$0
bash
cat /etc/bandit_pass/bandit33
```

```text
u4P2CyPOwPGLe94RdD9Uo2FxFwvnFswM
```
