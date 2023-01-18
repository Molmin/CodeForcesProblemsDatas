## Description

<div><p>In Aramic language words can only represent objects.</p><p>Words in Aramic have special properties: </p><ul> <li> A word is a <span class="tex-font-style-it">root</span> if it does not contain the same letter more than once. </li><li> A <span class="tex-font-style-it">root</span> and all its permutations represent the same object. </li><li> The <span class="tex-font-style-it">root</span> $x$ of a word $y$ is the word that contains all letters that appear in $y$ in a way that each letter appears once. For example, the <span class="tex-font-style-it">root</span> of "<span class="tex-font-style-tt">aaaa</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">aaa</span>" is "<span class="tex-font-style-tt">a</span>", the <span class="tex-font-style-it">root</span> of "<span class="tex-font-style-tt">aabb</span>", "<span class="tex-font-style-tt">bab</span>", "<span class="tex-font-style-tt">baabb</span>", "<span class="tex-font-style-tt">ab</span>" is "<span class="tex-font-style-tt">ab</span>". </li><li> Any word in Aramic represents the same object as its <span class="tex-font-style-it">root</span>. </li></ul><p>You have an ancient script in Aramic. What is the number of <span class="tex-font-style-bf">different objects</span> mentioned in the script?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^3$)&nbsp;— the number of words in the script.</p><p>The second line contains $n$ words $s_1, s_2, \ldots, s_n$&nbsp;— the script itself. The length of each string does not exceed $10^3$.</p><p>It is guaranteed that all characters of the strings are small latin letters.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the number of different objects mentioned in the given ancient Aramic script.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^3$)&nbsp;— the number of words in the script.</p><p>The second line contains $n$ words $s_1, s_2, \ldots, s_n$&nbsp;— the script itself. The length of each string does not exceed $10^3$.</p><p>It is guaranteed that all characters of the strings are small latin letters.</p>

## Output

<p>Output one integer&nbsp;— the number of different objects mentioned in the given ancient Aramic script.</p>





```input1
5
a aa aaa ab abb

```




```input2
3
amer arem mrea

```




```output1
2
```




```output2
1
```



## Note

<p>In the first test, there are two objects mentioned. The roots that represent them are "<span class="tex-font-style-tt">a</span>","<span class="tex-font-style-tt">ab</span>".</p><p>In the second test, there is only one object, its root is "<span class="tex-font-style-tt">amer</span>", the other strings are just permutations of "<span class="tex-font-style-tt">amer</span>".</p>
