## Description

<div><p>Each employee of the "Blake Techologies" company uses a special messaging app "Blake Messenger". All the stuff likes this app and uses it constantly. However, some important futures are missing. For example, many users want to be able to search through the message history. It was already announced that the new feature will appear in the nearest update, when developers faced some troubles that only you may help them to solve.</p><p>All the messages are represented as a strings consisting of only lowercase English letters. In order to reduce the network load strings are represented in the special compressed form. Compression algorithm works as follows: string is represented as a concatenation of <span class="tex-span"><i>n</i></span> blocks, each block containing only equal characters. One block may be described as a pair <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is the length of the <span class="tex-span"><i>i</i></span>-th block and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the corresponding letter. Thus, the string <span class="tex-span"><i>s</i></span> may be written as the sequence of pairs <img align="middle" class="tex-formula" src="file://B6VkE7zg.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Your task is to write the program, that given two compressed string <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>s</i></span> finds all occurrences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span>. Developers know that there may be many such occurrences, so they only ask you to find the <span class="tex-font-style-bf">number</span> of them. Note that <span class="tex-span"><i>p</i></span> is the starting position of some occurrence of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span> if and only if <span class="tex-span"><i>t</i><sub class="lower-index"><i>p</i></sub><i>t</i><sub class="lower-index"><i>p</i> + 1</sub>...<i>t</i><sub class="lower-index"><i>p</i> + |<i>s</i>| - 1</sub> = <i>s</i></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th character of string <span class="tex-span"><i>t</i></span>.</p><p>Note that the way to represent the string in compressed form may not be unique. For example string "<span class="tex-font-style-tt">aaaa</span>" may be given as <img align="middle" class="tex-formula" src="file://mzjO9BTG.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://w583xXDg.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://RZ59GOA4.png" style="max-width: 100.0%;max-height: 100.0%;">...</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the number of blocks in the strings <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>s</i></span>, respectively.</p><p>The second line contains the descriptions of <span class="tex-span"><i>n</i></span> parts of string <span class="tex-span"><i>t</i></span> in the format "<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the length of the <span class="tex-span"><i>i</i></span>-th part and the corresponding lowercase English letter.</p><p>The second line contains the descriptions of <span class="tex-span"><i>m</i></span> parts of string <span class="tex-span"><i>s</i></span> in the format "<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the length of the <span class="tex-span"><i>i</i></span>-th part and the corresponding lowercase English letter.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of occurrences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the number of blocks in the strings <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>s</i></span>, respectively.</p><p>The second line contains the descriptions of <span class="tex-span"><i>n</i></span> parts of string <span class="tex-span"><i>t</i></span> in the format "<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the length of the <span class="tex-span"><i>i</i></span>-th part and the corresponding lowercase English letter.</p><p>The second line contains the descriptions of <span class="tex-span"><i>m</i></span> parts of string <span class="tex-span"><i>s</i></span> in the format "<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the length of the <span class="tex-span"><i>i</i></span>-th part and the corresponding lowercase English letter.</p>

## Output

<p>Print a single integer&nbsp;— the number of occurrences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span>.</p>





```input1
5 3
3-a 2-b 4-c 3-a 2-c
2-a 2-b 1-c

```




```input2
6 1
3-a 6-b 7-a 4-c 8-e 2-a
3-a

```




```input3
5 5
1-h 1-e 1-l 1-l 1-o
1-w 1-o 1-r 1-l 1-d

```




```output1
1
```




```output2
6
```




```output3
0
```



## Note

<p>In the first sample, <span class="tex-span"><i>t</i></span> = "<span class="tex-font-style-tt">aaabbccccaaacc</span>", and string <span class="tex-span"><i>s</i></span> = "<span class="tex-font-style-tt">aabbc</span>". The only occurrence of string <span class="tex-span"><i>s</i></span> in string <span class="tex-span"><i>t</i></span> starts at position <span class="tex-span"><i>p</i> = 2</span>.</p><p>In the second sample, <span class="tex-span"><i>t</i></span> = "<span class="tex-font-style-tt">aaabbbbbbaaaaaaacccceeeeeeeeaa</span>", and <span class="tex-span"><i>s</i></span> = "<span class="tex-font-style-tt">aaa</span>". The occurrences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span> start at positions <span class="tex-span"><i>p</i> = 1</span>, <span class="tex-span"><i>p</i> = 10</span>, <span class="tex-span"><i>p</i> = 11</span>, <span class="tex-span"><i>p</i> = 12</span>, <span class="tex-span"><i>p</i> = 13</span> and <span class="tex-span"><i>p</i> = 14</span>.</p>
