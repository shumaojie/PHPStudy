#PHP 学习笔记#
##注意点##
1. 字符串相加是.(点号)而不是+（加号）。所学语言中php是这样
2. 判断字符串中含有字符串使用count(explode(nodele,source))>1
3. 变量命名是$,弱类型语言
4. 在查询数据库之前最好添加mysql_query("SET NAMES utf8");
5. <?php  里面填充内容 ?>
6. 在windows中安装xmapp,在ubuntu里面添加lamp来安装php集成环境
7. 语句需要用;(分号)作为结尾
8. 前后端交互，前端使用$.post()  那么后端使用 $para1= empty($_POST['para1']) ? die("请输入参数名称") : mysql_escape_string($_POST['para1']);
9. 对数组进行操作，$selectitems = array(); array_push($array,$item);
10. PHP对文中只替换一次的方法  $str=preg_replace('/abc/','abc',$str,1);
11. PHP中对文中含有/或者替换中含有/进行替换的需要书写额外的函数。例如str_replace_limit
12. PHP中字符串数组中删除里面的一个字字符串items.splice(index,1)



##PHP与mysql##
1. 数据库连接
2. 判断时间相等
3. 数据库进行更新update:$query = "update marketmsg set context='" . $Msg . "' where market='" . $market . "' and time='" . $time1 . "'";
4. 值需要加''
5. 查询语句：$query = "Select * FROM marketmsg WHERE market='" . $market . "' order by time desc ";
6. desc 降序，比如时间最前的排在前面。 asc升序，时间最早的排在前面
7. 对于子分类查询
8. sql表格的建立需要冗余机制
9. php链接远程数据库。 Warning: mysql_connect(): An established connection was aborted by the software in your host machine. 原因是防火墙
10.socket client不能主动来链接电脑是在哪里进行设置？

