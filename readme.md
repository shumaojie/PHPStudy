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



##PHP与mysql##
1. 数据库连接

