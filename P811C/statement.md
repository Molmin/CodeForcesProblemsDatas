## Description

<div><p>Vladik often travels by trains. He remembered some of his trips especially well and I would like to tell you about one of these trips:</p><p>Vladik is at initial train station, and now <span class="tex-span"><i>n</i></span> people (including Vladik) want to get on the train. They are already lined up in some order, and for each of them the city code <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is known (the code of the city in which they are going to).</p><p>Train chief selects some number of disjoint segments of the original sequence of people (covering entire sequence by segments is <span class="tex-font-style-bf">not necessary</span>). People who are in the same segment will be in the same train carriage. The segments are selected in such way that if at least one person travels to the city <span class="tex-span"><i>x</i></span>, then all people who are going to city <span class="tex-span"><i>x</i></span> should be in the same railway carriage. This means that they can’t belong to different segments. Note, that all people who travel to the city <span class="tex-span"><i>x</i></span>, either go to it and in the same railway carriage, or do not go anywhere at all.</p><p>Comfort of a train trip with people on segment from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span> is equal to <span class="tex-font-style-tt">XOR</span> of all distinct codes of cities for people on the segment from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>. <span class="tex-font-style-tt">XOR</span> operation also known as exclusive <span class="tex-font-style-tt">OR</span>.</p><p>Total comfort of a train trip is equal to sum of comfort for each segment.</p><p>Help Vladik to know maximal possible total comfort.</p></div><div class="input-specification"><p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— number of people.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes code of the city to which <span class="tex-span"><i>i</i></span>-th person is going.</p></div><div class="output-specification"><p>The output should contain a single integer&nbsp;— maximal possible total comfort.</p></div>

## Input

<p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— number of people.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes code of the city to which <span class="tex-span"><i>i</i></span>-th person is going.</p>

## Output

<p>The output should contain a single integer&nbsp;— maximal possible total comfort.</p>





```input1
6
4 4 2 5 2 3

```




```input2
9
5 1 3 1 5 2 4 2 5

```




```output1
14

```




```output2
9

```



## Note

<p>In the first test case best partition into segments is: <span class="tex-span">[4, 4]</span> <span class="tex-span">[2, 5, 2]</span> <span class="tex-span">[3]</span>, answer is calculated as follows: <span class="tex-span">4 + (2</span> <span class="tex-span"><i>xor</i></span> <span class="tex-span">5) + 3 = 4 + 7 + 3 = 14</span></p><p>In the second test case best partition into segments is: <span class="tex-span">5</span> <span class="tex-span">1</span> <span class="tex-span">[3]</span> <span class="tex-span">1</span> <span class="tex-span">5</span> <span class="tex-span">[2, 4, 2]</span> <span class="tex-span">5</span>, answer calculated as follows: <span class="tex-span">3 + (2</span> <span class="tex-span"><i>xor</i></span> <span class="tex-span">4) = 3 + 6 = 9</span>.</p>
