## 学习笔记

### 字典树

从一个空的根节点出发开始查找，每个子节点包含一个字符，从根节点到某个节点的路径上的字符连起来就是该节点对应的字符串。

### KMP

前缀： 指除了最后一个字符以外，一个字符串的全部头部组合  
后缀： 指除了第一个字符以外，一个字符串的全部尾部组合  
部分匹配是前缀和后缀共有的部分，通过这个形成匹配表  


eg: abcdab  
前缀：('|'左边是前缀，右边是后缀,最后代表共有长度)  
a -> a | a -> 0  
ab -> a | b -> 0  
abc -> a,ab | bc,c -> 0  
abcd -> a,ab,abc | bcd,cd,d -> 0  
abcda -> a,ab,abc,abcd | bcda,cda,da,a -> 1  
abcdab -> a,ab,abc,abcd,abcda | bcdab,cdab,dab,ab,a -> 2  


abcdab -> 0,0,0,0,1,2  


当我们匹配一段字符串时，当在匹配过程中遇到不匹配时，不再去比较已经匹配过的字符串，而是向后移动，移动的位数为已经匹配的字符串长度-部分匹配数  


### wildcard

还得再看看

