## Description

<div><p>As you know, Vova has recently become a new shaman in the city of Ultima Thule. So, he has received the shaman knowledge about the correct bracket sequences. The shamans of Ultima Thule have been using lots of different types of brackets since prehistoric times. A bracket type is a positive integer. The shamans define a correct bracket sequence as follows:</p><ul> <li> An empty sequence is a correct bracket sequence. </li><li> If <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i></sub>}</span> and <span class="tex-span">{<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub>}</span> are correct bracket sequences, then sequence <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i></sub>, <i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub>}</span> (their concatenation) also is a correct bracket sequence. </li><li> If <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i></sub>}</span> — is a correct bracket sequence, then sequence <img align="middle" class="tex-formula" src="file://qfkMgsuq.png" style="max-width: 100.0%;max-height: 100.0%;"> also is a correct bracket sequence, where <span class="tex-span"><i>v</i></span> <span class="tex-span">(<i>v</i> &gt; 0)</span> is an integer. </li></ul><p>For example, sequences <span class="tex-span">{1, 1,  - 1, 2,  - 2,  - 1}</span> and <span class="tex-span">{3,  - 3}</span> are correct bracket sequences, and <span class="tex-span">{2,  - 3}</span> is not.</p><p>Moreover, after Vova became a shaman, he learned the <span class="tex-font-style-it">most important</span> correct bracket sequence <span class="tex-span">{<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>}</span>, consisting of <span class="tex-span"><i>n</i></span> integers. As sequence <span class="tex-span"><i>x</i></span> is the most important, Vova decided to encrypt it just in case.</p><p>Encrypting consists of two sequences. The first sequence <span class="tex-span">{<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>}</span> contains types of brackets, that is, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = |<i>x</i><sub class="lower-index"><i>i</i></sub>|</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). The second sequence <span class="tex-span">{<i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>t</i></sub>}</span> contains <span class="tex-span"><i>t</i></span> integers — <span class="tex-font-style-bf">some positions</span> (possibly, not all of them), which had negative numbers in sequence <span class="tex-span">{<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>}</span>.</p><p>Unfortunately, Vova forgot the main sequence. But he was lucky enough to keep the encryption: sequences <span class="tex-span">{<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>}</span> and <span class="tex-span">{<i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>t</i></sub>}</span>. Help Vova restore sequence <span class="tex-span"><i>x</i></span> by the encryption. If there are multiple sequences that correspond to the encryption, restore any of them. If there are no such sequences, you should tell so.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The third line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>), followed by <span class="tex-span"><i>t</i></span> distinct integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>t</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>The numbers in each line are separated by spaces.</p></div><div class="output-specification"><p>Print a single string "<span class="tex-font-style-tt">NO</span>" (without the quotes) if Vova is mistaken and a suitable sequence <span class="tex-span">{<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>}</span> doesn't exist.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) and in the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| = <i>p</i><sub class="lower-index"><i>i</i></sub>;&nbsp;<i>x</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>j</i></sub></sub> &lt; 0)</span>. If there are multiple sequences that correspond to the encrypting, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The third line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>), followed by <span class="tex-span"><i>t</i></span> distinct integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>t</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>The numbers in each line are separated by spaces.</p>

## Output

<p>Print a single string "<span class="tex-font-style-tt">NO</span>" (without the quotes) if Vova is mistaken and a suitable sequence <span class="tex-span">{<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>}</span> doesn't exist.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) and in the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| = <i>p</i><sub class="lower-index"><i>i</i></sub>;&nbsp;<i>x</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>j</i></sub></sub> &lt; 0)</span>. If there are multiple sequences that correspond to the encrypting, you are allowed to print any of them.</p>





```input1
2
1 1
0

```




```input2
4
1 1 1 1
1 3

```




```input3
3
1 1 1
0

```




```input4
4
1 2 2 1
2 3 4

```




```output1
YES
1 -1

```




```output2
YES
1 1 -1 -1

```




```output3
NO

```




```output4
YES
1 2 -2 -1

```


