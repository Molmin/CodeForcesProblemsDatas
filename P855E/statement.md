## Description

<div><p>Harry came to know from Dumbledore that Salazar Slytherin's locket is a horcrux. This locket was present earlier at 12 Grimmauld Place, the home of Sirius Black's mother. It was stolen from there and is now present in the Ministry of Magic in the office of Dolorous Umbridge, Harry's former Defense Against the Dark Arts teacher. </p><p>Harry, Ron and Hermione are infiltrating the Ministry. Upon reaching Umbridge's office, they observed a code lock with a puzzle asking them to calculate count of magic numbers between two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (both inclusive). </p><p>Harry remembered from his detention time with Umbridge that she defined a magic number as a number which when converted to a given base <span class="tex-span"><i>b</i></span>, all the digits from <span class="tex-span">0</span> to <span class="tex-span"><i>b</i> - 1</span> appear even number of times in its representation without any leading zeros.</p><p>You have to answer <span class="tex-span"><i>q</i></span> queries to unlock the office. Each query has three integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, the base and the range for which you have to find the count of magic numbers.</p></div><div class="input-specification"><p>First line of input contains <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— number of queries.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain three space separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>You have to output <span class="tex-span"><i>q</i></span> lines, each containing a single integer, the answer to the corresponding query.</p></div>

## Input

<p>First line of input contains <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— number of queries.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain three space separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>You have to output <span class="tex-span"><i>q</i></span> lines, each containing a single integer, the answer to the corresponding query.</p>





```input1
2
2 4 9
3 1 10

```




```input2
2
2 1 100
5 1 100

```




```output1
1
2

```




```output2
21
4

```



## Note

<p>In sample test case <span class="tex-span">1</span>, for first query, when we convert numbers <span class="tex-span">4</span> to <span class="tex-span">9</span> into base <span class="tex-span">2</span>, we get: </p><ul> <li> <span class="tex-span">4 = 100<sub class="lower-index">2</sub></span>, </li><li> <span class="tex-span">5 = 101<sub class="lower-index">2</sub></span>, </li><li> <span class="tex-span">6 = 110<sub class="lower-index">2</sub></span>, </li><li> <span class="tex-span">7 = 111<sub class="lower-index">2</sub></span>, </li><li> <span class="tex-span">8 = 1000<sub class="lower-index">2</sub></span>, </li><li> <span class="tex-span">9 = 1001<sub class="lower-index">2</sub></span>. </li></ul><p>Out of these, only base <span class="tex-span">2</span> representation of <span class="tex-span">9</span> has even number of <span class="tex-span">1</span> and <span class="tex-span">0</span>. Thus, the answer is <span class="tex-span">1</span>.</p>
