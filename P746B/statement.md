## Description

<div><p>Polycarp is mad about coding, that is why he writes Sveta encoded messages. He calls the <span class="tex-font-style-it">median letter</span> in a word the letter which is in the middle of the word. If the word's length is even, the median letter is the left of the two middle letters. In the following examples, the median letter is highlighted: <span class="tex-font-style-tt">con<span class="tex-font-style-bf"><span class="tex-font-style-underline">t</span></span>est</span>, <span class="tex-font-style-tt">i<span class="tex-font-style-bf"><span class="tex-font-style-underline">n</span></span>fo</span>. If the word consists of single letter, then according to above definition this letter is the median letter. </p><p>Polycarp encodes each word in the following way: he writes down the median letter of the word, then deletes it and repeats the process until there are no letters left. For example, he encodes the word <span class="tex-font-style-tt">volga</span> as <span class="tex-font-style-tt">logva</span>.</p><p>You are given an encoding <span class="tex-span"><i>s</i></span> of some word, your task is to decode it. </p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the length of the encoded word.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase English letters&nbsp;— the encoding.</p></div><div class="output-specification"><p>Print the word that Polycarp encoded.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the length of the encoded word.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase English letters&nbsp;— the encoding.</p>

## Output

<p>Print the word that Polycarp encoded.</p>





```input1
5
logva

```




```input2
2
no

```




```input3
4
abba

```




```output1
volga

```




```output2
no

```




```output3
baba

```



## Note

<p>In the first example Polycarp encoded the word <span class="tex-font-style-tt">volga</span>. At first, he wrote down the letter <span class="tex-font-style-tt">l</span> from the position <span class="tex-span">3</span>, after that his word looked like <span class="tex-font-style-tt">voga</span>. After that Polycarp wrote down the letter <span class="tex-font-style-tt">o</span> from the position <span class="tex-span">2</span>, his word became <span class="tex-font-style-tt">vga</span>. Then Polycarp wrote down the letter <span class="tex-font-style-tt">g</span> which was at the second position, the word became <span class="tex-font-style-tt">va</span>. Then he wrote down the letter <span class="tex-font-style-tt">v</span>, then the letter <span class="tex-font-style-tt">a</span>. Thus, the encoding looked like <span class="tex-font-style-tt">logva</span>.</p><p>In the second example Polycarp encoded the word <span class="tex-font-style-tt">no</span>. He wrote down the letter <span class="tex-font-style-tt">n</span>, the word became <span class="tex-font-style-tt">o</span>, and he wrote down the letter <span class="tex-font-style-tt">o</span>. Thus, in this example, the word and its encoding are the same.</p><p>In the third example Polycarp encoded the word <span class="tex-font-style-tt">baba</span>. At first, he wrote down the letter <span class="tex-font-style-tt">a</span>, which was at the position <span class="tex-span">2</span>, after that the word looked like <span class="tex-font-style-tt">bba</span>. Then he wrote down the letter <span class="tex-font-style-tt">b</span>, which was at the position <span class="tex-span">2</span>, his word looked like <span class="tex-font-style-tt">ba</span>. After that he wrote down the letter <span class="tex-font-style-tt">b</span>, which was at the position <span class="tex-span">1</span>, the word looked like <span class="tex-font-style-tt">a</span>, and he wrote down that letter <span class="tex-font-style-tt">a</span>. Thus, the encoding is <span class="tex-font-style-tt">abba</span>.</p>
