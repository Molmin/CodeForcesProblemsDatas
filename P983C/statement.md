## Description

<div><p>You work in a big office. It is a <span class="tex-span">9</span>&nbsp;floor building with an elevator that can accommodate up to <span class="tex-span">4</span>&nbsp;people. It is your responsibility to manage this elevator.</p><p>Today you are late, so there are queues on some floors already. For each person you know the floor where he currently is and the floor he wants to reach. Also, you know the order in which people came to the elevator.</p><p>According to the company's rules, if an employee comes to the elevator earlier than another one, he has to enter the elevator earlier too (even if these employees stay on different floors). Note that the employees are allowed to leave the elevator in arbitrary order.</p><p>The elevator has two commands: </p><ul> <li> Go up or down one floor. The movement takes <span class="tex-span">1</span> second. </li><li> Open the doors on the current floor. During this operation all the employees who have reached their destination get out of the elevator. Then all the employees on the floor get in the elevator in the order they are queued up while it doesn't contradict the company's rules and there is enough space in the elevator. Each employee spends <span class="tex-span">1</span> second to get inside and outside the elevator. </li></ul><p>Initially the elevator is empty and is located on the floor <span class="tex-span">1</span>.</p><p>You are interested what is the minimum possible time you need to spend to deliver all the employees to their destination. It is not necessary to return the elevator to the floor <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of employees.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the floor on which an employee initially is, and the floor he wants to reach.</p><p>The employees are given in the order they came to the elevator.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimal possible time in seconds.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of employees.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the floor on which an employee initially is, and the floor he wants to reach.</p><p>The employees are given in the order they came to the elevator.</p>

## Output

<p>Print a single integer&nbsp;— the minimal possible time in seconds.</p>





```input1
2
3 5
5 3

```




```input2
2
5 3
3 5

```




```output1
10
```




```output2
12
```



## Note

<center> Explaination for the first sample <img class="tex-graphics" src="file://DabsBaq9.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 0</span><p><img class="tex-graphics" src="file://MgmNIOwf.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 2</span></p><p><img class="tex-graphics" src="file://rHtOHaQ5.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 3</span></p><p><img class="tex-graphics" src="file://GARjKNBt.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 5</span></p><p><img class="tex-graphics" src="file://qFCYj5F0.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 6</span></p><p><img class="tex-graphics" src="file://IH021w6W.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 7</span></p><p><img class="tex-graphics" src="file://fPPDoura.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 9</span></p><p><img class="tex-graphics" src="file://aCS0AhaN.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>t</i> = 10</span></p></center>
