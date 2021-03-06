# 1. Java正则表达式
* ^\d+(\.\d+)?
* ^ 定义了以什么开始
* \d+ 匹配一个或多个数字
* ? 设置括号内的选项是可选的
* \. 匹配 "."
*  \s+ 可以匹配多个空格
# 2. Java中是如何支持正则表达式操作的
## 2.1. Java中的String类提供了支持正则表达式操作的方法，包括：matches()、replaceAll()、replaceFirst()、split()。此外，Java中可以用Pattern类表示正则表达式对象，它提供了丰富的API进行各种正则表达式操作，如：
```import java.util.regex.Matcher;
import java.util.regex.Pattern;
class RegExpTest {
    public static void main(String[] args) {
        String str = "成都市(成华区)(武侯区)(高新区)";
        Pattern p = Pattern.compile(".*?(?=\\()");
        Matcher m = p.matcher(str);
        if(m.find()) {
            System.out.println(m.group());//成都市
        }
    }
}
```
# 3. 正则表达式语法
## 3.1. 常见匹配符号
| 正则表达式 |                          描述                           |
| --------- | ------------------------------------------------------ |
| .         | 匹配所有单个字符，除了换行字符（Linux:\n,WIndow:\r\n）     |
| ^regex    | 正则必须匹配字符串开头                                    |
| regex$    | 正则必须匹配字符串结尾                                    |
| [abc]     | 复选集定义匹配字母a或b或c                                 |
| [abc][vz] | 复选集定义匹配a或b或c，后面跟着v或z                       |
| [^abc]    | 匹配所有字符除了a或b或c                                  |
| [a-d1-7]  | 范围匹配，匹配字母 a 到 d 和数字从 1 到 7 之间，但不匹配 d1 |
| xz        | 匹配 X 后直接跟着 Z                                      |
![](_v_images/20190427100618478_22030.png)
## 3.2. 元字符
![](_v_images/20190427101801278_27543.png)
## 3.3. 限定符
![](_v_images/20190427101838593_26700.png)