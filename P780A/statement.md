## Description

<div><p>Andryusha is an orderly boy and likes to keep things in their place.</p><p>Today he faced a problem to put his socks in the wardrobe. He has <span class="tex-span"><i>n</i></span> distinct pairs of socks which are initially in a bag. The pairs are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Andryusha wants to put paired socks together and put them in the wardrobe. He takes the socks one by one from the bag, and for each sock he looks whether the pair of this sock has been already took out of the bag, or not. If not (that means the pair of this sock is still in the bag), he puts the current socks on the table in front of him. Otherwise, he puts both socks from the pair to the wardrobe.</p><p>Andryusha remembers the order in which he took the socks from the bag. Can you tell him what is the maximum number of socks that were on the table at the same time? </p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of sock pairs.</p><p>The second line contains <span class="tex-span">2<i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which describe the order in which Andryusha took the socks from the bag. More precisely, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th sock Andryusha took out was from pair <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that Andryusha took exactly two socks of each pair.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the maximum number of socks that were on the table at the same time.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of sock pairs.</p><p>The second line contains <span class="tex-span">2<i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which describe the order in which Andryusha took the socks from the bag. More precisely, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th sock Andryusha took out was from pair <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that Andryusha took exactly two socks of each pair.</p>

## Output

<p>Print single integer&nbsp;— the maximum number of socks that were on the table at the same time.</p>





```input1
1
1 1

```




```input2
3
2 1 1 3 2 3

```




```output1
1

```




```output2
2

```



## Note

<p>In the first example Andryusha took a sock from the first pair and put it on the table. Then he took the next sock which is from the first pair as well, so he immediately puts both socks to the wardrobe. Thus, at most one sock was on the table at the same time.</p><p>In the second example Andryusha behaved as follows: </p><ul> <li> Initially the table was empty, he took out a sock from pair <span class="tex-span">2</span> and put it on the table. </li><li> Sock <span class="tex-span">(2)</span> was on the table. Andryusha took out a sock from pair <span class="tex-span">1</span> and put it on the table. </li><li> Socks <span class="tex-span">(1, 2)</span> were on the table. Andryusha took out a sock from pair <span class="tex-span">1</span>, and put this pair into the wardrobe. </li><li> Sock <span class="tex-span">(2)</span> was on the table. Andryusha took out a sock from pair <span class="tex-span">3</span> and put it on the table. </li><li> Socks <span class="tex-span">(2, 3)</span> were on the table. Andryusha took out a sock from pair <span class="tex-span">2</span>, and put this pair into the wardrobe. </li><li> Sock <span class="tex-span">(3)</span> was on the table. Andryusha took out a sock from pair <span class="tex-span">3</span> and put this pair into the wardrobe. </li></ul> Thus, at most two socks were on the table at the same time.
