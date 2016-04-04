#液晶显示屏 Q706

##题目大意
<p>  将给出的数值，像以前红绿灯计时器的数字一样，使用'|'、'-'和空格表示</p>
例如，8可以表示成(\*代表空格)：<br>
\*\-\*<br>
|\*|<br>
\*\-\*<br>
|\*|<br>
\*\-\*<br>

##输入
每笔测试资料一列。每列有2个整数s,n（1 <= s <= 10, 0 <= n <= 99999999）。n是要显示的数字，s是每个字要求的大小。s=0, n=0代表输入结束。

##输出
请以计算机的数字样式，并以s的大小显示n。这些计算机数字是以'-'当作水平线，以'|'当作垂直线所构成，并且每个数字的大小宽为s+2，高为2s+3。数字0~9的样式请参考Sample Outpu，请注意：在2个数字中间有一空白行。

每组测试资料后亦请空一列。

##输入样例
+ 1 0123456789
+ 2 12345
+ 3 67890
+ 0 0

##输出样例
<img src="https://github.com/bwfullcolor/Practice/blob/master/oj%E9%A2%98/706%20LC-Display/706.png" alt=""><br>

##题目陷阱
输出时，最后一个数后面没有空格。

##参考
http://www.hankcs.com/program/uva-q706-lc-display.html