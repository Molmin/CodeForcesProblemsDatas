## Description

<div><p>There is a colony of villains with several holes aligned in a row, where each hole contains exactly one villain.</p><p>Each colony arrangement can be expressed as a string of <span class="tex-font-style-bf">even</span> length, where the $i$-th character of the string represents the type of villain in the $i$-th hole. </p><p>Iron Man can destroy a colony only if the colony arrangement is such that all villains of a certain type either live in the first half of the colony or in the second half of the colony.</p><p>His assistant Jarvis has a special power. It can swap villains of any two holes, i.e. swap any two characters in the string; he can do this operation any number of times.</p><p>Now Iron Man asks Jarvis $q$ questions. In each question, he gives Jarvis two numbers $x$ and $y$. Jarvis has to tell Iron Man the number of distinct colony arrangements he can create from the original one using his powers such that all villains having the same type as those originally living in $x$-th hole or $y$-th hole live in the same half and the Iron Man can destroy that colony arrangement.</p><p>Two colony arrangements are considered to be different if there exists a hole such that different types of villains are present in that hole in the arrangements.</p></div><div class="input-specification"><p>The first line contains a string $s$ ($2 \le |s| \le 10^{5}$), representing the initial colony arrangement. String $s$ can have both lowercase and uppercase English letters and its length is <span class="tex-font-style-bf">even</span>.</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^{5}$)&nbsp;— the number of questions.</p><p>The $i$-th of the next $q$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le |s|$, $x_i \ne y_i$)&nbsp;— the two numbers given to the Jarvis for the $i$-th question.</p></div><div class="output-specification"><p>For each question output the number of arrangements possible modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a string $s$ ($2 \le |s| \le 10^{5}$), representing the initial colony arrangement. String $s$ can have both lowercase and uppercase English letters and its length is <span class="tex-font-style-bf">even</span>.</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^{5}$)&nbsp;— the number of questions.</p><p>The $i$-th of the next $q$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le |s|$, $x_i \ne y_i$)&nbsp;— the two numbers given to the Jarvis for the $i$-th question.</p>

## Output

<p>For each question output the number of arrangements possible modulo $10^9+7$.</p>





```input1
abba
2
1 4
1 2
```




```input2
AAaa
2
1 2
1 3
```




```input3
abcd
1
1 3
```




```output1
2
0
```




```output2
2
0
```




```output3
8
```



## Note

<p>Consider the first example. For the first question, the possible arrangements are "<span class="tex-font-style-tt">aabb</span>" and "<span class="tex-font-style-tt">bbaa</span>", and for the second question, index $1$ contains '<span class="tex-font-style-tt">a</span>' and index $2$ contains '<span class="tex-font-style-tt">b</span>' and there is no valid arrangement in which all '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' are in the same half.</p>
