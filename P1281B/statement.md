## Description

<div><p>Your friend Jeff Zebos has been trying to run his new online company, but it's not going very well. He's not getting a lot of sales on his website which he decided to call <span class="tex-font-style-bf">Azamon</span>. His big problem, you think, is that he's not ranking high enough on the search engines. If only he could rename his products to have better names than his competitors, then he'll be at the top of the search results and will be a millionaire.</p><p>After doing some research, you find out that search engines only sort their results lexicographically. If your friend could rename his products to lexicographically smaller strings than his competitor's, then he'll be at the top of the rankings!</p><p>To make your strategy less obvious to his competitors, you decide to swap no more than two letters of the product names.</p><p>Please help Jeff to find improved names for his products that are lexicographically smaller than his competitor's!</p><p>Given the string $s$ representing Jeff's product name and the string $c$ representing his competitor's product name, find a way to swap <span class="tex-font-style-bf">at most one pair</span> of characters in $s$ (that is, find two distinct indices $i$ and $j$ and swap $s_i$ and $s_j$) such that the resulting new name becomes strictly lexicographically smaller than $c$, or determine that it is impossible.</p><p><span class="tex-font-style-bf">Note:</span> String $a$ is <span class="tex-font-style-underline">strictly lexicographically smaller</span> than string $b$ if and only if one of the following holds:</p><ul> <li> $a$ is a <span class="tex-font-style-underline">proper prefix</span> of $b$, that is, $a$ is a <span class="tex-font-style-underline">prefix</span> of $b$ such that $a \neq b$; </li><li> There exists an integer $1 \le i \le \min{(|a|, |b|)}$ such that $a_i &lt; b_i$ and $a_j = b_j$ for $1 \le j &lt; i$. </li></ul></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 1500$) denoting the number of test cases. The next lines contain descriptions of the test cases.</p><p>Each test case consists of a single line containing two space-separated strings $s$ and $c$ ($2 \le |s| \le 5000, 1 \le |c| \le 5000$). The strings $s$ and $c$ consists of uppercase English letters.</p><p>It is guaranteed that the sum of $|s|$ in the input is at most $5000$ and the sum of the $|c|$ in the input is at most $5000$.</p></div><div class="output-specification"><p>For each test case, output a single line containing a single string, which is either</p><ul> <li> the new name which is obtained after swapping no more than one pair of characters that is strictly lexicographically smaller than $c$. In case there are many possible such strings, you can output any of them; </li><li> three dashes (the string "<span class="tex-font-style-tt">---</span>" without quotes) if it is impossible. </li></ul></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 1500$) denoting the number of test cases. The next lines contain descriptions of the test cases.</p><p>Each test case consists of a single line containing two space-separated strings $s$ and $c$ ($2 \le |s| \le 5000, 1 \le |c| \le 5000$). The strings $s$ and $c$ consists of uppercase English letters.</p><p>It is guaranteed that the sum of $|s|$ in the input is at most $5000$ and the sum of the $|c|$ in the input is at most $5000$.</p>

## Output

<p>For each test case, output a single line containing a single string, which is either</p><ul> <li> the new name which is obtained after swapping no more than one pair of characters that is strictly lexicographically smaller than $c$. In case there are many possible such strings, you can output any of them; </li><li> three dashes (the string "<span class="tex-font-style-tt">---</span>" without quotes) if it is impossible. </li></ul>





```input1
3
AZAMON APPLE
AZAMON AAAAAAAAAAALIBABA
APPLE BANANA
```




```output1
AMAZON
---
APPLE
```



## Note

<p>In the first test case, it is possible to swap the second and the fourth letters of the string and the resulting string "<span class="tex-font-style-tt">AMAZON</span>" is lexicographically smaller than "<span class="tex-font-style-tt">APPLE</span>".</p><p>It is impossible to improve the product's name in the second test case and satisfy all conditions.</p><p>In the third test case, it is possible not to swap a pair of characters. The name "<span class="tex-font-style-tt">APPLE</span>" is lexicographically smaller than "<span class="tex-font-style-tt">BANANA</span>". Note that there are other valid answers, e.g., "<span class="tex-font-style-tt">APPEL</span>". </p>
