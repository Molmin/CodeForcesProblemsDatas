## Description

<div><p>This problem is the most boring one you've ever seen. </p><p>Given a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and a non-negative integer <span class="tex-span"><i>h</i></span>, our goal is to partition the sequence into two subsequences (not necessarily consist of continuous elements). Each element of the original sequence should be contained in exactly one of the result subsequences. Note, that one of the result subsequences can be empty.</p><p>Let's define function <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> on pairs of distinct elements (that is <span class="tex-span"><i>i</i> ≠ <i>j</i></span>) in the original sequence. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> are in the same subsequence in the current partition then <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>) = <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span> otherwise <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>) = <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub> + <i>h</i></span>. </p><p>Consider all possible values of the function <span class="tex-span"><i>f</i></span> for some partition. We'll call the <span class="tex-font-style-it">goodness</span> of this partiotion the difference between the maximum value of function <span class="tex-span"><i>f</i></span> and the minimum value of function <span class="tex-span"><i>f</i></span>.</p><p>Your task is to find a partition of the given sequence <span class="tex-span"><i>a</i></span> that have the minimal possible goodness among all possible partitions.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup>)</span>. In the second line there is a list of <span class="tex-span"><i>n</i></span> space-separated integers representing <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>.</p></div><div class="output-specification"><p>The first line of output should contain the required minimum goodness. </p><p>The second line describes the optimal partition. You should print <span class="tex-span"><i>n</i></span> whitespace-separated integers in the second line. The <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span">1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is in the first subsequence otherwise it should be <span class="tex-span">2</span>.</p><p>If there are several possible correct answers you are allowed to print any of them.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup>)</span>. In the second line there is a list of <span class="tex-span"><i>n</i></span> space-separated integers representing <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>.</p>

## Output

<p>The first line of output should contain the required minimum goodness. </p><p>The second line describes the optimal partition. You should print <span class="tex-span"><i>n</i></span> whitespace-separated integers in the second line. The <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span">1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is in the first subsequence otherwise it should be <span class="tex-span">2</span>.</p><p>If there are several possible correct answers you are allowed to print any of them.</p>





```input1
3 2
1 2 3

```




```input2
5 10
0 1 0 2 1

```




```output1
1
1 2 2 

```




```output2
3
2 2 2 2 2 

```



## Note

<p>In the first sample the values of <span class="tex-span"><i>f</i></span> are as follows: <span class="tex-span"><i>f</i>(1, 2) = 1 + 2 + 2 = 5</span>, <span class="tex-span"><i>f</i>(1, 3) = 1 + 3 + 2 = 6</span> and <span class="tex-span"><i>f</i>(2, 3) = 2 + 3 = 5</span>. So the difference between maximum and minimum values of <span class="tex-span"><i>f</i></span> is <span class="tex-span">1</span>.</p><p>In the second sample the value of <span class="tex-span"><i>h</i></span> is large, so it's better for one of the sub-sequences to be empty.</p>
