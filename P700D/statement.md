## Description

<div><p>Alice wants to send an important message to Bob. Message <span class="tex-span"><i>a</i> = (<i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> is a sequence of positive integers (<span class="tex-font-style-it">characters</span>).</p><p>To compress the message Alice wants to use binary Huffman coding. We recall that <span class="tex-font-style-it">binary Huffman code</span>, or <span class="tex-font-style-it">binary prefix code</span> is a function <span class="tex-span"><i>f</i></span>, that maps each letter that appears in the string to some binary string (that is, string consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only) such that for each pair of different characters <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> string <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>)</span> is not a prefix of <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>j</i></sub>)</span> (and vice versa). The result of the encoding of the message <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is the concatenation of the encoding of each character, that is the string <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index">1</sub>)<i>f</i>(<i>a</i><sub class="lower-index">2</sub>)... <i>f</i>(<i>a</i><sub class="lower-index"><i>n</i></sub>)</span>. Huffman codes are very useful, as the compressed message can be easily and uniquely decompressed, if the function <span class="tex-span"><i>f</i></span> is given. Code is usually chosen in order to minimize the total length of the compressed message, i.e. the length of the string <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index">1</sub>)<i>f</i>(<i>a</i><sub class="lower-index">2</sub>)... <i>f</i>(<i>a</i><sub class="lower-index"><i>n</i></sub>)</span>.</p><p>Because of security issues Alice doesn't want to send the whole message. Instead, she picks some substrings of the message and wants to send them separately. For each of the given substrings <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>... <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span> she wants to know the minimum possible length of the Huffman coding. Help her solve this problem.</p></div><div class="input-specification"><p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the initial message. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— characters of the message.</p><p>Next line contains the single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries.</p><p>Then follow <span class="tex-span"><i>q</i></span> lines with queries descriptions. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the position of the left and right ends of the <span class="tex-span"><i>i</i></span>-th substring respectively. Positions are numbered from <span class="tex-span">1</span>. Substrings may overlap in any way. The same substring may appear in the input more than once.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. Each line should contain a single integer&nbsp;— the minimum possible length of the Huffman encoding of the substring <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>... <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p></div>

## Input

<p>The first line of the input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the initial message. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— characters of the message.</p><p>Next line contains the single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries.</p><p>Then follow <span class="tex-span"><i>q</i></span> lines with queries descriptions. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the position of the left and right ends of the <span class="tex-span"><i>i</i></span>-th substring respectively. Positions are numbered from <span class="tex-span">1</span>. Substrings may overlap in any way. The same substring may appear in the input more than once.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. Each line should contain a single integer&nbsp;— the minimum possible length of the Huffman encoding of the substring <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>... <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p>





```input1
7
1 2 1 3 1 2 1
5
1 7
1 3
3 5
2 4
4 4

```




```output1
10
3
3
5
0

```



## Note

<p>In the first query, one of the optimal ways to encode the substring is to map <span class="tex-span">1</span> to "<span class="tex-font-style-tt">0</span>", <span class="tex-span">2</span> to "<span class="tex-font-style-tt">10</span>" and <span class="tex-span">3</span> to "<span class="tex-font-style-tt">11</span>".</p><p>Note that it is correct to map the letter to the empty substring (as in the fifth query from the sample).</p>
