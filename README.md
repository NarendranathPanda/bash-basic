# bash-basic
# 1 How to check the Exit code of previous command

```shell
echo "Hello Wolrd"
echo $?
```
*Return code 0 means sucessful any other number means the previous command didn't execute properly* 

# 2  Join Two command || -or , && and

```shell
echo "Good Morning" || echo "Good Night"
echo $?
```

```shell
echo sh test.sh || sh cleanup.sh
echo $?
```

```shell
sh test.sh && git push
echo $?
```

# 3 Bash file 

```shell

vi test.sh
```
```shell
#!/bin/bash

# -e is for exit on error  +e is for continue even if error is there
set -e 

function_run_junit_test(){
return 0;
}

function_run_integration_test(){
return 0;
}

function_run_e2e_test(){
return 0;
}

function_run_junit_test
function_run_integration_test
function_run_e2e_test

```
```shell
chmod +x test.sh
sh test.sh
```
# 4 Get Stream output  $(---)
```shell
function_get_version(){
echo "1.2.4"
}

echo "The version of the software is $(function_get_version)"





bash-basics
