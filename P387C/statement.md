## Description

<div><p>George is a cat, so he really likes to play. Most of all he likes to play with his array of positive integers <span class="tex-span"><i>b</i></span>. During the game, George modifies the array by using special changes. Let's mark George's current array as <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index">|<i>b</i>|</sub></span> (record <span class="tex-span">|<i>b</i>|</span> denotes the current length of the array). Then one change is a sequence of actions: </p><ul> <li> Choose two distinct indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ |<i>b</i>|;&nbsp;<i>i</i> ≠ <i>j</i>)</span>, such that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≥ <i>b</i><sub class="lower-index"><i>j</i></sub></span>. </li><li> Get number <span class="tex-span"><i>v</i> = <i>concat</i>(<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>)</span>, where <span class="tex-span"><i>concat</i>(<i>x</i>, <i>y</i>)</span> is a number obtained by adding number <span class="tex-span"><i>y</i></span> to the end of the decimal record of number <span class="tex-span"><i>x</i></span>. For example, <span class="tex-span"><i>concat</i>(500, 10) = 50010</span>, <span class="tex-span"><i>concat</i>(2, 2) = 22</span>. </li><li> Add number <span class="tex-span"><i>v</i></span> to the end of the array. The length of the array will increase by one. </li><li> Remove from the array numbers with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. The length of the array will decrease by two, and elements of the array will become re-numbered from <span class="tex-span">1</span> to current length of the array. </li></ul><p>George played for a long time with his array <span class="tex-span"><i>b</i></span> and received from array <span class="tex-span"><i>b</i></span> an array consisting of exactly one number <span class="tex-span"><i>p</i></span>. Now George wants to know: what is the maximum number of elements array <span class="tex-span"><i>b</i></span> could contain originally? Help him find this number. Note that originally the array could contain only <span class="tex-font-style-bf">positive</span> integers.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> &lt; 10<sup class="upper-index">100000</sup></span>). It is guaranteed that number <span class="tex-span"><i>p</i></span> doesn't contain any leading zeroes.</p></div><div class="output-specification"><p>Print an integer — the maximum number of elements array <span class="tex-span"><i>b</i></span> could contain originally.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> &lt; 10<sup class="upper-index">100000</sup></span>). It is guaranteed that number <span class="tex-span"><i>p</i></span> doesn't contain any leading zeroes.</p>

## Output

<p>Print an integer — the maximum number of elements array <span class="tex-span"><i>b</i></span> could contain originally.</p>





```input1
9555

```




```input2
10000000005

```




```input3
800101

```




```input4
45

```




```input5
1000000000000001223300003342220044555

```




```input6
19992000

```




```input7
310200

```




```output1
4
```




```output2
2
```




```output3
3
```




```output4
1
```




```output5
17
```




```output6
1
```




```output7
2
```



## Note

<p>Let's consider the test examples: </p><ul> <li> Originally array <span class="tex-span"><i>b</i></span> can be equal to <span class="tex-span">{5, 9, 5, 5}</span>. The sequence of George's changes could have been: <span class="tex-span">{5, 9, 5, 5} → {5, 5, 95} → {95, 55} → {9555}</span>. </li><li> Originally array <span class="tex-span"><i>b</i></span> could be equal to <span class="tex-span">{1000000000, 5}</span>. Please note that the array <span class="tex-span"><i>b</i></span> cannot contain zeros. </li><li> Originally array <span class="tex-span"><i>b</i></span> could be equal to <span class="tex-span">{800, 10, 1}</span>. </li><li> Originally array <span class="tex-span"><i>b</i></span> could be equal to <span class="tex-span">{45}</span>. It cannot be equal to <span class="tex-span">{4, 5}</span>, because George can get only array <span class="tex-span">{54}</span> from this array in one operation. </li></ul><p>Note that the numbers can be very large.</p>
