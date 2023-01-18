## Description

<div><p>The prehistoric caves of El Toll are located in Moià (Barcelona). You have heard that there is a treasure hidden in one of <span class="tex-span"><i>n</i></span> possible spots in the caves. You assume that each of the spots has probability <span class="tex-span">1 / <i>n</i></span> to contain a treasure.</p><p>You cannot get into the caves yourself, so you have constructed a robot that can search the caves for treasure. Each day you can instruct the robot to visit exactly <span class="tex-span"><i>k</i></span> distinct spots in the caves. If none of these spots contain treasure, then the robot will obviously return with empty hands. However, the caves are dark, and the robot may miss the treasure even when visiting the right spot. Formally, if one of the visited spots does contain a treasure, the robot will obtain it with probability <span class="tex-span">1 / 2</span>, otherwise it will return empty. Each time the robot searches the spot with the treasure, his success probability is independent of all previous tries (that is, the probability to miss the treasure after searching the right spot <span class="tex-span"><i>x</i></span> times is <span class="tex-span">1 / 2<sup class="upper-index"><i>x</i></sup></span>).</p><p>What is the expected number of days it will take to obtain the treasure if you choose optimal scheduling for the robot? Output the answer as a rational number modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Formally, let the answer be an irreducible fraction <span class="tex-span"><i>P</i> / <i>Q</i></span>, then you have to output <img align="middle" class="tex-formula" src="file://qsGmitYb.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that <span class="tex-span"><i>Q</i></span> is not divisible by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains the number of test cases <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 1000</span>).</p><p>Each of the next <span class="tex-span"><i>T</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">8</sup></span>).</p></div><div class="output-specification"><p>For each test case output the answer in a separate line.</p></div>

## Input

<p>The first line contains the number of test cases <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 1000</span>).</p><p>Each of the next <span class="tex-span"><i>T</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">8</sup></span>).</p>

## Output

<p>For each test case output the answer in a separate line.</p>





```input1
3
1 1
2 1
3 2

```




```output1
2
500000007
777777786

```



## Note

<p>In the first case the robot will repeatedly search in the only spot. The expected number of days in this case is 2. Note that in spite of the fact that we know the treasure spot from the start, the robot still has to search there until he succesfully recovers the treasure.</p><p>In the second case the answer can be shown to be equal to <span class="tex-span">7 / 2</span> if we search the two spots alternatively. In the third case the answer is <span class="tex-span">25 / 9</span>.</p>
