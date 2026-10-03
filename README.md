# oth

## Level 5 → 6

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
millionth       VR1ljMayciFxbnUokuQmJFw6QC9VKtub
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
