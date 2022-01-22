we can write top of the bash script by 
- #!/bin/bash (works for 90 percent of systems)
- #!/usr/bin/env bash (in some systems may be this works)
***
we can run bash scripts by 4 ways :
- ./app.sh
- /bin/bash app.sh
- bash app.sh
- sh app.sh
***
read => works like input 

```bash script
#!bin/bash
echo "Who are you dude?"
read name
echo "Hello $name"
```

```bash script
#!/bin/bash
echo "What is you linux distro name ?"
read distro
echo "oh dude , ${distro} is one of the best distros"
```

if condition in bash script
```bash script
 1 #!/bin/bash  
 2 echo Enter your integer  
 3 read v1  
 4 read v2  
 5 if [[ $v1 > $v2 ]]; then  
 6 		echo good , keep moving  
 7 elif [[ $v2 > $v2 ]]; then  
 8		 echo not bad , we can accepted that  
 9 else  
10 		 echo  go out  
11 fi
```

we can execute 2 condition or more in bash script by adding && between them and  we can accept to execute the condition just with one condition  (disjunctive composition) by adding ||  
```
if [[condition 1 && condition 2]]
if [[condition 1 || condition 2]]
```

Its better to use -gt and -lt instead of > < in bash script  and -eq instead of equal, there is a better list :)
- -eq # Equal
- -ne # Not equal
- -lt # Less than
- -le # Less than or equal
- -gt # Greater than
- -ge # Greater than or equal

actually in newer bash,  you can use (()) instead of [[]] and in this way you can use > <  easily.

```bash script
 1 #!/bin/bash  
 2 read n1  
 3 if (( n1 > 1000 )); then  
 4 		echo "ok , i understand that bro"  
 5 elif (( n1 < 800 )); then  
 6 		echo "fuck you"  
 7 fi

```

```bash script
arr{a,b,c,d,e}
for i in "${arr[@]}";do
		echo $i
```
‍‍‍‍

### bash is extremly case sensetive. 
***
