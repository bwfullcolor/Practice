#10069 Distinct SUbsequences

##题目大意
在母串中寻找子串(可不连续)出现的最大次数

##输入样例
2<br>
babgbag<br>
bag<br>
rabbbit<br>
rabbit<br>

##输出样例
5<br>
3<br>

##解决思路
dp[i][j] = dp[i - 1][j] + dp[i - 1][j - 1] （str[i] == sub[j]）<br>
<p>        = dp[i - 1][j]                    （str[i] != sub[j]）</p>

首先明确一个概念：子串结尾字母与母串结尾字母(假设第i位)不相同，那么想要找到与母串中子串的个数，可以在母串前i-1位寻找。问题第一次简化：dp[i] = dp[i - 1]。

str[i] == sub[j]的情况：要得到一个完整的子串，则需要算上母串前i-1子串前j-1的情况(dp[i-1][j-1])，另外还有一种可能，就是在母串前i-1位中已经含有完整子串的情况(这里指子串前j位)。

<h2 color=red>注意</h2>
本题目未AC，提供的思路完全正确

未AC原因：本题需高精度计算
