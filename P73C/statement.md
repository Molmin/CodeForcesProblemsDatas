## Description

<div><p>Vasya plays the LionAge II. He was bored of playing with a stupid computer, so he installed this popular MMORPG, to fight with his friends. Vasya came up with the name of his character — non-empty string <span class="tex-span"><i>s</i></span>, consisting of a lowercase Latin letters. However, in order not to put up a front of friends, Vasya has decided to change no more than <span class="tex-span"><i>k</i></span> letters of the character name so that the new name sounded as good as possible. Euphony of the line is defined as follows: for each pair of adjacent letters <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i></span> immediately precedes <span class="tex-span"><i>y</i></span>) the bonus <span class="tex-span"><i>c</i>(<i>x</i>, <i>y</i>)</span> is added to the result. Your task is to determine what the greatest Euphony can be obtained by changing at most <span class="tex-span"><i>k</i></span> letters in the name of the Vasya's character.</p></div><div class="input-specification"><p>The first line contains character's name <span class="tex-span"><i>s</i></span> and an integer number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>). The length of the nonempty string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">100</span>. The second line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 676</span>) — amount of pairs of letters, giving bonus to the euphony. The next <span class="tex-span"><i>n</i></span> lines contain description of these pairs «<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>c</i></span>», which means that sequence <span class="tex-span"><i>xy</i></span> gives bonus <span class="tex-span"><i>c</i></span> (<span class="tex-span"><i>x</i>, <i>y</i></span> — lowercase Latin letters, <span class="tex-span"> - 1000 ≤ <i>c</i> ≤ 1000)</span>. It is guaranteed that no pair <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> mentioned twice in the input data.</p></div><div class="output-specification"><p>Output the only number — maximum possible euphony оf the new character's name.</p></div>

## Input

<p>The first line contains character's name <span class="tex-span"><i>s</i></span> and an integer number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>). The length of the nonempty string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">100</span>. The second line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 676</span>) — amount of pairs of letters, giving bonus to the euphony. The next <span class="tex-span"><i>n</i></span> lines contain description of these pairs «<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>c</i></span>», which means that sequence <span class="tex-span"><i>xy</i></span> gives bonus <span class="tex-span"><i>c</i></span> (<span class="tex-span"><i>x</i>, <i>y</i></span> — lowercase Latin letters, <span class="tex-span"> - 1000 ≤ <i>c</i> ≤ 1000)</span>. It is guaranteed that no pair <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> mentioned twice in the input data.</p>

## Output

<p>Output the only number — maximum possible euphony оf the new character's name.</p>





```input1
winner 4
4
s e 7
o s 8
l o 13
o o 8

```




```input2
abcdef 1
5
a b -10
b c 5
c d 5
d e 5
e f 5

```




```output1
36
```




```output2
20
```



## Note

<p>In the first example the most euphony name will be <span class="tex-span"><i>looser</i></span>. It is easy to calculate that its euphony is 36.</p>
