## Description

<div><p>Recall that string $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly zero or all) characters. For example, for the string $a$="<span class="tex-font-style-tt">wowwo</span>", the following strings are subsequences: "<span class="tex-font-style-tt">wowwo</span>", "<span class="tex-font-style-tt">wowo</span>", "<span class="tex-font-style-tt">oo</span>", "<span class="tex-font-style-tt">wow</span>", "", and others, but the following are not subsequences: "<span class="tex-font-style-tt">owoo</span>", "<span class="tex-font-style-tt">owwwo</span>", "<span class="tex-font-style-tt">ooo</span>".</p><p>The <span class="tex-font-style-it">wow factor</span> of a string is the number of its subsequences equal to the word "<span class="tex-font-style-tt">wow</span>". Bob wants to write a string that has a large <span class="tex-font-style-it">wow factor</span>. However, the "<span class="tex-font-style-tt">w</span>" key on his keyboard is broken, so he types two "<span class="tex-font-style-tt">v</span>"s instead. </p><p>Little did he realise that he may have introduced more "<span class="tex-font-style-tt">w</span>"s than he thought. Consider for instance the string "<span class="tex-font-style-tt">ww</span>". Bob would type it as "<span class="tex-font-style-tt">vvvv</span>", but this string actually contains three occurrences of "<span class="tex-font-style-tt">w</span>": </p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span>vv</span>" </li><li> "<span class="tex-font-style-tt">v<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span>v</span>" </li><li> "<span class="tex-font-style-tt">vv<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span></span>" </li></ul><p>For example, the <span class="tex-font-style-it">wow factor</span> of the word "<span class="tex-font-style-tt">vvvovvv</span>" equals to four because there are four <span class="tex-font-style-it">wow</span>s:</p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span>v<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span><span class="tex-font-style-bf">vv</span></span>v</span>" </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span>v<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>v<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span></span>" </li><li> "<span class="tex-font-style-tt">v<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span><span class="tex-font-style-bf">o</span><span class="tex-font-style-bf">vv</span></span>v</span>" </li><li> "<span class="tex-font-style-tt">v<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span><span class="tex-font-style-bf">o</span></span>v<span class="tex-font-style-underline"><span class="tex-font-style-bf">vv</span></span></span>" </li></ul><p>Note that the subsequence "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">v</span></span>v<span class="tex-font-style-underline"><span class="tex-font-style-bf">v</span><span class="tex-font-style-bf">o</span><span class="tex-font-style-bf">vv</span></span>v</span>" does not count towards the <span class="tex-font-style-it">wow factor</span>, as the "<span class="tex-font-style-tt">v</span>"s have to be consecutive.</p><p>For a given string $s$, compute and output its <span class="tex-font-style-it">wow factor</span>. Note that it is <span class="tex-font-style-bf">not</span> guaranteed that it is possible to get $s$ from another string replacing "<span class="tex-font-style-tt">w</span>" with "<span class="tex-font-style-tt">vv</span>". For example, $s$ can be equal to "<span class="tex-font-style-tt">vov</span>".</p></div><div class="input-specification"><p>The input contains a single non-empty string $s$, consisting only of characters "<span class="tex-font-style-tt">v</span>" and "<span class="tex-font-style-tt">o</span>". The length of $s$ is at most $10^6$.</p></div><div class="output-specification"><p>Output a single integer, the <span class="tex-font-style-it">wow factor</span> of $s$.</p></div>

## Input

<p>The input contains a single non-empty string $s$, consisting only of characters "<span class="tex-font-style-tt">v</span>" and "<span class="tex-font-style-tt">o</span>". The length of $s$ is at most $10^6$.</p>

## Output

<p>Output a single integer, the <span class="tex-font-style-it">wow factor</span> of $s$.</p>





```input1
vvvovvv
```




```input2
vvovooovovvovoovoovvvvovovvvov
```




```output1
4
```




```output2
100
```



## Note

<p>The first example is explained in the legend.</p>
