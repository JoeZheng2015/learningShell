# 两种运行 Shell 脚本的方法

1. 作为可执行程序
``` bash
# 是脚本具有执行权限
chmod +x ./index.sh
# 执行脚本
./index.sh
```
注意，一定要指定文件的目录，如在当前目录 `./index.sh` 或上一级目录 `./hello_world/index.sh` 都可以，但 `index.sh` 则不行。因为不像 `ls, cs` 等， index.sh 是不在系统 PATH 里的！

2. 作为解释器参数
``` bash
/bin/sh index.sh
/bin/php index.php
```

扩展：
同理，主要指定 Node 为解释器，则可增加 js 脚本
``` bash
./index.js
```
