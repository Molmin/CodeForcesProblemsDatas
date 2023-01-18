## Description

<div><p>Vasya is an active Internet user. One day he came across an Internet resource he liked, so he wrote its address in the notebook. We know that the address of the written resource has format:</p><center> <span class="tex-font-style-tt">&lt;protocol&gt;://&lt;domain&gt;.ru[/&lt;context&gt;]</span> </center><p>where:</p><ul> <li> <span class="tex-font-style-tt">&lt;protocol&gt;</span> can equal either "<span class="tex-font-style-tt">http</span>" (without the quotes) or "<span class="tex-font-style-tt">ftp</span>" (without the quotes), </li><li> <span class="tex-font-style-tt">&lt;domain&gt;</span> is a non-empty string, consisting of lowercase English letters, </li><li> the <span class="tex-font-style-tt">/&lt;context&gt;</span> part may not be present. If it is present, then <span class="tex-font-style-tt">&lt;context&gt;</span> is a non-empty string, consisting of lowercase English letters. </li></ul><p>If string <span class="tex-font-style-tt">&lt;context&gt;</span> isn't present in the address, then the additional character "<span class="tex-font-style-tt">/</span>" isn't written. Thus, the address has either two characters "<span class="tex-font-style-tt">/</span>" (the ones that go before the domain), or three (an extra one in front of the context).</p><p>When the boy came home, he found out that the address he wrote in his notebook had no punctuation marks. Vasya must have been in a lot of hurry and didn't write characters "<span class="tex-font-style-tt">:</span>", "<span class="tex-font-style-tt">/</span>", "<span class="tex-font-style-tt">.</span>".</p><p>Help Vasya to restore the possible address of the recorded Internet resource.</p></div><div class="input-specification"><p>The first line contains a non-empty string that Vasya wrote out in his notebook. This line consists of lowercase English letters only. </p><p>It is guaranteed that the given string contains at most 50 letters. It is guaranteed that the given string can be obtained from some correct Internet resource address, described above.</p></div><div class="output-specification"><p>Print a single line — the address of the Internet resource that Vasya liked. If there are several addresses that meet the problem limitations, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains a non-empty string that Vasya wrote out in his notebook. This line consists of lowercase English letters only. </p><p>It is guaranteed that the given string contains at most 50 letters. It is guaranteed that the given string can be obtained from some correct Internet resource address, described above.</p>

## Output

<p>Print a single line — the address of the Internet resource that Vasya liked. If there are several addresses that meet the problem limitations, you are allowed to print any of them.</p>





```input1
httpsunrux

```




```input2
ftphttprururu

```




```output1
http://sun.ru/x

```




```output2
ftp://http.ru/ruru

```



## Note

<p>In the second sample there are two more possible answers: "<span class="tex-font-style-tt">ftp://httpruru.ru</span>" and "<span class="tex-font-style-tt">ftp://httpru.ru/ru</span>".</p>
