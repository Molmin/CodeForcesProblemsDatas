## Description

<div><p>Kaavi, the mysterious fortune teller, deeply believes that one's fate is inevitable and unavoidable. Of course, she makes her living by predicting others' future. While doing divination, Kaavi believes that magic spells can provide great power for her to see the future. </p><center><img class="tex-graphics" src="file://BlVJAkhA.png" style="max-width: 100.0%;max-height: 100.0%;"></center>&nbsp;<p>Kaavi has a string $T$ of length $m$ and all the strings with the prefix $T$ are magic spells. Kaavi also has a string $S$ of length $n$ and an empty string $A$.</p><p>During the divination, Kaavi needs to perform a sequence of operations. There are two different operations:</p><ul><li> Delete the first character of $S$ and add it at the <span class="tex-font-style-bf">front</span> of $A$.</li><li> Delete the first character of $S$ and add it at the <span class="tex-font-style-bf">back</span> of $A$.</li></ul><p>Kaavi can perform <span class="tex-font-style-bf">no more than</span> $n$ operations. To finish the divination, she wants to know the number of different operation sequences to make $A$ a magic spell (i.e. with the prefix $T$). As her assistant, can you help her? The answer might be huge, so Kaavi only needs to know the answer modulo $998\,244\,353$.</p><p>Two operation sequences are considered different if they are different in length or there exists an $i$ that their $i$-th operation is different. </p><p>A substring is a contiguous sequence of characters within a string. A prefix of a string $S$ is a substring of $S$ that occurs at the beginning of $S$.</p></div><div class="input-specification"><p>The first line contains a string $S$ of length $n$ ($1 \leq n \leq 3000$).</p><p>The second line contains a string $T$ of length $m$ ($1 \leq m \leq n$).</p><p>Both strings contain only lowercase Latin letters.</p></div><div class="output-specification"><p>The output contains only one integer &nbsp;— the answer modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a string $S$ of length $n$ ($1 \leq n \leq 3000$).</p><p>The second line contains a string $T$ of length $m$ ($1 \leq m \leq n$).</p><p>Both strings contain only lowercase Latin letters.</p>

## Output

<p>The output contains only one integer &nbsp;— the answer modulo $998\,244\,353$.</p>





```input1
abab
ba
```




```input2
defineintlonglong
signedmain
```




```input3
rotator
rotator
```




```input4
cacdcdbbbb
bdcaccdbbb
```




```output1
12
```




```output2
0
```




```output3
4
```




```output4
24
```



## Note

<p>The first test:</p><p><img class="tex-graphics" src="file://pzZPwBzn.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The red ones are the magic spells. In the first operation, Kaavi can either add the first character "<span class="tex-font-style-tt">a</span>" at the front or the back of $A$, although the results are the same, they are considered as different operations. So the answer is $6\times2=12$.</p>
