## Description

<div><p>You are given a string $s$ consisting of lowercase Latin letters. Let the length of $s$ be $|s|$. You may perform several operations on this string.</p><p>In one operation, you can choose some index $i$ and <span class="tex-font-style-bf">remove</span> the $i$-th character of $s$ ($s_i$) if <span class="tex-font-style-bf">at least one</span> of its adjacent characters is the <span class="tex-font-style-it">previous</span> letter in the Latin alphabet for $s_i$. For example, the <span class="tex-font-style-it">previous</span> letter for <span class="tex-font-style-tt">b</span> is <span class="tex-font-style-tt">a</span>, the <span class="tex-font-style-it">previous</span> letter for <span class="tex-font-style-tt">s</span> is <span class="tex-font-style-tt">r</span>, the letter <span class="tex-font-style-tt">a</span> has no <span class="tex-font-style-it">previous</span> letters. Note that after each removal the length of the string decreases by one. So, the index $i$ should satisfy the condition $1 \le i \le |s|$ during each operation.</p><p>For the character $s_i$ adjacent characters are $s_{i-1}$ and $s_{i+1}$. The first and the last characters of $s$ both have only one adjacent character (unless $|s| = 1$).</p><p>Consider the following example. Let $s=$ <span class="tex-font-style-tt">bacabcab</span>.</p><ol> <li> During the first move, you can remove the first character $s_1=$ <span class="tex-font-style-tt">b</span> because $s_2=$ <span class="tex-font-style-tt">a</span>. Then the string becomes $s=$ <span class="tex-font-style-tt">acabcab</span>. </li><li> During the second move, you can remove the fifth character $s_5=$ <span class="tex-font-style-tt">c</span> because $s_4=$ <span class="tex-font-style-tt">b</span>. Then the string becomes $s=$ <span class="tex-font-style-tt">acabab</span>. </li><li> During the third move, you can remove the sixth character $s_6=$'<span class="tex-font-style-tt">b</span>' because $s_5=$ <span class="tex-font-style-tt">a</span>. Then the string becomes $s=$ <span class="tex-font-style-tt">acaba</span>. </li><li> During the fourth move, the only character you can remove is $s_4=$ <span class="tex-font-style-tt">b</span>, because $s_3=$ <span class="tex-font-style-tt">a</span> (or $s_5=$ <span class="tex-font-style-tt">a</span>). The string becomes $s=$ <span class="tex-font-style-tt">acaa</span> and you cannot do anything with it. </li></ol><p>Your task is to find the maximum possible number of characters you can remove if you choose the sequence of operations optimally.</p></div><div class="input-specification"><p>The first line of the input contains one integer $|s|$ ($1 \le |s| \le 100$) — the length of $s$.</p><p>The second line of the input contains one string $s$ consisting of $|s|$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print one integer — the maximum possible number of characters you can remove if you choose the sequence of moves optimally.</p></div>

## Input

<p>The first line of the input contains one integer $|s|$ ($1 \le |s| \le 100$) — the length of $s$.</p><p>The second line of the input contains one string $s$ consisting of $|s|$ lowercase Latin letters.</p>

## Output

<p>Print one integer — the maximum possible number of characters you can remove if you choose the sequence of moves optimally.</p>





```input1
8
bacabcab
```




```input2
4
bcda
```




```input3
6
abbbbb
```




```output1
4
```




```output2
3
```




```output3
5
```



## Note

<p>The first example is described in the problem statement. Note that the sequence of moves provided in the statement is not the only, but it can be shown that the maximum possible answer to this test is $4$.</p><p>In the second example, you can remove all but one character of $s$. The only possible answer follows.</p><ol> <li> During the first move, remove the third character $s_3=$ <span class="tex-font-style-tt">d</span>, $s$ becomes <span class="tex-font-style-tt">bca</span>. </li><li> During the second move, remove the second character $s_2=$ <span class="tex-font-style-tt">c</span>, $s$ becomes <span class="tex-font-style-tt">ba</span>. </li><li> And during the third move, remove the first character $s_1=$ <span class="tex-font-style-tt">b</span>, $s$ becomes <span class="tex-font-style-tt">a</span>. </li></ol>
