## Description

<div><p>One day Nikita found the string containing letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>" only. </p><p>Nikita thinks that string is beautiful if it can be cut into <span class="tex-span">3</span> strings (possibly empty) without changing the order of the letters, where the <span class="tex-span">1</span>-st and the <span class="tex-span">3</span>-rd one contain only letters "<span class="tex-font-style-tt">a</span>" and the <span class="tex-span">2</span>-nd contains only letters "<span class="tex-font-style-tt">b</span>".</p><p>Nikita wants to make the string beautiful by removing some (possibly none) of its characters, but without changing their order. What is the maximum length of the string he can get?</p></div><div class="input-specification"><p>The first line contains a non-empty string of length not greater than <span class="tex-span">5 000</span> containing only lowercase English letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible size of beautiful string Nikita can get.</p></div>

## Input

<p>The first line contains a non-empty string of length not greater than <span class="tex-span">5 000</span> containing only lowercase English letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p>

## Output

<p>Print a single integer&nbsp;— the maximum possible size of beautiful string Nikita can get.</p>





```input1
abba

```




```input2
bab

```




```output1
4
```




```output2
2
```



## Note

<p>It the first sample the string is already beautiful.</p><p>In the second sample he needs to delete one of "<span class="tex-font-style-tt">b</span>" to make it beautiful.</p>
