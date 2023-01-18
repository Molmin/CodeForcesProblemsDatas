## Description

<div><p>Dr. Moriarty is about to send a message to Sherlock Holmes. He has a string <span class="tex-span"><i>s</i></span>. </p><p>String <span class="tex-span"><i>p</i></span> is called a <span class="tex-font-style-it">substring</span> of string <span class="tex-span"><i>s</i></span> if you can read it starting from some position in the string <span class="tex-span"><i>s</i></span>. For example, string "<span class="tex-font-style-tt">aba</span>" has six substrings: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aba</span>".</p><p>Dr. Moriarty plans to take string <span class="tex-span"><i>s</i></span> and cut out some substring from it, let's call it <span class="tex-span"><i>t</i></span>. Then he needs to <span class="tex-font-style-underline">change</span> the substring <span class="tex-span"><i>t</i></span> zero or more times. As a result, he should obtain a fixed string <span class="tex-span"><i>u</i></span> (which is the string that should be sent to Sherlock Holmes). One change is defined as making one of the following actions: </p><ul> <li> Insert one letter to any end of the string. </li><li> Delete one letter from any end of the string. </li><li> Change one letter into any other one. </li></ul><p>Moriarty is very smart and after he chooses some substring <span class="tex-span"><i>t</i></span>, he always makes the minimal number of changes to obtain <span class="tex-span"><i>u</i></span>. </p><p>Help Moriarty choose the best substring <span class="tex-span"><i>t</i></span> from all substrings of the string <span class="tex-span"><i>s</i></span>. The substring <span class="tex-span"><i>t</i></span> should minimize the number of changes Moriarty should make to obtain the string <span class="tex-span"><i>u</i></span> from it.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters. The second line contains a non-empty string <span class="tex-span"><i>u</i></span>, consisting of lowercase Latin letters. The lengths of both strings are in the range from <span class="tex-span">1</span> to <span class="tex-span">2000</span>, inclusive.</p></div><div class="output-specification"><p>Print the only integer — the minimum number of changes that Dr. Moriarty has to make with the string that you choose.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters. The second line contains a non-empty string <span class="tex-span"><i>u</i></span>, consisting of lowercase Latin letters. The lengths of both strings are in the range from <span class="tex-span">1</span> to <span class="tex-span">2000</span>, inclusive.</p>

## Output

<p>Print the only integer — the minimum number of changes that Dr. Moriarty has to make with the string that you choose.</p>





```input1
aaaaa
aaa

```




```input2
abcabc
bcd

```




```input3
abcdef
klmnopq

```




```output1
0

```




```output2
1

```




```output3
7

```



## Note

<p>In the first sample Moriarty can take any substring of length <span class="tex-span">3</span>, and it will be equal to the required message <span class="tex-span"><i>u</i></span>, so Moriarty won't have to make any changes.</p><p>In the second sample you should take a substring consisting of characters from second to fourth ("<span class="tex-font-style-tt">bca</span>") or from fifth to sixth ("<span class="tex-font-style-tt">bc</span>"). Then you will only have to make one change: to change or to add the last character.</p><p>In the third sample the initial string <span class="tex-span"><i>s</i></span> doesn't contain any character that the message should contain, so, whatever string you choose, you will have to make at least <span class="tex-span">7</span> changes to obtain the required message.</p>
