## Description

<div><p>Hongcow is learning to spell! One day, his teacher gives him a word that he needs to learn to spell. Being a dutiful student, he immediately learns how to spell the word.</p><p>Hongcow has decided to try to make new words from this one. He starts by taking the word he just learned how to spell, and moves the last character of the word to the beginning of the word. He calls this a <span class="tex-font-style-it">cyclic shift</span>. He can apply cyclic shift many times. For example, consecutively applying cyclic shift operation to the word "abracadabra" Hongcow will get words "aabracadabr", "raabracadab" and so on.</p><p>Hongcow is now wondering how many distinct words he can generate by doing the cyclic shift arbitrarily many times. The initial string is also counted.</p></div><div class="input-specification"><p>The first line of input will be a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>), the word Hongcow initially learns how to spell. The string <span class="tex-span"><i>s</i></span> consists only of lowercase English letters ('<span class="tex-font-style-tt">a</span>'–'<span class="tex-font-style-tt">z</span>').</p></div><div class="output-specification"><p>Output a single integer equal to the number of distinct strings that Hongcow can obtain by applying the cyclic shift arbitrarily many times to the given string.</p></div>

## Input

<p>The first line of input will be a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>), the word Hongcow initially learns how to spell. The string <span class="tex-span"><i>s</i></span> consists only of lowercase English letters ('<span class="tex-font-style-tt">a</span>'–'<span class="tex-font-style-tt">z</span>').</p>

## Output

<p>Output a single integer equal to the number of distinct strings that Hongcow can obtain by applying the cyclic shift arbitrarily many times to the given string.</p>





```input1
abcd

```




```input2
bbb

```




```input3
yzyz

```




```output1
4

```




```output2
1

```




```output3
2

```



## Note

<p>For the first sample, the strings Hongcow can generate are "<span class="tex-font-style-tt">abcd</span>", "<span class="tex-font-style-tt">dabc</span>", "<span class="tex-font-style-tt">cdab</span>", and "<span class="tex-font-style-tt">bcda</span>".</p><p>For the second sample, no matter how many times Hongcow does the cyclic shift, Hongcow can only generate "<span class="tex-font-style-tt">bbb</span>".</p><p>For the third sample, the two strings Hongcow can generate are "<span class="tex-font-style-tt">yzyz</span>" and "<span class="tex-font-style-tt">zyzy</span>".</p>
