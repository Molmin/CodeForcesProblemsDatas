## Description

<div><p>Polycarp has just attempted to pass the driving test. He ran over the straight road with the signs of four types.</p><ul> <li> speed limit: this sign comes with a positive integer number — maximal speed of the car after the sign (cancel the action of the previous sign of this type); </li><li> overtake is allowed: this sign means that after some car meets it, it can overtake any other car; </li><li> no speed limit: this sign cancels speed limit if any (car can move with arbitrary speed after this sign); </li><li> no overtake allowed: some car can't overtake any other car after this sign. </li></ul><p>Polycarp goes past the signs consequentially, each new sign cancels the action of all the previous signs of it's kind (speed limit/overtake). It is possible that two or more "no overtake allowed" signs go one after another with zero "overtake is allowed" signs between them. It works with "no speed limit" and "overtake is allowed" signs as well.</p><p>In the beginning of the ride overtake is allowed and there is no speed limit.</p><p>You are given the sequence of events in chronological order — events which happened to Polycarp during the ride. There are events of following types:</p><ol> <li> Polycarp changes the speed of his car to specified (this event comes with a positive integer number); </li><li> Polycarp's car overtakes the other car; </li><li> Polycarp's car goes past the "speed limit" sign (this sign comes with a positive integer); </li><li> Polycarp's car goes past the "overtake is allowed" sign; </li><li> Polycarp's car goes past the "no speed limit"; </li><li> Polycarp's car goes past the "no overtake allowed"; </li></ol><p>It is guaranteed that the first event in chronological order is the event of type <span class="tex-span">1</span> (Polycarp changed the speed of his car to specified).</p><p>After the exam Polycarp can justify his rule violations by telling the driving instructor that he just didn't notice some of the signs. What is the minimal number of signs Polycarp should say he didn't notice, so that he would make no rule violations from his point of view?</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of events.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines starts with integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 6</span>) — the type of the event.</p><p>An integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 300</span>) follows in the query of the first and the third type (if it is the query of first type, then it's new speed of Polycarp's car, if it is the query of third type, then it's new speed limit).</p><p>It is guaranteed that the first event in chronological order is the event of type <span class="tex-span">1</span> (Polycarp changed the speed of his car to specified).</p></div><div class="output-specification"><p>Print the minimal number of road signs Polycarp should say he didn't notice, so that he would make no rule violations from his point of view.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of events.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines starts with integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 6</span>) — the type of the event.</p><p>An integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 300</span>) follows in the query of the first and the third type (if it is the query of first type, then it's new speed of Polycarp's car, if it is the query of third type, then it's new speed limit).</p><p>It is guaranteed that the first event in chronological order is the event of type <span class="tex-span">1</span> (Polycarp changed the speed of his car to specified).</p>

## Output

<p>Print the minimal number of road signs Polycarp should say he didn't notice, so that he would make no rule violations from his point of view.</p>





```input1
11
1 100
3 70
4
2
3 120
5
3 120
6
1 150
4
3 300

```




```input2
5
1 100
3 200
2
4
5

```




```input3
7
1 20
2
6
4
6
6
2

```




```output1
2

```




```output2
0

```




```output3
2

```



## Note

<p>In the first example Polycarp should say he didn't notice the "speed limit" sign with the limit of <span class="tex-span">70</span> and the second "speed limit" sign with the limit of <span class="tex-span">120</span>.</p><p>In the second example Polycarp didn't make any rule violation.</p><p>In the third example Polycarp should say he didn't notice both "no overtake allowed" that came after "overtake is allowed" sign.</p>
