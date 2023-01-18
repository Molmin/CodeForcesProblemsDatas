## Description

<div><p>Caesar cipher is one of the simplest encryption techniques. To transform the original message into encrypted one using key <span class="tex-span"><i>k</i></span>, one has to replace each letter with a letter which is <span class="tex-span"><i>k</i></span> positions later in the alphabet (if this takes the position beyond Z, the rest of it is counted from the start of the alphabet). In a more formal way, if letters of the alphabet are enumerated starting with <span class="tex-span">0</span>, the result of encryption for character <span class="tex-span"><i>x</i></span> will be <img align="middle" class="tex-formula" src="file://zNs2thSc.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">26</span> is the number of letters in the Latin alphabet).</p><p>You are given the original message and the encryption key <span class="tex-span"><i>k</i></span>. Output the result of encryption.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 25</span>) — the encryption key.</p><p>The second line contains the original message — a sequence of uppercase Latin letters ('<span class="tex-font-style-tt">A</span>'-'<span class="tex-font-style-tt">Z</span>'). The length of the message is from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive.</p></div><div class="output-specification"><p>Output the result of encryption.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 25</span>) — the encryption key.</p><p>The second line contains the original message — a sequence of uppercase Latin letters ('<span class="tex-font-style-tt">A</span>'-'<span class="tex-font-style-tt">Z</span>'). The length of the message is from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive.</p>

## Output

<p>Output the result of encryption.</p>





```input1
5
CODEFORCES

```




```input2
13
FALSERULEZ

```




```output1
HTIJKTWHJX

```




```output2
SNYFREHYRM

```


