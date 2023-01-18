## Description

<div><p>Hacker Zhorik wants to decipher two secret messages he intercepted yesterday. Yeah message is a sequence of encrypted blocks, each of them consists of several bytes of information.</p><p>Zhorik knows that each of the messages is an archive containing one or more files. Zhorik knows how each of these archives was transferred through the network: if an archive consists of <span class="tex-span"><i>k</i></span> files of sizes <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>k</i></sub></span> bytes, then the <span class="tex-span"><i>i</i></span>-th file is split to one or more blocks <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>b</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>b</i><sub class="lower-index"><i>i</i>, <i>m</i><sub class="lower-index"><i>i</i></sub></sub></span> (here the total length of the blocks <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, 1</sub> + <i>b</i><sub class="lower-index"><i>i</i>, 2</sub> + ... + <i>b</i><sub class="lower-index"><i>i</i>, <i>m</i><sub class="lower-index"><i>i</i></sub></sub></span> is equal to the length of the file <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>), and after that all blocks are transferred through the network, maintaining the order of files in the archive.</p><p>Zhorik thinks that the two messages contain the same archive, because their total lengths are equal. However, each file can be split in blocks in different ways in the two messages.</p><p>You are given the lengths of blocks in each of the two messages. Help Zhorik to determine what is the maximum number of files could be in the archive, if the Zhorik's assumption is correct.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of blocks in the first and in the second messages.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the blocks that form the first message.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the blocks that form the second message.</p><p>It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + ... + <i>x</i><sub class="lower-index"><i>n</i></sub> = <i>y</i><sub class="lower-index">1</sub> + ... + <i>y</i><sub class="lower-index"><i>m</i></sub></span>. <span class="tex-font-style-bf">Also, it is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + ... + <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>.</span></p></div><div class="output-specification"><p>Print the maximum number of files the intercepted array could consist of.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of blocks in the first and in the second messages.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the blocks that form the first message.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the blocks that form the second message.</p><p>It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + ... + <i>x</i><sub class="lower-index"><i>n</i></sub> = <i>y</i><sub class="lower-index">1</sub> + ... + <i>y</i><sub class="lower-index"><i>m</i></sub></span>. <span class="tex-font-style-bf">Also, it is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + ... + <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>.</span></p>

## Output

<p>Print the maximum number of files the intercepted array could consist of.</p>





```input1
7 6
2 5 3 1 11 4 4
7 8 2 4 1 8

```




```input2
3 3
1 10 100
1 100 10

```




```input3
1 4
4
1 1 1 1

```




```output1
3

```




```output2
2

```




```output3
1

```



## Note

<p>In the first example the maximum number of files in the archive is 3. For example, it is possible that in the archive are three files of sizes <span class="tex-span">2 + 5 = 7</span>, <span class="tex-span">15 = 3 + 1 + 11 = 8 + 2 + 4 + 1</span> and <span class="tex-span">4 + 4 = 8</span>.</p><p>In the second example it is possible that the archive contains two files of sizes <span class="tex-span">1</span> and <span class="tex-span">110 = 10 + 100 = 100 + 10</span>. Note that the order of files is kept while transferring archives through the network, so we can't say that there are three files of sizes <span class="tex-span">1</span>, <span class="tex-span">10</span> and <span class="tex-span">100</span>.</p><p>In the third example the only possibility is that the archive contains a single file of size <span class="tex-span">4</span>.</p>
