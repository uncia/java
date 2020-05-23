# java

## wget:
```
wget -N --no-check-certificate https://github.com/uncia/java/releases/download/jre-8u251/jre-8u251-linux-x64.rpm && rpm -ivh jre-*-linux-*.rpm --force --nodeps
```

```
wget -N --no-check-certificate https://github.com/uncia/java/releases/download/jdk-8u251/jdk-8u251-linux-x64.rpm && rpm -ivh jdk-*-linux-*.rpm --force --nodeps
```

修改profile文件
追加脚本如下：
```
vim /etc/profile
```

```
export JAVA_HOME=/usr/java/jdk1.8.0_251
export PATH=$PATH:$JAVA_HOME/bin:$JAVA_HOME/jre/bin
export CLASSPATH=$JAVA_HOME/lib:$JAVA_HOME/lib/tools.jar
```
保存退出，使其生效：

```
source /etc/profile
java -version
```

jre:
```
jre-8u251-linux-i586.rpm
jre-8u251-linux-i586.tar.gz
jre-8u251-linux-x64.rpm
jre-8u251-linux-x64.tar.gz
jre-8u251-macosx-x64.dmg
jre-8u251-macosx-x64.tar.gz
jre-8u251-windows-i586.exe
jre-8u251-windows-i586.tar.gz
jre-8u251-windows-x64.exe
jre-8u251-windows-x64.tar.gz
```
jdk:
```
jdk-8u251-linux-i586.rpm
jdk-8u251-linux-i586.tar.gz
jdk-8u251-linux-x64.rpm
jdk-8u251-linux-x64.tar.gz
jdk-8u251-macosx-x64.dmg
jdk-8u251-windows-i586.exe
jdk-8u251-windows-x64.exe
```
