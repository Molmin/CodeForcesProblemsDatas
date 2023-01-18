## Description

<div><p>Mr. Kitayuta has kindly given you a string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters. You are asked to insert exactly <span class="tex-span"><i>n</i></span> lowercase English letters into <span class="tex-span"><i>s</i></span> to make it a palindrome. (A <span class="tex-font-style-it">palindrome</span> is a string that reads the same forward and backward. For example, "<span class="tex-font-style-tt">noon</span>", "<span class="tex-font-style-tt">testset</span>" and "<span class="tex-font-style-tt">a</span>" are all palindromes, while "<span class="tex-font-style-tt">test</span>" and "<span class="tex-font-style-tt">kitayuta</span>" are not.) You can choose any <span class="tex-span"><i>n</i></span> lowercase English letters, and insert each of them to any position of <span class="tex-span"><i>s</i></span>, possibly to the beginning or the end of <span class="tex-span"><i>s</i></span>. You have to insert exactly <span class="tex-span"><i>n</i></span> letters even if it is possible to turn <span class="tex-span"><i>s</i></span> into a palindrome by inserting less than <span class="tex-span"><i>n</i></span> letters.</p><p>Find the number of the palindromes that can be obtained in this way, modulo <span class="tex-span">10007</span>.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>). Each character in <span class="tex-span"><i>s</i></span> is a lowercase English letter.</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the number of the palindromes that can be obtained, modulo <span class="tex-span">10007</span>.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>). Each character in <span class="tex-span"><i>s</i></span> is a lowercase English letter.</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the number of the palindromes that can be obtained, modulo <span class="tex-span">10007</span>.</p>





```input1
revive
1

```




```input2
add
2

```




```output1
1

```




```output2
28

```



## Note

<p>For the first sample, you can obtain the palindrome "<span class="tex-font-style-tt">reviver</span>" by inserting '<span class="tex-font-style-tt">r</span>' to the end of "<span class="tex-font-style-tt">revive</span>".</p><p>For the second sample, the following 28 palindromes can be obtained: "<span class="tex-font-style-tt">adada</span>", "<span class="tex-font-style-tt">adbda</span>", ..., "<span class="tex-font-style-tt">adzda</span>", "<span class="tex-font-style-tt">dadad</span>" and "<span class="tex-font-style-tt">ddadd</span>".</p>
