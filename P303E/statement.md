## Description

<div><p>Imagine a real contest or exam of <span class="tex-span"><i>n</i></span> participants. Every participant will get a particular score. We can predict the standings board more or less, if we do some statistics on their previous performance.</p><center> <img class="tex-graphics" src="file://s6tYleUb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let's say the score of the participants will be uniformly distributed in interval <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> (the score can be a real number). Can you predict the standings board according to these data? In other words you should say for each participant the probability that he gets some fixed place in the scoreboard. <span class="tex-font-style-bf">The participants are sorted by increasing of their scores in the scoreboard. So, the participant with the largest score gets the last place.</span></p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤ <i>n</i>  ≤ 80</span>), showing how many participants we have. Each of the next <span class="tex-span"><i>n</i></span> lines contains our predictions, the <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> as the distributed interval for participant <span class="tex-span"><i>i</i></span>.</p><p>Consider the participants numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some way.</p></div><div class="output-specification"><p>Output a distributed matrix <span class="tex-span"><i>a</i></span> of order <span class="tex-span"><i>n</i></span>. The element <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> of the matrix is the probability that participant <span class="tex-span"><i>i</i></span> has rank <span class="tex-span"><i>j</i></span>.</p><p>Your answer will considered correct if it has at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> absolute or relative error.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤ <i>n</i>  ≤ 80</span>), showing how many participants we have. Each of the next <span class="tex-span"><i>n</i></span> lines contains our predictions, the <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> as the distributed interval for participant <span class="tex-span"><i>i</i></span>.</p><p>Consider the participants numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some way.</p>

## Output

<p>Output a distributed matrix <span class="tex-span"><i>a</i></span> of order <span class="tex-span"><i>n</i></span>. The element <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> of the matrix is the probability that participant <span class="tex-span"><i>i</i></span> has rank <span class="tex-span"><i>j</i></span>.</p><p>Your answer will considered correct if it has at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> absolute or relative error.</p>





```input1
2
1 6
4 9

```




```input2
8
0 2
1 3
2 4
3 5
4 6
5 7
6 8
7 9

```




```output1
0.9200000000 0.080 
0.080 0.9200000000 

```




```output2
0.875 0.125 0 0 0 0 0 0 
0.125 0.750 0.125 0 0 0 0 0 
0 0.125 0.750 0.125 0 0 0 0 
0 0 0.125 0.750 0.125 0 0 0 
0 0 0 0.125 0.750 0.125 0 0 
0 0 0 0 0.125 0.750 0.125 0 
0 0 0 0 0 0.125 0.750 0.125 
0 0 0 0 0 0 0.125 0.875 

```



## Note

<p>The score probability distribution is continuous, which means, there is no possibility for a draw.</p>
