## Description

<div><p>One way to create a task is to learn from life. You can choose some experience in real life, formalize it and then you will get a new task.</p><p>Let's think about a scene in real life: there are lots of people waiting in front of the elevator, each person wants to go to a certain floor. We can formalize it in the following way. We have <span class="tex-span"><i>n</i></span> people standing on the first floor, the <span class="tex-span"><i>i</i></span>-th person wants to go to the <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>-th floor. Unfortunately, there is only one elevator and its capacity equal to <span class="tex-span"><i>k</i></span> (that is at most <span class="tex-span"><i>k</i></span> people can use it simultaneously). Initially the elevator is located on the first floor. The elevator needs <span class="tex-span">|<i>a</i> - <i>b</i>|</span> seconds to move from the <span class="tex-span"><i>a</i></span>-th floor to the <span class="tex-span"><i>b</i></span>-th floor (we don't count the time the people need to get on and off the elevator).</p><p>What is the minimal number of seconds that is needed to transport all the people to the corresponding floors and then return the elevator to the first floor?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 2000)</span> — the number of people and the maximal capacity of the elevator.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span>, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> denotes the target floor of the <span class="tex-span"><i>i</i></span>-th person.</p></div><div class="output-specification"><p>Output a single integer — the minimal time needed to achieve the goal.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 2000)</span> — the number of people and the maximal capacity of the elevator.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span>, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> denotes the target floor of the <span class="tex-span"><i>i</i></span>-th person.</p>

## Output

<p>Output a single integer — the minimal time needed to achieve the goal.</p>





```input1
3 2
2 3 4

```




```input2
4 2
50 100 50 100

```




```input3
10 3
2 2 2 2 2 2 2 2 2 2

```




```output1
8

```




```output2
296

```




```output3
8

```



## Note

<p>In first sample, an optimal solution is: </p><ol> <li> The elevator takes up person #1 and person #2. </li><li> It goes to the 2nd floor. </li><li> Both people go out of the elevator. </li><li> The elevator goes back to the 1st floor. </li><li> Then the elevator takes up person #3. </li><li> And it goes to the 2nd floor. </li><li> It picks up person #2. </li><li> Then it goes to the 3rd floor. </li><li> Person #2 goes out. </li><li> Then it goes to the 4th floor, where person #3 goes out. </li><li> The elevator goes back to the 1st floor. </li></ol>
