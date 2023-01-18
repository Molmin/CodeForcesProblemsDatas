## Description

<div><p>There's a famous museum in the city where Kleofáš lives. In the museum, <span class="tex-span"><i>n</i></span> exhibits (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>) had been displayed for a long time; the <span class="tex-span"><i>i</i></span>-th of those exhibits has value <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and mass <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Then, the museum was bought by a large financial group and started to vary the exhibits. At about the same time, Kleofáš... gained interest in the museum, so to say.</p><p>You should process <span class="tex-span"><i>q</i></span> events of three types:</p><ul><li> type <span class="tex-span">1</span> — the museum displays an exhibit with value <span class="tex-span"><i>v</i></span> and mass <span class="tex-span"><i>w</i></span>; the exhibit displayed in the <span class="tex-span"><i>i</i></span>-th event of this type is numbered <span class="tex-span"><i>n</i> + <i>i</i></span> (see sample explanation for more details)</li><li> type <span class="tex-span">2</span> — the museum removes the exhibit with number <span class="tex-span"><i>x</i></span> and stores it safely in its vault</li><li> type <span class="tex-span">3</span> — Kleofáš visits the museum and wonders (for no important reason at all, of course): if there was a robbery and exhibits with total mass at most <span class="tex-span"><i>m</i></span> were stolen, what would their maximum possible total value be?</li></ul><p>For each event of type 3, let <span class="tex-span"><i>s</i>(<i>m</i>)</span> be the maximum possible total value of stolen exhibits with total mass <span class="tex-span"> ≤ <i>m</i></span>.</p><p>Formally, let <span class="tex-span"><i>D</i></span> be the set of numbers of all exhibits that are currently displayed (so initially <span class="tex-span"><i>D</i></span> = {1, ..., n}). Let <span class="tex-span"><i>P</i>(<i>D</i>)</span> be the set of all subsets of <span class="tex-span"><i>D</i></span> and let </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://xBSJd9Ab.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Then, <span class="tex-span"><i>s</i>(<i>m</i>)</span> is defined as </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://y4nJ3KGf.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Compute <span class="tex-span"><i>s</i>(<i>m</i>)</span> for each <img align="middle" class="tex-formula" src="file://WZwefGK5.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that the output follows a special format.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the initial number of exhibits in the museum and the maximum interesting mass of stolen exhibits. </p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated positive integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the value and mass of the <span class="tex-span"><i>i</i></span>-th exhibit.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 30 000</span>)&nbsp;— the number of events.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains the description of one event in the following format:</p><ul><li> <span class="tex-span">1 <i>v</i> <i>w</i></span> — an event of type 1, a new exhibit with value <span class="tex-span"><i>v</i></span> and mass <span class="tex-span"><i>w</i></span> has been added (<span class="tex-span">1 ≤ <i>v</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 1000</span>)</li><li> <span class="tex-span">2 <i>x</i></span> — an event of type 2, the exhibit with number <span class="tex-span"><i>x</i></span> has been removed; it's guaranteed that the removed exhibit had been displayed at that time</li><li> <span class="tex-span">3</span> — an event of type 3, Kleofáš visits the museum and asks his question</li></ul><p>There will be at most <span class="tex-span">10 000</span> events of type 1 and at least one event of type 3.</p></div><div class="output-specification"><p>As the number of values <span class="tex-span"><i>s</i>(<i>m</i>)</span> can get large, output the answers to events of type 3 in a special format.</p><p>For each event of type 3, consider the values <span class="tex-span"><i>s</i>(<i>m</i>)</span> computed for the question that Kleofáš asked in this event; print one line containing a single number </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://DS9HMx3K.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where <span class="tex-span"><i>p</i> = 10<sup class="upper-index">7</sup> + 19</span> and <span class="tex-span"><i>q</i> = 10<sup class="upper-index">9</sup> + 7</span>.</p><p>Print the answers to events of type 3 in the order in which they appear in the input.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the initial number of exhibits in the museum and the maximum interesting mass of stolen exhibits. </p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated positive integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the value and mass of the <span class="tex-span"><i>i</i></span>-th exhibit.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 30 000</span>)&nbsp;— the number of events.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains the description of one event in the following format:</p><ul><li> <span class="tex-span">1 <i>v</i> <i>w</i></span> — an event of type 1, a new exhibit with value <span class="tex-span"><i>v</i></span> and mass <span class="tex-span"><i>w</i></span> has been added (<span class="tex-span">1 ≤ <i>v</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 1000</span>)</li><li> <span class="tex-span">2 <i>x</i></span> — an event of type 2, the exhibit with number <span class="tex-span"><i>x</i></span> has been removed; it's guaranteed that the removed exhibit had been displayed at that time</li><li> <span class="tex-span">3</span> — an event of type 3, Kleofáš visits the museum and asks his question</li></ul><p>There will be at most <span class="tex-span">10 000</span> events of type 1 and at least one event of type 3.</p>

## Output

<p>As the number of values <span class="tex-span"><i>s</i>(<i>m</i>)</span> can get large, output the answers to events of type 3 in a special format.</p><p>For each event of type 3, consider the values <span class="tex-span"><i>s</i>(<i>m</i>)</span> computed for the question that Kleofáš asked in this event; print one line containing a single number </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://DS9HMx3K.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where <span class="tex-span"><i>p</i> = 10<sup class="upper-index">7</sup> + 19</span> and <span class="tex-span"><i>q</i> = 10<sup class="upper-index">9</sup> + 7</span>.</p><p>Print the answers to events of type 3 in the order in which they appear in the input.</p>





```input1
3 10
30 4
60 6
5 1
9
3
1 42 5
1 20 3
3
2 2
2 4
3
1 40 6
3

```




```input2
3 1000
100 42
100 47
400 15
4
2 2
2 1
2 3
3

```




```output1
556674384
168191145
947033915
181541912

```




```output2
0

```



## Note

<p>In the first sample, the numbers of displayed exhibits and values <span class="tex-span"><i>s</i>(1), ..., <i>s</i>(10)</span> for individual events of type 3 are, in order: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://BoPZ7oL9.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <center class="tex-equation"><img align="middle" class="tex-formula" src="file://cepVeuTz.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <center class="tex-equation"><img align="middle" class="tex-formula" src="file://Qk5OYBHS.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <center class="tex-equation"><img align="middle" class="tex-formula" src="file://BpV3UNJr.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The values of individual exhibits are <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = 30, <i>v</i><sub class="lower-index">2</sub> = 60, <i>v</i><sub class="lower-index">3</sub> = 5, <i>v</i><sub class="lower-index">4</sub> = 42, <i>v</i><sub class="lower-index">5</sub> = 20, <i>v</i><sub class="lower-index">6</sub> = 40</span> and their masses are <span class="tex-span"><i>w</i><sub class="lower-index">1</sub> = 4, <i>w</i><sub class="lower-index">2</sub> = 6, <i>w</i><sub class="lower-index">3</sub> = 1, <i>w</i><sub class="lower-index">4</sub> = 5, <i>w</i><sub class="lower-index">5</sub> = 3, <i>w</i><sub class="lower-index">6</sub> = 6</span>.</p><p>In the second sample, the only question is asked after removing all exhibits, so <span class="tex-span"><i>s</i>(<i>m</i>) = 0</span> for any <span class="tex-span"><i>m</i></span>.</p>
