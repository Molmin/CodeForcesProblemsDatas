## Description

<div><p>Yash is finally tired of computing the length of the longest Fibonacci-ish sequence. He now plays around with more complex things such as Fibonacci-ish potentials. </p><p>Fibonacci-ish potential of an array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is computed as follows: </p><ol> <li> Remove all elements <span class="tex-span"><i>j</i></span> if there exists <span class="tex-span"><i>i</i> &lt; <i>j</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub></span>. </li><li> Sort the remaining elements in ascending order, i.e. <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </li><li> Compute the potential as <span class="tex-span"><i>P</i>(<i>a</i>) = <i>a</i><sub class="lower-index">1</sub>·<i>F</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub>·<i>F</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub>·<i>F</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th Fibonacci number (see notes for clarification). </li></ol><p>You are given an array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> ranges from <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>. For each range <span class="tex-span"><i>j</i></span> you have to compute the Fibonacci-ish potential of the array <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, composed using all elements of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> inclusive. Find these potentials modulo <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains integers of <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30 000</span>)&nbsp;— the length of the initial array and the modulo, respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p><p>Then follow the number of ranges <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 30 000</span>).</p><p>Last <span class="tex-span"><i>q</i></span> lines contain pairs of indices <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— ranges to compute Fibonacci-ish potentials.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines, <span class="tex-span"><i>i</i></span>-th of them must contain the Fibonacci-ish potential of the <span class="tex-span"><i>i</i></span>-th range modulo <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line of the input contains integers of <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30 000</span>)&nbsp;— the length of the initial array and the modulo, respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— elements of the array.</p><p>Then follow the number of ranges <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 30 000</span>).</p><p>Last <span class="tex-span"><i>q</i></span> lines contain pairs of indices <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— ranges to compute Fibonacci-ish potentials.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines, <span class="tex-span"><i>i</i></span>-th of them must contain the Fibonacci-ish potential of the <span class="tex-span"><i>i</i></span>-th range modulo <span class="tex-span"><i>m</i></span>.</p>





```input1
5 10
2 1 2 1 2
2
2 4
4 5

```




```output1
3
3

```



## Note

<p>For the purpose of this problem define Fibonacci numbers as follows: </p><ol> <li> <span class="tex-span"><i>F</i><sub class="lower-index">1</sub> = <i>F</i><sub class="lower-index">2</sub> = 1</span>. </li><li> <span class="tex-span"><i>F</i><sub class="lower-index"><i>n</i></sub> = <i>F</i><sub class="lower-index"><i>n</i> - 1</sub> + <i>F</i><sub class="lower-index"><i>n</i> - 2</sub></span> for each <span class="tex-span"><i>n</i> &gt; 2</span>. </li></ol><p>In the first query, the subarray [1,2,1] can be formed using the minimal set {1,2}. Thus, the potential of this subarray is 1*1+2*1=3.</p>
