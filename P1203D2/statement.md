## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the length of the string</span>.</p><p>You are given a string $s$ and a string $t$, both consisting only of lowercase Latin letters. It is guaranteed that $t$ can be obtained from $s$ by removing some (possibly, zero) number of characters (not necessary contiguous) from $s$ without changing order of remaining characters (in other words, it is guaranteed that $t$ is a subsequence of $s$).</p><p>For example, the strings "<span class="tex-font-style-tt">test</span>", "<span class="tex-font-style-tt">tst</span>", "<span class="tex-font-style-tt">tt</span>", "<span class="tex-font-style-tt">et</span>" and "" are subsequences of the string "<span class="tex-font-style-tt">test</span>". But the strings "<span class="tex-font-style-tt">tset</span>", "<span class="tex-font-style-tt">se</span>", "<span class="tex-font-style-tt">contest</span>" are not subsequences of the string "<span class="tex-font-style-tt">test</span>".</p><p>You want to remove some substring (contiguous subsequence) from $s$ of <span class="tex-font-style-bf">maximum possible length</span> such that after removing this substring $t$ will remain a subsequence of $s$.</p><p>If you want to remove the substring $s[l;r]$ then the string $s$ will be transformed to $s_1 s_2 \dots s_{l-1} s_{r+1} s_{r+2} \dots s_{|s|-1} s_{|s|}$ (where $|s|$ is the length of $s$).</p><p>Your task is to find the maximum possible length of the substring you can remove so that $t$ is still a subsequence of $s$.</p></div><div class="input-specification"><p>The first line of the input contains one string $s$ consisting of at least $1$ and at most $2 \cdot 10^5$ lowercase Latin letters.</p><p>The second line of the input contains one string $t$ consisting of at least $1$ and at most $2 \cdot 10^5$ lowercase Latin letters.</p><p>It is guaranteed that $t$ is a subsequence of $s$.</p></div><div class="output-specification"><p>Print one integer — the maximum possible length of the substring you can remove so that $t$ is still a subsequence of $s$.</p></div>

## Input

<p>The first line of the input contains one string $s$ consisting of at least $1$ and at most $2 \cdot 10^5$ lowercase Latin letters.</p><p>The second line of the input contains one string $t$ consisting of at least $1$ and at most $2 \cdot 10^5$ lowercase Latin letters.</p><p>It is guaranteed that $t$ is a subsequence of $s$.</p>

## Output

<p>Print one integer — the maximum possible length of the substring you can remove so that $t$ is still a subsequence of $s$.</p>





```input1
bbaba
bb
```




```input2
baaba
ab
```




```input3
abcde
abcde
```




```input4
asdfasdf
fasd
```




```output1
3
```




```output2
2
```




```output3
0
```




```output4
3
```


