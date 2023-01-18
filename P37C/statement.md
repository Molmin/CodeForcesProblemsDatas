## Description

<div><p>Berland scientists know that the Old Berland language had exactly <span class="tex-span"><i>n</i></span> words. Those words had lengths of <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>n</i></sub></span> letters. Every word consisted of two letters, <span class="tex-span">0</span> and <span class="tex-span">1</span>. Ancient Berland people spoke quickly and didn’t make pauses between the words, but at the same time they could always understand each other perfectly. It was possible because no word was a prefix of another one. The prefix of a string is considered to be one of its substrings that starts from the initial symbol.</p><p>Help the scientists determine whether all the words of the Old Berland language can be reconstructed and if they can, output the words themselves.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 1000</span>) — the number of words in Old Berland language. The second line contains <span class="tex-span"><i>N</i></span> space-separated integers — the lengths of these words. All the lengths are natural numbers not exceeding <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>If there’s no such set of words, in the single line output <span class="tex-font-style-tt">NO</span>. Otherwise, in the first line output <span class="tex-font-style-tt">YES</span>, and in the next <span class="tex-span"><i>N</i></span> lines output the words themselves in the order their lengths were given in the input file. If the answer is not unique, output any.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 1000</span>) — the number of words in Old Berland language. The second line contains <span class="tex-span"><i>N</i></span> space-separated integers — the lengths of these words. All the lengths are natural numbers not exceeding <span class="tex-span">1000</span>.</p>

## Output

<p>If there’s no such set of words, in the single line output <span class="tex-font-style-tt">NO</span>. Otherwise, in the first line output <span class="tex-font-style-tt">YES</span>, and in the next <span class="tex-span"><i>N</i></span> lines output the words themselves in the order their lengths were given in the input file. If the answer is not unique, output any.</p>





```input1
3
1 2 3

```




```input2
3
1 1 1

```




```output1
YES
0
10
110

```




```output2
NO

```


