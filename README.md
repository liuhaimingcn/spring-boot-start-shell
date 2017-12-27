# springboot-start-shell
用来启动 停止 springboot应用的脚本

## start 启动应用

* start 后面可以跟相对路径和绝对路径, 最后的文件名来作为AppName

``` sh
➜ ./sbm.sh start /Users/liuhaiming/nlp-user/target/nlpUser.jar
check running status...

App is NOT running.
start...
check running status...
App is running.
Start success!
```

## check 检查应用的状态

``` sh
➜ ./sbm.sh check nlpUser
check running status...
App is running.
➜ ./sbm.sh check nlp
check running status...
App is NOT running.
```

## stop 停止应用

``` sh
➜ ./sbm.sh stop nlpUser
Stop Process...
Stop Success!
➜ ./sbm.sh stop nlp
App already stop!
```

## list 列出所有运行中的应用

``` sh
➜ ./sbm.sh list all
80569 java nlpUser
➜ ./sbm.sh list nlpUser
80569 java nlpUser
➜ ./sbm.sh list nlp

```
