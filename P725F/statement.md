## Description

<div><p>Alice and Bonnie are sisters, but they don't like each other very much. So when some old family photos were found in the attic, they started to argue about who should receive which photos. In the end, they decided that they would take turns picking photos. Alice goes first.</p><p>There are <span class="tex-span"><i>n</i></span> stacks of photos. Each stack contains <span class="tex-font-style-bf">exactly two</span> photos. In each turn, a player may take only a photo from the top of one of the stacks.</p><p>Each photo is described by two non-negative integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, indicating that it is worth <span class="tex-span"><i>a</i></span> units of happiness to Alice and <span class="tex-span"><i>b</i></span> units of happiness to Bonnie. Values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> might differ for different photos.</p><p>It's allowed to pass instead of taking a photo. The game ends when all photos are taken or both players pass consecutively.</p><p>The players don't act to maximize their own happiness. Instead, each player acts to maximize the amount by which her happiness exceeds her sister's. Assuming both players play optimal, find the difference between Alice's and Bonnie's happiness. That is, if there's a perfectly-played game such that Alice has <span class="tex-span"><i>x</i></span> happiness and Bonnie has <span class="tex-span"><i>y</i></span> happiness at the end, you should print <span class="tex-span"><i>x</i> - <i>y</i></span>.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of two-photo stacks. Then follow <span class="tex-span"><i>n</i></span> lines, each describing one of the stacks. A stack is described by four space-separated non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, each not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> describe the top photo in the stack, while <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> describe the bottom photo in the stack.</p></div><div class="output-specification"><p>Output a single integer: the difference between Alice's and Bonnie's happiness if both play optimally.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of two-photo stacks. Then follow <span class="tex-span"><i>n</i></span> lines, each describing one of the stacks. A stack is described by four space-separated non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, each not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> describe the top photo in the stack, while <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> describe the bottom photo in the stack.</p>

## Output

<p>Output a single integer: the difference between Alice's and Bonnie's happiness if both play optimally.</p>





```input1
2
12 3 4 7
1 15 9 1

```




```input2
2
5 4 8 8
4 12 14 0

```




```input3
1
0 10 0 10

```




```output1
1

```




```output2
4

```




```output3
-10

```


