# 第4节：Java命名规范


## java 命名规范

1. 命名使用名词

2. 驼峰命名法（Camel-Case）: 当变量名或函数名是由一个或多个单字连结在一起，而构成的唯一识别字时，首字母以小写开头，每个单词首字母大写（第一个单词除外）。如：myFirstName

3. 项目名、包名全小写。如: com.fxy.dao

4. 类名首字母大写。 如: StudentAnswer.java

5. 接口类：UserInterface( Dao、Service ).java   接口实现类：UserInterfaceImpl( Dao、Service ).java

6. 变量名：基本结构为typeVariableName，用3字符前缀来表示数据类型。如：定义一个整形变量：intDocCount
 避免用Flag来命名状态变量
 用Is来命名逻辑变量，如：blnFileIsFound

7. 静态变量：全部大写，多词合成的变量采用“_”来连接各单词。如：USER_LIST

8. 方法：首字母以小写开头，每个单词首字母大写（第一个单词除外）。最好是一个动词或者动词词组或者第一个单词为一个动词。如：getUserName()

9.  Web层（action、controller）方法：最好是贴近web的语言，如register，login，logout
服务层方法（service）：根据方法的行为命名，只描述方法的意义，而不采用方法的目的命名。比如系统的添加新用户，用户可以前台注册，也可以管理员后台添加，方法会被重用，所以最好不要用使用register，采用add会更好写。避免使用与web层相关的方法

            数据层方法（dao）：只能以insert（插入）,delete（删除）,update（更新）,select（查找）,count（统计）开头

10. 注释 （Javadoc）：以/**开头，而以*/结束，即 /**    */

11. Jsp页面名称：
   1．全部采用小写的英文字符和”_ ”组成 
   2．整体采用模块名+操作的形式。如：user_view.jsp
    3．Jsp页面尽可能与action的意思对应，如UserListAction 对应user_list.jsp

[参考:JAVA命名规范（阿里巴巴）及其口语化总结](https://blog.csdn.net/qq_36688143/article/details/79428732)