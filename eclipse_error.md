1 常见的引用包错误（ex:The import javax.servlet cannot be resolved ）    

解决方法在Eclipse中，右击项目，选择Build Path->configure build path->Libraries->Add External JARs，    
找到你计算机中tomcat的解压路径，在lib文件夹下选中"servlet-api.jar"，添加点击“确定”  ，
