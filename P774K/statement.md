## Description

<div><p>Stepan likes to repeat vowel letters when he writes words. For example, instead of the word "<span class="tex-font-style-tt">pobeda</span>" he can write "<span class="tex-font-style-tt">pobeeeedaaaaa</span>".</p><p>Sergey does not like such behavior, so he wants to write a program to format the words written by Stepan. This program must combine all consecutive equal vowels to a single vowel. The vowel letters are "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>", "<span class="tex-font-style-tt">i</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">u</span>" and "<span class="tex-font-style-tt">y</span>".</p><p>There are exceptions: if letters "<span class="tex-font-style-tt">e</span>" or "<span class="tex-font-style-tt">o</span>" repeat in a row exactly <span class="tex-span">2</span> times, like in words "<span class="tex-font-style-tt">feet</span>" and "<span class="tex-font-style-tt">foot</span>", the program must skip them and do not transform in one vowel. For example, the word "<span class="tex-font-style-tt">iiiimpleeemeentatiioon</span>" must be converted to the word "<span class="tex-font-style-tt">implemeentatioon</span>".</p><p>Sergey is very busy and asks you to help him and write the required program.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of letters in the word written by Stepan.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> which has length that equals to <span class="tex-span"><i>n</i></span> and contains only lowercase English letters — the word written by Stepan.</p></div><div class="output-specification"><p>Print the single string — the word written by Stepan converted according to the rules described in the statement.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of letters in the word written by Stepan.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> which has length that equals to <span class="tex-span"><i>n</i></span> and contains only lowercase English letters — the word written by Stepan.</p>

## Output

<p>Print the single string — the word written by Stepan converted according to the rules described in the statement.</p>





```input1
13
pobeeeedaaaaa

```




```input2
22
iiiimpleeemeentatiioon

```




```input3
18
aeiouyaaeeiioouuyy

```




```input4
24
aaaoooiiiuuuyyyeeeggghhh

```




```output1
pobeda

```




```output2
implemeentatioon

```




```output3
aeiouyaeeioouy

```




```output4
aoiuyeggghhh

```


