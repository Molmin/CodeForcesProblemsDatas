## Description

<div><p>Kyoya Ootori is selling photobooks of the Ouran High School Host Club. He has 26 photos, labeled "a" to "z", and he has compiled them into a photo booklet with some photos in some order (possibly with some photos being duplicated). A photo booklet can be described as a string of lowercase letters, consisting of the photos in the booklet in order. He now wants to sell some "special edition" photobooks, each with one extra photo inserted anywhere in the book. He wants to make as many distinct photobooks as possible, so he can make more money. He asks Haruhi, how many distinct photobooks can he make by inserting one extra photo into the photobook he already has?</p><p>Please help Haruhi solve this problem.</p></div><div class="input-specification"><p>The first line of input will be a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 20</span>). String <span class="tex-span"><i>s</i></span> consists only of lowercase English letters. </p></div><div class="output-specification"><p>Output a single integer equal to the number of distinct photobooks Kyoya Ootori can make.</p></div>

## Input

<p>The first line of input will be a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 20</span>). String <span class="tex-span"><i>s</i></span> consists only of lowercase English letters. </p>

## Output

<p>Output a single integer equal to the number of distinct photobooks Kyoya Ootori can make.</p>





```input1
a

```




```input2
hi

```




```output1
51

```




```output2
76

```



## Note

<p>In the first case, we can make '<span class="tex-font-style-tt">ab</span>','<span class="tex-font-style-tt">ac</span>',<span class="tex-span">...</span>,'<span class="tex-font-style-tt">az</span>','<span class="tex-font-style-tt">ba</span>','<span class="tex-font-style-tt">ca</span>',<span class="tex-span">...</span>,'<span class="tex-font-style-tt">za</span>', and '<span class="tex-font-style-tt">aa</span>', producing a total of 51 distinct photo booklets. </p>
