## Description

<div><p>Harry Potter lost his Invisibility Cloak, running from the school caretaker Filch. Finding an invisible object is not an easy task. Fortunately, Harry has friends who are willing to help. Hermione Granger had read "The Invisibility Cloaks, and Everything about Them", as well as six volumes of "The Encyclopedia of Quick Search of Shortest Paths in Graphs, Network Flows, the Maximal Increasing Subsequences and Other Magical Objects". She has already developed a search algorithm for the invisibility cloak in complex dynamic systems (Hogwarts is one of them).</p><p>Hogwarts consists of <span class="tex-span"><i>n</i></span> floors, numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some pairs of floors are connected by staircases. The staircases may change its position, moving exactly one end. Formally the situation is like this: if a staircase connects the floors <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, then in one move it may modify its position so as to connect the floors <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>c</i></span> or <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, where <span class="tex-span"><i>c</i></span> is any floor different from <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Under no circumstances the staircase can connect a floor with itself. At the same time there can be multiple stairs between a pair of floors.</p><p>Initially, Harry is on the floor with the number <span class="tex-span">1</span>. He does not remember on what floor he has lost the cloak and wants to look for it on each of the floors. Therefore, his goal is to visit each of <span class="tex-span"><i>n</i></span> floors at least once. Harry can visit the floors in any order and finish the searching at any floor.</p><p>Nowadays the staircases move quite rarely. However, Ron and Hermione are willing to put a spell on any of them to help Harry find the cloak. To cause less suspicion, the three friends plan to move the staircases one by one, and no more than once for each staircase. In between shifting the staircases Harry will be able to move about the floors, reachable at the moment from the staircases, and look for his Invisibility Cloak. It is assumed that during all this time the staircases will not move spontaneously.</p><p>Help the three friends to compose a searching plan. If there are several variants to solve the problem, any valid option (not necessarily the optimal one) will be accepted.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), which are the number of floors and staircases in Hogwarts, respectively. The following <span class="tex-span"><i>m</i></span> lines contain pairs of floors connected by staircases at the initial moment of time.</p></div><div class="output-specification"><p>In the first line print "YES" (without the quotes) if Harry is able to search all the floors, and "NO" otherwise. If the answer is positive, then print on the second line the number of staircases that Ron and Hermione will have to shift. Further output should look like this:</p><p><span class="tex-font-style-tt">Harry's moves</span> </p><p><span class="tex-font-style-tt">a staircase's move</span> </p><p><span class="tex-font-style-tt">Harry's moves</span></p><p><span class="tex-font-style-tt">a staircase's move</span></p><p>...</p><p><span class="tex-font-style-tt">a staircase's move</span></p><p><span class="tex-font-style-tt">Harry's moves</span></p><p>Each "<span class="tex-font-style-tt">Harry's move</span>" should be represented as a list of floors in the order in which they have been visited. <span class="tex-font-style-bf">The total amount of elements of these lists must not exceed</span> <span class="tex-span">10<sup class="upper-index">6</sup></span>. When you print each list, first print the number of elements in it, and then in the same line print the actual space-separated elements. The first number in the first list should be the number <span class="tex-span">1</span> (the floor, from which Harry begins to search). Any list except the first one might contain the zero number of elements. Note that Harry can visit some floors again, but must visit all <span class="tex-span"><i>n</i></span> floors at least once. Two consecutively visited floors must be directly connected by a staircase (at the time Harry goes from one of them to the other one). <span class="tex-font-style-bf">No two floors that are visited consequtively can be equal.</span></p><p>In the description of a "<span class="tex-font-style-tt">staircase's move</span>" indicate the number of staircase (the staircases are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order in which they are given in the input data) and its new location (two numbers of the connected floors in any order).</p><p>Any staircase can be moved at most once. If there are several solutions, output any.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), which are the number of floors and staircases in Hogwarts, respectively. The following <span class="tex-span"><i>m</i></span> lines contain pairs of floors connected by staircases at the initial moment of time.</p>

## Output

<p>In the first line print "YES" (without the quotes) if Harry is able to search all the floors, and "NO" otherwise. If the answer is positive, then print on the second line the number of staircases that Ron and Hermione will have to shift. Further output should look like this:</p><p><span class="tex-font-style-tt">Harry's moves</span> </p><p><span class="tex-font-style-tt">a staircase's move</span> </p><p><span class="tex-font-style-tt">Harry's moves</span></p><p><span class="tex-font-style-tt">a staircase's move</span></p><p>...</p><p><span class="tex-font-style-tt">a staircase's move</span></p><p><span class="tex-font-style-tt">Harry's moves</span></p><p>Each "<span class="tex-font-style-tt">Harry's move</span>" should be represented as a list of floors in the order in which they have been visited. <span class="tex-font-style-bf">The total amount of elements of these lists must not exceed</span> <span class="tex-span">10<sup class="upper-index">6</sup></span>. When you print each list, first print the number of elements in it, and then in the same line print the actual space-separated elements. The first number in the first list should be the number <span class="tex-span">1</span> (the floor, from which Harry begins to search). Any list except the first one might contain the zero number of elements. Note that Harry can visit some floors again, but must visit all <span class="tex-span"><i>n</i></span> floors at least once. Two consecutively visited floors must be directly connected by a staircase (at the time Harry goes from one of them to the other one). <span class="tex-font-style-bf">No two floors that are visited consequtively can be equal.</span></p><p>In the description of a "<span class="tex-font-style-tt">staircase's move</span>" indicate the number of staircase (the staircases are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order in which they are given in the input data) and its new location (two numbers of the connected floors in any order).</p><p>Any staircase can be moved at most once. If there are several solutions, output any.</p>





```input1
6 4
1 2
1 3
2 3
4 5

```




```input2
4 1
1 2

```




```input3
5 5
1 2
1 3
3 4
3 5
4 5

```




```output1
YES
2
3 1 2 3
2 3 5
3 5 4 5
4 5 6
3 6 5 3

```




```output2
NO

```




```output3
YES
0
6 1 2 1 3 4 5

```


