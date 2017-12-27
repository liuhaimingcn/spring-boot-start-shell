# springboot-start-shell
用来启动 停止 springboot应用的脚本

## start 启动应用

* start 后面可以跟相对路径和绝对路径, 最后的文件名来作为AppName

``` sh
➜  springboot-start-shell git:(master) ./pms.sh start /Users/liuhaiming/Documents/workspace/raventech/code/nlp/nlp-user/target/nlpUser.jar
check running status...

App is NOT running.
start...
check running status...
App is running.
Start success!
```

## check 检查应用的状态

``` sh
➜  springboot-start-shell git:(master) ./pms.sh check nlpUser
check running status...
App is running.
➜  springboot-start-shell git:(master) ✗ ./pms.sh check nlp
check running status...
App is NOT running.
```

## stop 停止应用

``` sh
➜  springboot-start-shell git:(master) ✗ ./pms.sh stop nlpUser
Stop Process...
Stop Success!
➜  springboot-start-shell git:(master) ✗ ./pms.sh stop nlp
App already stop!
```

## list 列出所有运行中的应用

``` sh
➜  springboot-start-shell git:(master) ✗ ./pms.sh list all
80569 java nlpUser
➜  springboot-start-shell git:(master) ✗ ./pms.sh list nlpUser
80569 java nlpUser
➜  springboot-start-shell git:(master) ✗ ./pms.sh list nlp

```
