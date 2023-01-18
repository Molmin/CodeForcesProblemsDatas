## Description

<div><p>There are <span class="tex-span"><i>n</i></span> people taking part in auction today. The rules of auction are classical. There were <span class="tex-span"><i>n</i></span> bids made, though it's not guaranteed they were from different people. It might happen that some people made no bids at all.</p><p>Each bid is define by two integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the index of the person, who made this bid and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is its size. Bids are given in chronological order, meaning <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i> &lt; <i>n</i></span>. Moreover, participant never makes two bids in a row (no one updates his own bid), i.e. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i> &lt; <i>n</i></span>.</p><p>Now you are curious with the following question: who (and which bid) will win the auction if some participants were absent? Consider that if someone was absent, all his bids are just removed and no new bids are added.</p><p>Note, that if during this imaginary exclusion of some participants it happens that some of the remaining participants makes a bid twice (or more times) in a row, only first of these bids is counted. For better understanding take a look at the samples.</p><p>You have several questions in your mind, compute the answer for each of them.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of participants and bids.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i> + 1</sub></span>)&nbsp;— the number of participant who made the <span class="tex-span"><i>i</i></span>-th bid and the size of this bid.</p><p>Next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of question you have in mind.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), followed by <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of people who are not coming in this question and their indices. It is guarenteed that <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> values are different for a single question.</p><p>It's guaranteed that the sum of <span class="tex-span"><i>k</i></span> over all question won't exceed <span class="tex-span">200 000</span>.</p></div><div class="output-specification"><p>For each question print two integer&nbsp;— the index of the winner and the size of the winning bid. If there is no winner (there are no remaining bids at all), print two zeroes.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of participants and bids.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i> + 1</sub></span>)&nbsp;— the number of participant who made the <span class="tex-span"><i>i</i></span>-th bid and the size of this bid.</p><p>Next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of question you have in mind.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), followed by <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of people who are not coming in this question and their indices. It is guarenteed that <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> values are different for a single question.</p><p>It's guaranteed that the sum of <span class="tex-span"><i>k</i></span> over all question won't exceed <span class="tex-span">200 000</span>.</p>

## Output

<p>For each question print two integer&nbsp;— the index of the winner and the size of the winning bid. If there is no winner (there are no remaining bids at all), print two zeroes.</p>





```input1
6
1 10
2 100
3 1000
1 10000
2 100000
3 1000000
3
1 3
2 2 3
2 1 2

```




```input2
3
1 10
2 100
1 1000
2
2 1 2
2 2 3

```




```output1
2 100000
1 10
3 1000

```




```output2
0 0
1 10

```



## Note

<p>Consider the first sample: </p><ul> <li> In the first question participant number <span class="tex-span">3</span> is absent so the sequence of bids looks as follows: <ol> <li> <span class="tex-span">1</span> <span class="tex-span">10</span> </li><li> <span class="tex-span">2</span> <span class="tex-span">100</span> </li><li> <span class="tex-span">1</span> <span class="tex-span">10 000</span> </li><li> <span class="tex-span">2</span> <span class="tex-span">100 000</span> </li></ol> Participant number <span class="tex-span">2</span> wins with the bid <span class="tex-span">100 000</span>.</li><li> In the second question participants <span class="tex-span">2</span> and <span class="tex-span">3</span> are absent, so the sequence of bids looks: <ol> <li> <span class="tex-span">1</span> <span class="tex-span">10</span> </li><li> <span class="tex-span">1</span> <span class="tex-span">10 000</span> </li></ol> The winner is, of course, participant number <span class="tex-span">1</span> but the winning bid is <span class="tex-span">10</span> instead of <span class="tex-span">10 000</span> as no one will ever increase his own bid (in this problem). </li><li> In the third question participants <span class="tex-span">1</span> and <span class="tex-span">2</span> are absent and the sequence is: <ol> <li> <span class="tex-span">3</span> <span class="tex-span">1 000</span> </li><li> <span class="tex-span">3</span> <span class="tex-span">1 000 000</span> </li></ol> The winner is participant <span class="tex-span">3</span> with the bid <span class="tex-span">1 000</span>. </li></ul>
