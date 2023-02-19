## Description

<div><p>Not so long ago, Vlad had a birthday, for which he was presented with a package of candies. There were $n$ types of candies, there are $a_i$ candies of the type $i$ ($1 \le i \le n$).</p><p>Vlad decided to eat exactly one candy every time, choosing any of the candies of a type that is currently the most frequent (if there are several such types, he can choose <span class="tex-font-style-bf">any</span> of them). To get the maximum pleasure from eating, Vlad <span class="tex-font-style-bf">does not want</span> to eat two candies of the same type in a row.</p><p>Help him figure out if he can eat all the candies without eating two identical candies in a row.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input test cases.</p><p>The following is a description of $t$ test cases of input, two lines for each.</p><p>The first line of the case contains the single number $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of types of candies in the package.</p><p>The second line of the case contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$) — the number of candies of the type $i$.</p><p>It is guaranteed that the sum of $n$ for all cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ lines, each of which contains the answer to the corresponding test case of input. As an answer, output "<span class="tex-font-style-tt">YES</span>" if Vlad can eat candy as planned, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input test cases.</p><p>The following is a description of $t$ test cases of input, two lines for each.</p><p>The first line of the case contains the single number $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of types of candies in the package.</p><p>The second line of the case contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$) — the number of candies of the type $i$.</p><p>It is guaranteed that the sum of $n$ for all cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ lines, each of which contains the answer to the corresponding test case of input. As an answer, output "<span class="tex-font-style-tt">YES</span>" if Vlad can eat candy as planned, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1
6
2
2 3
1
2
5
1 6 2 4 3
4
2 2 2 1
3
1 1000000000 999999999
1
1
```




```output1
YES
NO
NO
YES
YES
YES
```



## Note

<p>In the first example, it is necessary to eat sweets in this order:</p><ul><li> a candy of the type $2$, it is the most frequent, now $a = [2, 2]$;</li><li> a candy of the type $1$, there are the same number of candies of the type $2$, but we just ate one, now $a = [1, 2]$;</li><li> a candy of the type $2$, it is the most frequent, now $a = [1, 1]$;</li><li> a candy of the type $1$, now $a = [0, 1]$;</li><li> a candy of the type $2$, now $a = [0, 0]$ and the candy has run out.</li></ul><p>In the second example, all the candies are of the same type and it is impossible to eat them without eating two identical ones in a row.</p><p>In the third example, first of all, a candy of the type $2$ will be eaten, after which this kind will remain the only kind that is the most frequent, and you will have to eat a candy of the type $2$ again.</p>
