## Description

<div><p>One day Ms Swan bought an orange in a shop. The orange consisted of <span class="tex-span"><i>n</i>·<i>k</i></span> segments, numbered with integers from 1 to <span class="tex-span"><i>n</i>·<i>k</i></span>. </p><p>There were <span class="tex-span"><i>k</i></span> children waiting for Ms Swan at home. The children have recently learned about the orange and they decided to divide it between them. For that each child took a piece of paper and wrote the number of the segment that he would like to get: the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>k</i>)</span> child wrote the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>·<i>k</i>)</span>. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> accidentally turned out to be different.</p><p>Now the children wonder, how to divide the orange so as to meet these conditions:</p><ul> <li> each child gets exactly <span class="tex-span"><i>n</i></span> orange segments; </li><li> the <span class="tex-span"><i>i</i></span>-th child gets the segment with number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for sure; </li><li> no segment goes to two children simultaneously. </li></ul><p>Help the children, divide the orange and fulfill the requirements, described above.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 30)</span>. The second line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>·<i>k</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the orange segment that the <span class="tex-span"><i>i</i></span>-th child would like to get.</p><p>It is guaranteed that all numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>n</i>·<i>k</i></span> distinct integers. The first <span class="tex-span"><i>n</i></span> integers represent the indexes of the segments the first child will get, the second <span class="tex-span"><i>n</i></span> integers represent the indexes of the segments the second child will get, and so on. Separate the printed numbers with whitespaces.</p><p>You can print a child's segment indexes in any order. It is guaranteed that the answer always exists. If there are multiple correct answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 30)</span>. The second line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>·<i>k</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the orange segment that the <span class="tex-span"><i>i</i></span>-th child would like to get.</p><p>It is guaranteed that all numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print exactly <span class="tex-span"><i>n</i>·<i>k</i></span> distinct integers. The first <span class="tex-span"><i>n</i></span> integers represent the indexes of the segments the first child will get, the second <span class="tex-span"><i>n</i></span> integers represent the indexes of the segments the second child will get, and so on. Separate the printed numbers with whitespaces.</p><p>You can print a child's segment indexes in any order. It is guaranteed that the answer always exists. If there are multiple correct answers, print any of them.</p>





```input1
2 2
4 1

```




```input2
3 1
2

```




```output1
2 4 
1 3 

```




```output2
3 2 1 

```


