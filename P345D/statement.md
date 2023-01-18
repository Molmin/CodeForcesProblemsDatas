## Description

<div><p>A chain letter is a kind of a message which urges the recipient to forward it to as many contacts as possible, usually with some kind of mystic explanation. Of course, this is only a superstition, and you don't believe in it, but all your friends do. You know that today there will be one of these letters going around, and you want to know how many times you'll receive it — of course, not that you'll be sending it yourself!</p><p>You are given an array of strings <span class="tex-span"><i>f</i></span> with <span class="tex-span"><i>n</i></span> elements which describes the contacts between you and <span class="tex-span"><i>n</i> - 1</span> of your friends: <span class="tex-span"><i>j</i></span>-th character of <span class="tex-span"><i>i</i></span>-th string (<span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>i</i></span>][<span class="tex-span"><i>j</i></span>]) is "<span class="tex-font-style-tt">1</span>" if people <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> will send messages to each other, and "<span class="tex-font-style-tt">0</span>" otherwise. Person 1 starts sending the letter to all his contacts; every person who receives the letter for the first time sends it to all his contacts. You are person <span class="tex-span"><i>n</i></span>, and you don't forward the letter when you receive it. </p><p>Calculate the number of copies of this letter you'll receive.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 50)</span> — the number of people involved. Next <span class="tex-span"><i>n</i></span> following lines contain elements of <span class="tex-span"><i>f</i></span>, strings of length <span class="tex-span"><i>n</i></span>. Each character in <span class="tex-span"><i>f</i></span> is either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". It's guaranteed that two following equations hold: <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>i</i></span>][<span class="tex-span"><i>j</i></span>] = <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>j</i></span>][<span class="tex-span"><i>i</i></span>], <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>i</i></span>][<span class="tex-span"><i>i</i></span>] = 0, for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the number of copies of the letter you will receive eventually.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 50)</span> — the number of people involved. Next <span class="tex-span"><i>n</i></span> following lines contain elements of <span class="tex-span"><i>f</i></span>, strings of length <span class="tex-span"><i>n</i></span>. Each character in <span class="tex-span"><i>f</i></span> is either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". It's guaranteed that two following equations hold: <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>i</i></span>][<span class="tex-span"><i>j</i></span>] = <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>j</i></span>][<span class="tex-span"><i>i</i></span>], <span class="tex-span"><i>f</i></span>[<span class="tex-span"><i>i</i></span>][<span class="tex-span"><i>i</i></span>] = 0, for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>.</p>

## Output

<p>Output a single integer — the number of copies of the letter you will receive eventually.</p>





```input1
4
0111
1011
1101
1110

```




```input2
4
0110
1010
1100
0000

```




```input3
4
0101
1001
0001
1110

```




```output1
3

```




```output2
0

```




```output3
2

```



## Note

<p>In the first case, everybody sends letters to everyone, so you get copies from all three of your friends.</p><p>In the second case, you don't know any of these people, so they don't bother you with their superstitious stuff.</p><p>In the third case, two of your friends send you copies of the letter but the third friend doesn't know them so he is unaffected.</p>
