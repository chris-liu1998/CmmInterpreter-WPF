# CmmInterpreter-CSharp
## C#版Cmm解释器(WPF)

词法分析->token序列->ll(1)文法->递归下降子程序法->语法树（尽可能把没用的节点去掉，方便语义分析）->生成中间代码（四元式表示）->解释执行  

已实现的功能有：  
> + 基本的数据类型：整型(int)、字符型(char)、浮点型(real)、支持三种数据类型的数组（包括多维）  
> + scan、print语句  
> + if-else语句、while语句、break语句、continue语句    
> + 赋值运算 =、+=、-=、*=、/=、%=，且可以连续赋值  
> + 声明语句、初始化（数组的初始化目前语义上不支持，语法上支持）  
> + 实现了基本的算术运算 +、-、*、/、%，关系运算 >、<、<>、==、>=、<=，逻辑运算 ||、&&、!，以及一些自增自减运算++，--  
> + 各运算符的优先级参考C语言  
> + 数组运算  

可能有些不全，记得的大概这么多_(:з」∠)_  
还有一些缺点，比如用scan语句的时候，自带控制台会很卡，而且打开程序后控制台会一直开着，不太美观，另外UI有些元素和功能没有完善（暂时是个摆设，主要是WPF的数据绑定我不太会Orz），目前没法解决，以后有时间再继续研究...(¦3[▓▓]  

## 界面演示图：  
![avatar](https://github.com/chris-liu1998/CmmInterpreter-CSharp/blob/master/CmmInterpreter/Resources/GUI.jpg)
