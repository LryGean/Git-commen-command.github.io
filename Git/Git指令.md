网页查看代码将`github.com`改成`github1s.com`

初始化（管理文件夹）：`git init`

检测当前文件夹下文件状态：`git status`

管理文件：`git add .（全部文件）`or `git add （某个文件）`

生成版本：`git commit -m 'v1'(注释或版本号)`

查看版本信息：`git log`

推送：`git push`
注意：若出现`fatal: unable to access 'https://github.com/.......': OpenSSL SSL_read: Connection was reset, errno 10054`
解除ssl验证后，再次git即可 命令：`git config --global http.sslVerify "false"`


******
`git config --global --unset http.proxy`
`git config --global --unset https.proxy`

问题：
1.`Failed to connect to github.com port 443: Timed out`
解决：`git config --global --unset http.proxy`

2.`warning: LF will be replaced by CRLF in demo/demo.py.
         The file will have its original line endings in your working directory`
解决：`git config --global core.autocrlf true`
3.`OpenSSL SSL_read: Connection was reset, errno 10054`
解决：`git config --global http.sslVerify "false"`




*******

scrcpy
手机端：
①usb调试
②ADB调试
PC端
cmd:
adb usb
连接：
1.scrcpy
2.   
+ adb devices (获取手机序列号)
+ scrcpy -m 1920 -s 46FDU19614004369	 