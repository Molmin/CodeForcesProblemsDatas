## Description

<div><p>After you had helped Fedor to find friends in the «Call of Soldiers 3» game, he stopped studying completely. Today, the English teacher told him to prepare an essay. Fedor didn't want to prepare the essay, so he asked Alex for help. Alex came to help and wrote the essay for Fedor. But Fedor didn't like the essay at all. Now Fedor is going to change the essay using the synonym dictionary of the English language.</p><p>Fedor does not want to change the meaning of the essay. So the only change he would do: change a word from essay to one of its synonyms, basing on a replacement rule from the dictionary. Fedor may perform this operation any number of times.</p><p>As a result, Fedor wants to get an essay which contains as little letters «<span class="tex-font-style-tt">R</span>» (the case doesn't matter) as possible. If there are multiple essays with minimum number of «<span class="tex-font-style-tt">R</span>»s he wants to get the one with minimum length (length of essay is the sum of the lengths of all the words in it). Help Fedor get the required essay.</p><p>Please note that in this problem <span class="tex-font-style-bf">the case of letters doesn't matter</span>. For example, if the synonym dictionary says that word <span class="tex-font-style-tt">cat</span> can be replaced with word <span class="tex-font-style-tt">DOG</span>, then it is allowed to replace the word <span class="tex-font-style-tt">Cat</span> with the word <span class="tex-font-style-tt">doG</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of words in the initial essay. The second line contains words of the essay. The words are separated by a single space. It is guaranteed that the total length of the words won't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p><p>The next line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of pairs of words in synonym dictionary. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated non-empty words <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. They mean that word <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> can be replaced with word <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (but not vise versa). It is guaranteed that the total length of all pairs of synonyms doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span> characters.</p><p>All the words at input can only consist of uppercase and lowercase letters of the English alphabet.</p></div><div class="output-specification"><p>Print two integers — the minimum number of letters «<span class="tex-font-style-tt">R</span>» in an optimal essay and the minimum length of an optimal essay.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of words in the initial essay. The second line contains words of the essay. The words are separated by a single space. It is guaranteed that the total length of the words won't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p><p>The next line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of pairs of words in synonym dictionary. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated non-empty words <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. They mean that word <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> can be replaced with word <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (but not vise versa). It is guaranteed that the total length of all pairs of synonyms doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span> characters.</p><p>All the words at input can only consist of uppercase and lowercase letters of the English alphabet.</p>

## Output

<p>Print two integers — the minimum number of letters «<span class="tex-font-style-tt">R</span>» in an optimal essay and the minimum length of an optimal essay.</p>





```input1
3
AbRb r Zz
4
xR abRb
aA xr
zz Z
xr y

```




```input2
2
RuruRu fedya
1
ruruRU fedor

```




```output1
2 6

```




```output2
1 10

```


