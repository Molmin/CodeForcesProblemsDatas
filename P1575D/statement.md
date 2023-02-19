## Description

<div><p>Mr. Chanek has an integer represented by a string $s$. Zero or more digits have been erased and are denoted by the character <span class="tex-font-style-tt">_</span>. There are also zero or more digits marked by the character <span class="tex-font-style-tt">X</span>, meaning they're the same digit.</p><p>Mr. Chanek wants to count the number of possible integer $s$, where $s$ is divisible by $25$. Of course, $s$ must not contain any leading zero. He can replace the character <span class="tex-font-style-tt">_</span> with any digit. He can also replace the character <span class="tex-font-style-tt">X</span> with any digit, but it must be the same for every character <span class="tex-font-style-tt">X</span>.</p><p>As a note, a leading zero is any <span class="tex-font-style-tt">0</span> digit that comes before the first nonzero digit in a number string in positional notation. For example, <span class="tex-font-style-tt">0025</span> has two leading zeroes. An exception is the integer zero, (<span class="tex-font-style-tt">0</span> has no leading zero, but <span class="tex-font-style-tt">0000</span> has three leading zeroes).</p></div><div class="input-specification"><p>One line containing the string $s$ ($1 \leq |s| \leq 8$). The string $s$ consists of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">3</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">5</span>, <span class="tex-font-style-tt">6</span>, <span class="tex-font-style-tt">7</span>, <span class="tex-font-style-tt">8</span>, <span class="tex-font-style-tt">9</span>, <span class="tex-font-style-tt">_</span>, and <span class="tex-font-style-tt">X</span>.</p></div><div class="output-specification"><p>Output an integer denoting the number of possible integer $s$.</p></div>

## Input

<p>One line containing the string $s$ ($1 \leq |s| \leq 8$). The string $s$ consists of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">3</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">5</span>, <span class="tex-font-style-tt">6</span>, <span class="tex-font-style-tt">7</span>, <span class="tex-font-style-tt">8</span>, <span class="tex-font-style-tt">9</span>, <span class="tex-font-style-tt">_</span>, and <span class="tex-font-style-tt">X</span>.</p>

## Output

<p>Output an integer denoting the number of possible integer $s$.</p>





```input1
25
```




```input2
_00
```




```input3
_XX
```




```input4
0
```




```input5
0_25
```




```output1
1
```




```output2
9
```




```output3
9
```




```output4
1
```




```output5
0
```



## Note

<p>In the first example, the only possible $s$ is $25$.</p><p>In the second and third example, $s \in \{100, 200,300,400,500,600,700,800,900\}$.</p><p>In the fifth example, all possible $s$ will have at least one leading zero.</p>
