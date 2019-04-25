# Java正则表达式
* ^\d+(\.\d+)?
* ^ 定义了以什么开始
* \d+ 匹配一个或多个数字
* ? 设置括号内的选项是可选的
* \. 匹配 "."
*  \s+ 可以匹配多个空格
# Java中是如何支持正则表达式操作的
## Java中的String类提供了支持正则表达式操作的方法，包括：matches()、replaceAll()、replaceFirst()、split()。此外，Java中可以用Pattern类表示正则表达式对象，它提供了丰富的API进行各种正则表达式操作，如：
```import java.util.regex.Matcher;
import java.util.regex.Pattern;
class RegExpTest {
    public static void main(String[] args) {
        String str = "成都市(成华区)(武侯区)(高新区)";
        Pattern p = Pattern.compile(".*?(?=\\()");
        Matcher m = p.matcher(str);
        if(m.find()) {
            System.out.println(m.group());
        }
    }
}
```