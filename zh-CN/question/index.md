# 常见问题
本章节会记录开发中常见和遇到的一些问题，大家若在开发中遇到的问题，也可以更新到这里。

##### SQL报错排查【==修改此文件必须重启服务，否则不生效==】
解决方法：
* 打开vendor\swoft\db\src\Db.php 
* 搜索$dbResult; 
* 在return $dbResult; 前面增加一行代码var_dump($dbResult)
* ==重启服务==
