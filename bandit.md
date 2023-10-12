# Level 0

`ssh bandit0@bandit.labs.overthewire.org -p 2220`, password: `bandit0`

```
cat readme
```

# Level 1

`ssh bandit1@bandit.labs.overthewire.org -p 2220`

```
cat < -
```

# Level 2

`ssh bandit2@bandit.labs.overthewire.org -p 2220`

```
cat spaces\ in\ this\ filename
```

# Level 3

`ssh bandit3@bandit.labs.overthewire.org -p 2220`

```
cat inhere/.hidden
```

# Level 4

`ssh bandit4@bandit.labs.overthewire.org -p 2220`

```
cat < inhere/-file00
cat < inhere/-file01
cat < inhere/-file02
cat < inhere/-file03
cat < inhere/-file04
cat < inhere/-file05
cat < inhere/-file06
cat < inhere/-file07
cat < inhere/-file08
cat < inhere/-file09
```

# Level 5

`ssh bandit5@bandit.labs.overthewire.org -p 2220`

```
cd inhere
find ./ -size 1033c
cat ./maybehere07/.file2
```

# Level 6

`ssh bandit6@bandit.labs.overthewire.org -p 2220`

```
find / -size 33c /user bandit7
cat /var/lib/dpkg/info/bandit7.password
```

# Level 7

`ssh bandit7@bandit.labs.overthewire.org -p 2220`

```
grep millionth data.txt
```

# Level 8

`ssh bandit8@bandit.labs.overthewire.org -p 2220`

```
sort data.txt | uniq -c | grep "1 "
```

# Level 9

`ssh bandit9@bandit.labs.overthewire.org -p 2220`

```
grep -a === data.txt
```

# Level 10

`ssh bandit10@bandit.labs.overthewire.org -p 2220`

```
base64 -d data.txt
```

# Level 11

`ssh bandit11@bandit.labs.overthewire.org -p 2220`

```
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

# Level 12

`ssh bandit12@bandit.labs.overthewire.org -p 2220`

```
mktemp -d
cp data.txt /temp/temp.XXX
cd /temp/temp.XXX

xxd -r data.txt > tmp

file tmp
mv tmp tmp.gz
gunzip tmp.gz

file tmp
mv tmp tmp.bz2 
bzip2 -d tmp.bz2

file tmp
mv tmp tmp.gz
gunzip tmp.gz

file tmp
tar -xvf tmp
tar -xvf data5.bin

file data6.bin
mv data6.bin data6.bz2
bzip2 data6.bz2

file data6
tar -xvf data6

file data8.bin
mv data8.bin data8.gz
gunzip data8.gz

cat data8
```










































