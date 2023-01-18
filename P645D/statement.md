## Description

<div><p>While Farmer John rebuilds his farm in an unfamiliar portion of Bovinia, Bessie is out trying some alternative jobs. In her new gig as a reporter, Bessie needs to know about programming competition results as quickly as possible. When she covers the 2016 Robot Rap Battle Tournament, she notices that all of the robots operate under deterministic algorithms. In particular, robot <span class="tex-span"><i>i</i></span> will beat robot <span class="tex-span"><i>j</i></span> if and only if robot <span class="tex-span"><i>i</i></span> has a higher skill level than robot <span class="tex-span"><i>j</i></span>. And if robot <span class="tex-span"><i>i</i></span> beats robot <span class="tex-span"><i>j</i></span> and robot <span class="tex-span"><i>j</i></span> beats robot <span class="tex-span"><i>k</i></span>, then robot <span class="tex-span"><i>i</i></span> will beat robot <span class="tex-span"><i>k</i></span>. Since rapping is such a subtle art, two robots can never have the same skill level.</p><p>Given the results of the rap battles in the order in which they were played, determine the <span class="tex-font-style-bf">minimum number</span> of first rap battles that needed to take place before Bessie could order all of the robots by skill level.</p></div><div class="input-specification"><p>The first line of the input consists of two integers, the number of robots <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) and the number of rap battles <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://b4gV09jz.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines describe the results of the rap battles in the order they took place. Each consists of two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), indicating that robot <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> beat robot <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the <span class="tex-span"><i>i</i></span>-th rap battle. No two rap battles involve the same pair of robots.</p><p>It is guaranteed that at least one ordering of the robots satisfies all <span class="tex-span"><i>m</i></span> relations.</p></div><div class="output-specification"><p>Print the minimum <span class="tex-span"><i>k</i></span> such that the ordering of the robots by skill level is uniquely defined by the first <span class="tex-span"><i>k</i></span> rap battles. If there exists more than one ordering that satisfies all <span class="tex-span"><i>m</i></span> relations, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input consists of two integers, the number of robots <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) and the number of rap battles <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://b4gV09jz.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines describe the results of the rap battles in the order they took place. Each consists of two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), indicating that robot <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> beat robot <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the <span class="tex-span"><i>i</i></span>-th rap battle. No two rap battles involve the same pair of robots.</p><p>It is guaranteed that at least one ordering of the robots satisfies all <span class="tex-span"><i>m</i></span> relations.</p>

## Output

<p>Print the minimum <span class="tex-span"><i>k</i></span> such that the ordering of the robots by skill level is uniquely defined by the first <span class="tex-span"><i>k</i></span> rap battles. If there exists more than one ordering that satisfies all <span class="tex-span"><i>m</i></span> relations, output <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 5
2 1
1 3
2 3
4 2
4 3

```




```input2
3 2
1 2
3 2

```




```output1
4

```




```output2
-1

```



## Note

<p>In the first sample, the robots from strongest to weakest must be <span class="tex-span">(4, 2, 1, 3)</span>, which Bessie can deduce after knowing the results of the first four rap battles.</p><p>In the second sample, both <span class="tex-span">(1, 3, 2)</span> and <span class="tex-span">(3, 1, 2)</span> are possible orderings of the robots from strongest to weakest after both rap battles.</p>
