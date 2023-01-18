## Description

<div><p>Advertising has become part of our routine. And now, in the era of progressive technologies, we need your ideas to make advertising better!</p><p>In this problem we'll look at a simplified version of context advertising. You've got a text, consisting of exactly <span class="tex-span"><i>n</i></span> words. A standard advertising banner has exactly <span class="tex-span"><i>r</i></span> lines, each line can contain at most <span class="tex-span"><i>c</i></span> characters. The potential customer always likes it when they can see lots of advertising, so you should determine which maximum number of consecutive words from the text can be written on the banner. Single words in one line of the banner should be separated by spaces. You are allowed to insert more than one space at once. Note that you are not allowed to break the words, that is, each word in the text must occupy exactly one line in the banner. Besides, you cannot change the word order, that is, if you read the banner text consecutively, from top to bottom and from left to right, you should get some consecutive part of the advertisement text.</p><p>More formally, the statement can be written like that. Let's say that all words are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they occur in the advertisement text. Then you have to choose all words, starting from some <span class="tex-span"><i>i</i></span>-th one and ending with some <span class="tex-span"><i>j</i></span>-th one <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i>)</span>, so that all of them could be written on the banner. There must be as many words as possible. See the samples for clarifications.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>r</i> × <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>). The next line contains a text, consisting of <span class="tex-span"><i>n</i></span> words. The words consist only of lowercase English letters and are not empty. The words in the lines are separated by single spaces. The total number of characters in all words doesn't exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print at most <span class="tex-span"><i>r</i></span> lines, in each line print at most <span class="tex-span"><i>c</i></span> characters — the optimal advertisement banner. If there are multiple advertisement banners, print any of them. </p><p>Note that some lines of the banner <span class="tex-font-style-bf">can be empty</span>. You are allowed not to print such lines.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>r</i> × <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>). The next line contains a text, consisting of <span class="tex-span"><i>n</i></span> words. The words consist only of lowercase English letters and are not empty. The words in the lines are separated by single spaces. The total number of characters in all words doesn't exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print at most <span class="tex-span"><i>r</i></span> lines, in each line print at most <span class="tex-span"><i>c</i></span> characters — the optimal advertisement banner. If there are multiple advertisement banners, print any of them. </p><p>Note that some lines of the banner <span class="tex-font-style-bf">can be empty</span>. You are allowed not to print such lines.</p>





```input1
9 4 12
this is a sample text for croc final round

```




```input2
9 1 9
this is a sample text for croc final round

```




```input3
6 2 3
croc a a a croc a

```




```input4
2 2 5
first second

```




```output1
this is a
sample text
for croc
final round

```




```output2
this is a

```




```output3
a a
a

```




```output4
first

```


