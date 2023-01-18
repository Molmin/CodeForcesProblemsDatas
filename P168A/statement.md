## Description

<div><p>Some country is populated by wizards. They want to organize a demonstration.</p><p>There are <span class="tex-span"><i>n</i></span> people living in the city, <span class="tex-span"><i>x</i></span> of them are the wizards who will surely go to the demonstration. Other city people (<span class="tex-span"><i>n</i> - <i>x</i></span> people) do not support the wizards and aren't going to go to the demonstration. We know that the city administration will react only to the demonstration involving at least <span class="tex-span"><i>y</i></span> percent of the city people. Having considered the matter, the wizards decided to create clone puppets which can substitute the city people on the demonstration. </p><p>So all in all, the demonstration will involve only the wizards and their puppets. The city administration cannot tell the difference between a puppet and a person, so, as they calculate the percentage, the administration will consider the city to be consisting of only <span class="tex-span"><i>n</i></span> people and not containing any clone puppets. </p><p>Help the wizards and find the minimum number of clones to create to that the demonstration had no less than <span class="tex-span"><i>y</i></span> percent of the city people.</p></div><div class="input-specification"><p>The first line contains three space-separated integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">4</sup>, <i>x</i> ≤ <i>n</i></span>) — the number of citizens in the city, the number of wizards and the percentage the administration needs, correspondingly.</p><p>Please note that <span class="tex-span"><i>y</i></span> can exceed 100 percent, that is, the administration wants to see on a demonstration more people that actually live in the city (<span class="tex-span"> &gt; <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem, the minimum number of clones to create, so that the demonstration involved no less than <span class="tex-span"><i>y</i></span> percent of <span class="tex-span"><i>n</i></span> (the real total city population). </p></div>

## Input

<p>The first line contains three space-separated integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">4</sup>, <i>x</i> ≤ <i>n</i></span>) — the number of citizens in the city, the number of wizards and the percentage the administration needs, correspondingly.</p><p>Please note that <span class="tex-span"><i>y</i></span> can exceed 100 percent, that is, the administration wants to see on a demonstration more people that actually live in the city (<span class="tex-span"> &gt; <i>n</i></span>).</p>

## Output

<p>Print a single integer — the answer to the problem, the minimum number of clones to create, so that the demonstration involved no less than <span class="tex-span"><i>y</i></span> percent of <span class="tex-span"><i>n</i></span> (the real total city population). </p>





```input1
10 1 14

```




```input2
20 10 50

```




```input3
1000 352 146

```




```output1
1

```




```output2
0

```




```output3
1108

```



## Note

<p>In the first sample it is necessary that at least 14% of 10 people came to the demonstration. As the number of people should be integer, then at least two people should come. There is only one wizard living in the city and he is going to come. That isn't enough, so he needs to create one clone. </p><p>In the second sample 10 people should come to the demonstration. The city has 10 wizards. They will all come to the demonstration, so nobody has to create any clones.</p>
