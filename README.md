# -
安卓简单反编译

下载如下工具：<br>
 apktool <br>
 dex2jar <br>
 jd-gui  <br>
 
解压apktool，得到3个文件：aapt.exe,apktool.bat,apktool.jar,将须要反编译的APK文件放到该文件夹下，<br>

打开命令行界面（执行-CMD）,定位到apktool目录。输入命令：apktool.bat d -f  test.apk  test <br>

（命令中test.apk指的是要反编译的APK文件全名，test为反编译后资源文件存放的文件夹名称，即为：apktool.bat   d  -f    [apk文件 ]   [输出目录]）<br>

将需要反编译的test.apk改为test.zip然后解压，取出classes.dex文件，放入dex2jar工具目录内，执行dex2jar.bat   classes.dex命令，取出classes_dex2jar.jar，打开jd-gui.exe，然后打开classes_dex2jar.jar
