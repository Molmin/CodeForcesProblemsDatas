## Description

<div><p>You are given a string $s$. You have to reverse it — that is, the first letter should become equal to the last letter before the reversal, the second letter should become equal to the second-to-last letter before the reversal — and so on. For example, if your goal is to reverse the string "<span class="tex-font-style-tt">abddea</span>", you should get the string "<span class="tex-font-style-tt">aeddba</span>". To accomplish your goal, you can swap the <span class="tex-font-style-bf">neighboring elements of the string</span>. </p><p>Your task is to calculate the minimum number of swaps you have to perform to reverse the given string.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 200\,000$) — the length of $s$.</p><p>The second line contains $s$ — a string consisting of $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print one integer — the minimum number of swaps of neighboring elements you have to perform to reverse the string.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 200\,000$) — the length of $s$.</p><p>The second line contains $s$ — a string consisting of $n$ lowercase Latin letters.</p>

## Output

<p>Print one integer — the minimum number of swaps of neighboring elements you have to perform to reverse the string.</p>





```input1
5
aaaza
```




```input2
6
cbaabc
```




```input3
9
icpcsguru
```




```output1
2
```




```output2
0
```




```output3
30
```



## Note

<p>In the first example, you have to swap the third and the fourth elements, so the string becomes "<span class="tex-font-style-tt">aazaa</span>". Then you have to swap the second and the third elements, so the string becomes "<span class="tex-font-style-tt">azaaa</span>". So, it is possible to reverse the string in two swaps.</p><p>Since the string in the second example is a palindrome, you don't have to do anything to reverse it.</p>
