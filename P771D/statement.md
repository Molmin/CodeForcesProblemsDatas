## Description

<div><p>Bear Limak prepares problems for a programming competition. Of course, it would be unprofessional to mention the sponsor name in the statement. Limak takes it seriously and he is going to change some words. To make it still possible to read, he will try to modify each word as little as possible.</p><p>Limak has a string <span class="tex-span"><i>s</i></span> that consists of uppercase English letters. In one move he can swap two <span class="tex-font-style-bf">adjacent</span> letters of the string. For example, he can transform a string "<span class="tex-font-style-tt">ABBC</span>" into "<span class="tex-font-style-tt">BABC</span>" or "<span class="tex-font-style-tt">ABCB</span>" in one move.</p><p>Limak wants to obtain a string without a substring "<span class="tex-font-style-tt">VK</span>" (i.e. there should be no letter '<span class="tex-font-style-tt">V</span>' immediately followed by letter '<span class="tex-font-style-tt">K</span>'). It can be easily proved that it's possible for any initial string <span class="tex-span"><i>s</i></span>.</p><p>What is the minimum possible number of moves Limak can do?</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75</span>)&nbsp;— the length of the string.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of uppercase English letters. The length of the string is equal to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print one integer, denoting the minimum possible number of moves Limak can do, in order to obtain a string without a substring "<span class="tex-font-style-tt">VK</span>".</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75</span>)&nbsp;— the length of the string.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of uppercase English letters. The length of the string is equal to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print one integer, denoting the minimum possible number of moves Limak can do, in order to obtain a string without a substring "<span class="tex-font-style-tt">VK</span>".</p>





```input1
4
VKVK

```




```input2
5
BVVKV

```




```input3
7
VVKEVKK

```




```input4
20
VKVKVVVKVOVKVQKKKVVK

```




```input5
5
LIMAK

```




```output1
3

```




```output2
2

```




```output3
3

```




```output4
8

```




```output5
0

```



## Note

<p>In the first sample, the initial string is "<span class="tex-font-style-tt">VKVK</span>". The minimum possible number of moves is <span class="tex-span">3</span>. One optimal sequence of moves is:</p><ol><li> Swap two last letters. The string becomes "<span class="tex-font-style-tt">VKKV</span>".</li><li> Swap first two letters. The string becomes "<span class="tex-font-style-tt">KVKV</span>".</li><li> Swap the second and the third letter. The string becomes "<span class="tex-font-style-tt">KKVV</span>". Indeed, this string doesn't have a substring "<span class="tex-font-style-tt">VK</span>".</li></ol><p>In the second sample, there are two optimal sequences of moves. One is "<span class="tex-font-style-tt">BVVKV</span>"<span class="tex-span">  →  </span>"<span class="tex-font-style-tt">VBVKV</span>"<span class="tex-span">  →  </span>"<span class="tex-font-style-tt">VVBKV</span>". The other is "<span class="tex-font-style-tt">BVVKV</span>"<span class="tex-span">  →  </span>"<span class="tex-font-style-tt">BVKVV</span>"<span class="tex-span">  →  </span>"<span class="tex-font-style-tt">BKVVV</span>".</p><p>In the fifth sample, no swaps are necessary.</p>
