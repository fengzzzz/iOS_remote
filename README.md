#ios_remote
#启动步骤：
#1，搭建好wda真机运行环境、mvn、java、ios-minicap、libimobiledevice（使用它的iproxy命令）
#2，在命令行运行iproxy 8200 8100 （这里的8200跟/src/main/resources/config.properties中的wdaPort应该一致）
#3，修改/src/main/resources/config.properties配置文件，修改minicapPath，bashPath，wdaPort，minicapPort成本地你的路径
#4, 修改/src/main/resources/execWDA.sh，更改里面的xcodebuild命令的project为你本地的wda路径。
#5，在项目目录下运行命令：mvn tomcat7:run-war,默认监听本机8080端口。
#6，打开浏览器，访问 http://localhost:8080/ios/
