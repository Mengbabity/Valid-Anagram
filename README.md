# Valid-Anagram

两个字符串，判读是否互为乱序字符串。

建立一个map。
开始的想法是将两个字符串放入两个map中，但无法比较。解决方法是，仅建立一个map，m[s[i]]++,m[p[i]]--。
即前一个字符串进行加入，后一个字符串进行删减。若互为乱序字符串则应在最后，map的每个key对应的value为0，否则返回false。

在c++11中，map的遍历方法：for(auto it:map)
                             it.first/it.second
