## Description

<div><p>There are <span class="tex-span"><i>n</i></span> animals in the queue to Dr. Dolittle. When an animal comes into the office, the doctor examines him, gives prescriptions, appoints tests and may appoint extra examination. Doc knows all the forest animals perfectly well and therefore knows exactly that the animal number <span class="tex-span"><i>i</i></span> in the queue will have to visit his office exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> times. We will assume that an examination takes much more time than making tests and other extra procedures, and therefore we will assume that once an animal leaves the room, it immediately gets to the end of the queue to the doctor. Of course, if the animal has visited the doctor as many times as necessary, then it doesn't have to stand at the end of the queue and it immediately goes home. </p><p>Doctor plans to go home after receiving <span class="tex-span"><i>k</i></span> animals, and therefore what the queue will look like at that moment is important for him. Since the doctor works long hours and she can't get distracted like that after all, she asked you to figure it out. </p></div><div class="input-specification"><p>The first line of input data contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">14</sup></span>). In the second line are given space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (you can also use the <span class="tex-font-style-tt">%I64d</span> specificator). </p></div><div class="output-specification"><p>If the doctor will overall carry out less than <span class="tex-span"><i>k</i></span> examinations, print a single number "-1" (without quotes). Otherwise, print the sequence of numbers — number of animals in the order in which they stand in the queue. </p><p><span class="tex-font-style-bf">Note that this sequence may be empty.</span> This case is present in pretests. You can just print nothing or print one "End of line"-character. Both will be accepted.</p></div>

## Input

<p>The first line of input data contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">14</sup></span>). In the second line are given space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit numbers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (you can also use the <span class="tex-font-style-tt">%I64d</span> specificator). </p>

## Output

<p>If the doctor will overall carry out less than <span class="tex-span"><i>k</i></span> examinations, print a single number "-1" (without quotes). Otherwise, print the sequence of numbers — number of animals in the order in which they stand in the queue. </p><p><span class="tex-font-style-bf">Note that this sequence may be empty.</span> This case is present in pretests. You can just print nothing or print one "End of line"-character. Both will be accepted.</p>





```input1
3 3
1 2 1

```




```input2
4 10
3 3 2 1

```




```input3
7 10
1 3 3 1 2 3 1

```




```output1
2
```




```output2
-1

```




```output3
6 2 3
```



## Note

<p>In the first sample test:</p><ul> <li> Before examination: <span class="tex-span">{1, 2, 3}</span> </li><li> After the first examination: <span class="tex-span">{2, 3}</span> </li><li> After the second examination: <span class="tex-span">{3, 2}</span> </li><li> After the third examination: <span class="tex-span">{2}</span> </li></ul><p>In the second sample test:</p><ul> <li> Before examination: <span class="tex-span">{1, 2, 3, 4, 5, 6, 7}</span> </li><li> After the first examination: <span class="tex-span">{2, 3, 4, 5, 6, 7}</span> </li><li> After the second examination: <span class="tex-span">{3, 4, 5, 6, 7, 2}</span> </li><li> After the third examination: <span class="tex-span">{4, 5, 6, 7, 2, 3}</span> </li><li> After the fourth examination: <span class="tex-span">{5, 6, 7, 2, 3}</span> </li><li> After the fifth examination: <span class="tex-span">{6, 7, 2, 3, 5}</span> </li><li> After the sixth examination: <span class="tex-span">{7, 2, 3, 5, 6}</span> </li><li> After the seventh examination: <span class="tex-span">{2, 3, 5, 6}</span> </li><li> After the eighth examination: <span class="tex-span">{3, 5, 6, 2}</span> </li><li> After the ninth examination: <span class="tex-span">{5, 6, 2, 3}</span> </li><li> After the tenth examination: <span class="tex-span">{6, 2, 3}</span> </li></ul>
