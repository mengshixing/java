1 常见的引用包错误（ex:The import javax.servlet cannot be resolved ）    

解决方法在Eclipse中，右击项目，选择Build Path->configure build path->Libraries->Add External JARs，    
找到你计算机中tomcat的解压路径，在lib文件夹下选中"servlet-api.jar"，添加点击“确定”  ，

2 centos环境下提示 no libsigar-x86-linux.so in java.library.path 错误

下载请把libsigar-x86-linux.so文件一般来说放到/usr/lib64下即可

3  ERROR net.sf.ehcache.Cache - Unable to set localhost. This prevents creation of a GUID. Cause was: liulan: liulan: 未知的名称或服务.java.net.UnknownHostException: liulan: liulan: 未知的名称或服务

vi /etc/hosts 加到127.0.0.1 后面即可
