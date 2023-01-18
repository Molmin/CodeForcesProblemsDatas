## Description

<div><p>Welcome to Innopolis city. Throughout the whole year, Innopolis citizens suffer from everlasting city construction. </p><p>From the window in your room, you see the sequence of <span class="tex-span"><i>n</i></span> hills, where <span class="tex-span"><i>i</i></span>-th of them has height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The Innopolis administration wants to build some houses on the hills. However, for the sake of city appearance, a house can be only built on the hill, which is strictly higher than neighbouring hills (if they are present). For example, if the sequence of heights is <span class="tex-span">5, 4, 6, 2</span>, then houses could be built on hills with heights <span class="tex-span">5</span> and <span class="tex-span">6</span> only.</p><p>The Innopolis administration has an excavator, that can decrease the height of an arbitrary hill by one in one hour. The excavator can only work on one hill at a time. It is allowed to decrease hills up to zero height, or even to negative values. Increasing height of any hill is impossible. The city administration wants to build <span class="tex-span"><i>k</i></span> houses, so there must be at least <span class="tex-span"><i>k</i></span> hills that satisfy the condition above. What is the minimum time required to adjust the hills to achieve the administration's plan?</p><p>However, the exact value of <span class="tex-span"><i>k</i></span> is not yet determined, so could you please calculate answers for all <span class="tex-span"><i>k</i></span> in range <img align="middle" class="tex-formula" src="file://7RcMvqFF.png" style="max-width: 100.0%;max-height: 100.0%;">? Here <img align="middle" class="tex-formula" src="file://QkxZPqXI.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes <span class="tex-span"><i>n</i></span> divided by two, rounded up.</p></div><div class="input-specification"><p>The first line of input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)—the number of the hills in the sequence.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)—the heights of the hills in the sequence.</p></div><div class="output-specification"><p>Print exactly <img align="middle" class="tex-formula" src="file://uc5Kl74X.png" style="max-width: 100.0%;max-height: 100.0%;"> numbers separated by spaces. The <span class="tex-span"><i>i</i></span>-th printed number should be equal to the minimum number of hours required to level hills so it becomes possible to build <span class="tex-span"><i>i</i></span> houses.</p></div>

## Input

<p>The first line of input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)—the number of the hills in the sequence.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)—the heights of the hills in the sequence.</p>

## Output

<p>Print exactly <img align="middle" class="tex-formula" src="file://uc5Kl74X.png" style="max-width: 100.0%;max-height: 100.0%;"> numbers separated by spaces. The <span class="tex-span"><i>i</i></span>-th printed number should be equal to the minimum number of hours required to level hills so it becomes possible to build <span class="tex-span"><i>i</i></span> houses.</p>





```input1
5
1 1 1 1 1

```




```input2
3
1 2 3

```




```input3
5
1 2 3 2 2

```




```output1
1 2 2 

```




```output2
0 2 

```




```output3
0 1 3 

```



## Note

<p>In the first example, to get at least one hill suitable for construction, one can decrease the second hill by one in one hour, then the sequence of heights becomes <span class="tex-span">1, 0, 1, 1, 1</span> and the first hill becomes suitable for construction.</p><p>In the first example, to get at least two or at least three suitable hills, one can decrease the second and the fourth hills, then the sequence of heights becomes <span class="tex-span">1, 0, 1, 0, 1</span>, and hills <span class="tex-span">1, 3, 5</span> become suitable for construction.</p>
