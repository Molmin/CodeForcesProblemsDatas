## Description

<div><p>Volodya likes listening to heavy metal and (occasionally) reading. No wonder Volodya is especially interested in texts concerning his favourite music style.</p><p>Volodya calls a string powerful if it starts with "<span class="tex-font-style-tt">heavy</span>" and ends with "<span class="tex-font-style-tt">metal</span>". Finding all powerful substrings (by substring Volodya means a subsequence of consecutive characters in a string) in a given text makes our hero especially joyful. Recently he felt an enormous fit of energy while reading a certain text. So Volodya decided to count all powerful substrings in this text and brag about it all day long. Help him in this difficult task. Two substrings are considered different if they appear at the different positions in the text.</p><p>For simplicity, let us assume that Volodya's text can be represented as a single string.</p></div><div class="input-specification"><p>Input contains a single non-empty string consisting of the lowercase Latin alphabet letters. Length of this string will not be greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p></div><div class="output-specification"><p>Print exactly one number — the number of powerful substrings of the given string.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>Input contains a single non-empty string consisting of the lowercase Latin alphabet letters. Length of this string will not be greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p>

## Output

<p>Print exactly one number — the number of powerful substrings of the given string.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
heavymetalisheavymetal

```




```input2
heavymetalismetal

```




```input3
trueheavymetalissotruewellitisalsosoheavythatyoucanalmostfeeltheweightofmetalonyou

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



## Note

<p>In the first sample the string "<span class="tex-font-style-tt">heavymetalisheavymetal</span>" contains powerful substring "<span class="tex-font-style-tt">heavymetal</span>" twice, also the whole string "<span class="tex-font-style-tt">heavymetalisheavymetal</span>" is certainly powerful.</p><p>In the second sample the string "<span class="tex-font-style-tt">heavymetalismetal</span>" contains two powerful substrings: "<span class="tex-font-style-tt">heavymetal</span>" and "<span class="tex-font-style-tt">heavymetalismetal</span>".</p>
