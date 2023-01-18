## Description

<div><p>Many of you must be familiar with the Google Code Jam round rules. Let us remind you of some key moments that are crucial to solving this problem. During the round, the participants are suggested to solve several problems, each divided into two subproblems: an easy one with small limits (Small input), and a hard one with large limits (Large input). You can submit a solution for Large input only after you've solved the Small input for this problem. There are no other restrictions on the order of solving inputs. In particular, the participant can first solve the Small input, then switch to another problem, and then return to the Large input. Solving each input gives the participant some number of points (usually different for each problem). This takes into account only complete solutions that work correctly on all tests of the input. The participant gets the test result of a Small input right after he submits it, but the test result of a Large input are out only after the round's over. In the final results table the participants are sorted by non-increasing of received points. If the points are equal, the participants are sorted by ascending of time penalty. By the Google Code Jam rules the time penalty is the <span class="tex-font-style-bf">time when the last correct solution was submitted</span>.</p><p>Vasya decided to check out a new tactics on another round. As soon as the round begins, the boy quickly read all the problems and accurately evaluated the time it takes to solve them. Specifically, for each one of the <span class="tex-span"><i>n</i></span> problems Vasya knows five values:</p><ul><li> Solving the Small input of the <span class="tex-span"><i>i</i></span>-th problem gives to the participant <span class="tex-span"><i>scoreSmall</i><sub class="lower-index"><i>i</i></sub></span> points, and solving the Large input gives <span class="tex-span"><i>scoreLarge</i><sub class="lower-index"><i>i</i></sub></span> more points. That is, the maximum number of points you can get for the <span class="tex-span"><i>i</i></span>-th problem equals <span class="tex-span"><i>scoreSmall</i><sub class="lower-index"><i>i</i></sub> + <i>scoreLarge</i><sub class="lower-index"><i>i</i></sub></span>.</li><li> Writing the solution for the Small input of the <span class="tex-span"><i>i</i></span>-th problem takes exactly <span class="tex-span"><i>timeSmall</i><sub class="lower-index"><i>i</i></sub></span> minutes for Vasya. Improving this code and turning it into the solution of the Large input takes another <span class="tex-span"><i>timeLarge</i><sub class="lower-index"><i>i</i></sub></span> minutes.</li><li> Vasya's had much practice, so he solves all Small inputs from the first attempt. But it's not so easy with the Large input: there is the <span class="tex-span"><i>probFail</i><sub class="lower-index"><i>i</i></sub></span> probability that the solution to the Large input will turn out to be wrong at the end of the round. Please keep in mind that these solutions do not affect the participants' points and the time penalty.</li></ul><p>A round lasts for <span class="tex-span"><i>t</i></span> minutes. The time for reading problems and submitting solutions can be considered to equal zero. Vasya is allowed to submit a solution exactly at the moment when the round ends.</p><p>Vasya wants to choose a set of inputs and the order of their solution so as to make the expectation of the total received points maximum possible. If there are multiple ways to do this, he needs to minimize the expectation of the time penalty. Help Vasya to cope with this problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>t</i> ≤ 1560</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing 5 numbers: <span class="tex-span"><i>scoreSmall</i><sub class="lower-index"><i>i</i></sub>, <i>scoreLarge</i><sub class="lower-index"><i>i</i></sub>, <i>timeSmall</i><sub class="lower-index"><i>i</i></sub>, <i>timeLarge</i><sub class="lower-index"><i>i</i></sub>, <i>probFail</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>scoreSmall</i><sub class="lower-index"><i>i</i></sub>, <i>scoreLarge</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>timeSmall</i><sub class="lower-index"><i>i</i></sub>, <i>timeLarge</i><sub class="lower-index"><i>i</i></sub> ≤ 1560, 0 ≤ <i>probFail</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>).</p><p><span class="tex-span"><i>probFail</i><sub class="lower-index"><i>i</i></sub></span> are real numbers, given with at most 6 digits after the decimal point. All other numbers in the input are integers.</p></div><div class="output-specification"><p>Print two real numbers — the maximum expectation of the total points and the corresponding minimum possible time penalty expectation. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>t</i> ≤ 1560</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing 5 numbers: <span class="tex-span"><i>scoreSmall</i><sub class="lower-index"><i>i</i></sub>, <i>scoreLarge</i><sub class="lower-index"><i>i</i></sub>, <i>timeSmall</i><sub class="lower-index"><i>i</i></sub>, <i>timeLarge</i><sub class="lower-index"><i>i</i></sub>, <i>probFail</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>scoreSmall</i><sub class="lower-index"><i>i</i></sub>, <i>scoreLarge</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>timeSmall</i><sub class="lower-index"><i>i</i></sub>, <i>timeLarge</i><sub class="lower-index"><i>i</i></sub> ≤ 1560, 0 ≤ <i>probFail</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>).</p><p><span class="tex-span"><i>probFail</i><sub class="lower-index"><i>i</i></sub></span> are real numbers, given with at most 6 digits after the decimal point. All other numbers in the input are integers.</p>

## Output

<p>Print two real numbers — the maximum expectation of the total points and the corresponding minimum possible time penalty expectation. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3 40
10 20 15 4 0.5
4 100 21 1 0.99
1 4 1 1 0.25

```




```input2
1 1
100000000 200000000 1 1 0

```




```output1
24.0 18.875

```




```output2
100000000 1

```



## Note

<p>In the first sample one of the optimal orders of solving problems is:</p><ol><li> The Small input of the third problem. </li><li> The Small input of the first problem. </li><li> The Large input of the third problem. </li><li> The Large input of the first problem.</li></ol><p>Note that if you solve the Small input of the second problem instead of two inputs of the third one, then total score expectation will be the same but the time penalty expectation will be worse (<span class="tex-span">38</span>).</p>
