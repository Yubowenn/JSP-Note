# JSP基础语法
一. 指令  
二. 注释  
三. 小脚本  
四. 声明   
五. 表达式   
六. 静态内容  

## 一. 指令
### 1.page指令
* 位于jsp页面顶端，同一个页面可以包含多个page指令
* 语法：`<%@ page attribute="value" %>`
### 2.include指令
### 3.taglib指令

## 二. 注释
1. html注释
2. jsp注释
3. jsp脚本注释
* 举例：
```jsp
<!--html注释，客户端可见-->
<%--jsp注释，客户端不可见--%>
<%
    //单行注释
    /*多行注释 */
%>
```



## 三. 小脚本 
* 用来写java代码
* 语法：`<%java代码%>`
* 举例：
```jsp
<%
    out.println("大家好")；
%>
```

## 四. 声明 
* 用于定义变量或方法
* 语法：`<%!java代码%>`
* 举例：
```jsp
<%!
    String s = "余博文";
    int add(int x,int y){
        return x+y;
    }
%>
```

## 五. 表达式
* 执行语句，⚠️注意表达式后面没有分号
* 语法：`<%!java代码%>`
```jsp
<%!
    String s = "余博文";
    int add(int x,int y){
        return x+y;
    }
%>
<!--以下是表达式-->
你好，<%=s %>
x+y=<%=add(10,5) %>
```



