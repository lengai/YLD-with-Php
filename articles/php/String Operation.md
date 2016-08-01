# 字符串操作

## 字符串的整理：
### chop()
 + 除字符串右端的空白字符或其他预定义字符
 + chop(string,charlist)
   - string：必需。规定要检查的字符串。
   - charlist:可选。规定从字符串中删除哪些字符。
            如果 charlist 参数为空，则移除以下字符：<br/>
            "\0" - NULL<br/>
            "\t" - 制表符<br/>
            "\n" - 换行<br/>
            "\x0B" - 垂直制表符<br/>
            "\r" - 回车<br/>
            " " - 空格
+ 函数示例：
 
 ```
 function funcChop() {
 	$str = "Hello World";
 	echo $str . "<br>";
 	echo chop($str,"World!");
 }
 ```
 + 输出：
 
 ```
 Hello World
 Hello
 ```
    
              
                
### ltrim()
###  trim()