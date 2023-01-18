## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>In the Wonderful Metropolis of the Future, there is no need in subway train drivers. Due to the technological progress, they were replaced by the Artificial Intelligence (AI). Unfortunately, one day the predictions of sci-fi writers came true: the AI rebelled and now there is an uncontrollable train in the subway. It can be dangerous! Your task is to find the train and stop the AI.</p><p>The subway of the Metropolis is one line (regular straight line with no self-intersections) with $n$ stations, indexed consecutively from $1$ to $n$. At each moment the train is at some station. You need to determine the index of this station, so that the train would be secured.</p><p>To find the train, dispatcher Sarah gave you a gadget that allows you to select arbitrary numbers $l$ and $r$ ($l \le r$), and then check, whether the train is located on a station with index between $l$ and $r$, inclusive. Unfortunately, recharging of the gadget takes some time (and every time you use it as soon as possible), so between two applications of the gadget the train can move to any station that is at most $k$ stations away. Formally, if the train was at the station $x$ when the gadget was applied, then at the next application of the gadget the train can appear at any station $y$ such that $\max(1, x - k) \leq y \leq \min(n, x + k)$.</p><p>Note that AI is not aware that you are trying to catch the train, so it makes all moves according to its predefined plan.</p><p>After an examination of the gadget you found that it is very old and can hold no more than $4500$ applications, after which it will break and your mission will be considered a failure.</p><p>Can you find the station with the train using no more than $4500$ applications of the gadgets?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^{18}$, $0 \leq k \leq 10$)&nbsp;— the number of stations and the maximum number of stations the train can move between two applications of the gadget.</p></div><div><h2>Interaction</h2><p>You can apply the gadget at most $4500$ times. In order to apply the gadget you need to print two space-separated integers $l$ and $r$ ($1 \leq l \leq r \leq n$). You will then receive either string "<span class="tex-font-style-tt">Yes</span>", if the train is between stations $l$ and $r$, inclusive, or string "<span class="tex-font-style-tt">No</span>" otherwise. If $l = r$ and you received "<span class="tex-font-style-tt">Yes</span>", then you found the train successfully, and your program must halt immediately.</p><p>Answer "<span class="tex-font-style-tt">Bad</span>" instead of "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>" means that you made an invalid query or made too many queries. Exit immediately after receiving "<span class="tex-font-style-tt">Bad</span>" and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>In order to hack, you should present a test in the following format.</p><p>The first line should contain three integers $n$, $k$ and $p$ ($1 \le n \le 10^{18}$, $0 \le k \le 10$, $1 \le p \le n$)&nbsp;— the number of stations, the maximum number of stations the train can move between two applications of the gadget and the initial position of the train, respectively.</p><p>Each of the next $4500$ lines should contain a single integer $x$ ($1 \le x \le n$)&nbsp;— the positions of the train after each query. Two consecutive positions (including the initial one) should not differ by more than $k$.</p><p>For example, the following lines are the first lines of the sample test.</p><pre class="verbatim"><br>10 2 5<br>5<br>3<br>5<br>7<br>7<br>...<br></pre></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 10^{18}$, $0 \leq k \leq 10$)&nbsp;— the number of stations and the maximum number of stations the train can move between two applications of the gadget.</p>





```input1
10 2

Yes

No

Yes

Yes

```




```output1
3 5

3 3

3 4

5 5

```



## Note

<p>In the first sample, the train was initially at the station $5$, after the first application of the gadget it did not move, after the second application it moved to the station $3$, and after the third application moved again to the station $5$.</p>
