## Description

<div><p>Sergey attends lessons of the <span class="tex-span"><i>N</i></span>-ish language. Each lesson he receives a hometask. This time the task is to translate some sentence to the <span class="tex-span"><i>N</i></span>-ish language. Sentences of the <span class="tex-span"><i>N</i></span>-ish language can be represented as strings consisting of lowercase Latin letters without spaces or punctuation marks.</p><p>Sergey totally forgot about the task until half an hour before the next lesson and hastily scribbled something down. But then he recollected that in the last lesson he learned the grammar of <span class="tex-span"><i>N</i></span>-ish. The spelling rules state that <span class="tex-span"><i>N</i></span>-ish contains some "forbidden" pairs of letters: such letters can never occur in a sentence next to each other. Also, the order of the letters doesn't matter (for example, if the pair of letters "<span class="tex-font-style-tt">ab</span>" is forbidden, then any occurrences of substrings "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">ba</span>" are also forbidden). Also, each pair has different letters and each letter occurs in no more than one forbidden pair.</p><p>Now Sergey wants to correct his sentence so that it doesn't contain any "forbidden" pairs of letters that stand next to each other. However, he is running out of time, so he decided to simply cross out some letters from the sentence. What smallest number of letters will he have to cross out? When a letter is crossed out, it is "removed" so that the letters to its left and right (if they existed), become neighboring. For example, if we cross out the first letter from the string "<span class="tex-font-style-tt">aba</span>", we get the string "<span class="tex-font-style-tt">ba</span>", and if we cross out the second letter, we get "<span class="tex-font-style-tt">aa</span>".</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters — that's the initial sentence in <span class="tex-span"><i>N</i></span>-ish, written by Sergey. The length of string <span class="tex-span"><i>s</i></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 13</span>) — the number of forbidden pairs of letters.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain descriptions of forbidden pairs of letters. Each line contains exactly two different lowercase Latin letters without separators that represent the forbidden pairs. It is guaranteed that each letter is included in no more than one pair.</p></div><div class="output-specification"><p>Print the single number — the smallest number of letters that need to be removed to get a string without any forbidden pairs of neighboring letters. Please note that the answer always exists as it is always possible to remove all letters.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase Latin letters — that's the initial sentence in <span class="tex-span"><i>N</i></span>-ish, written by Sergey. The length of string <span class="tex-span"><i>s</i></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 13</span>) — the number of forbidden pairs of letters.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain descriptions of forbidden pairs of letters. Each line contains exactly two different lowercase Latin letters without separators that represent the forbidden pairs. It is guaranteed that each letter is included in no more than one pair.</p>

## Output

<p>Print the single number — the smallest number of letters that need to be removed to get a string without any forbidden pairs of neighboring letters. Please note that the answer always exists as it is always possible to remove all letters.</p>





```input1
ababa
1
ab

```




```input2
codeforces
2
do
cs

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample you should remove two letters <span class="tex-font-style-tt">b</span>.</p><p>In the second sample you should remove the second or the third letter. The second restriction doesn't influence the solution.</p>
