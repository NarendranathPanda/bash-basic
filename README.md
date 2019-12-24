# bash-basic
# 1 How to check the Exit code of previous command

```shell
echo "Hello Wolrd"
echo $?
```
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

# Bash file 

```shell

vi test.sh
```
```shell
#!/bin/bash
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
sh test.sh
```
bash-basics
