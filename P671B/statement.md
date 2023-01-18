## Description

<div><p>We all know the impressive story of Robin Hood. Robin Hood uses his archery skills and his wits to steal the money from rich, and return it to the poor.</p><p>There are <span class="tex-span"><i>n</i></span> citizens in Kekoland, each person has <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> coins. Each day, Robin Hood will take exactly <span class="tex-span">1</span> coin from the richest person in the city and he will give it to the poorest person (poorest person right after taking richest's <span class="tex-span">1</span> coin). In case the choice is not unique, he will select one among them at random. Sadly, Robin Hood is old and want to retire in <span class="tex-span"><i>k</i></span> days. He decided to spend these last days with helping poor people. </p><p>After taking his money are taken by Robin Hood richest person may become poorest person as well, and it might even happen that Robin Hood will give his money back. For example if all people have same number of coins, then next day they will have same number of coins too. </p><p>Your task is to find the difference between richest and poorest persons wealth after <span class="tex-span"><i>k</i></span> days. Note that the choosing at random among richest and poorest doesn't affect the answer.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of citizens in Kekoland and the number of days left till Robin Hood's retirement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial wealth of the <span class="tex-span"><i>i</i></span>-th person.</p></div><div class="output-specification"><p>Print a single line containing the difference between richest and poorest peoples wealth.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of citizens in Kekoland and the number of days left till Robin Hood's retirement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial wealth of the <span class="tex-span"><i>i</i></span>-th person.</p>

## Output

<p>Print a single line containing the difference between richest and poorest peoples wealth.</p>





```input1
4 1
1 1 4 2

```




```input2
3 1
2 2 2

```




```output1
2

```




```output2
0

```



## Note

<p>Lets look at how wealth changes through day in the first sample.</p><ol> <li> <span class="tex-span">[1, 1, 4, 2]</span> </li><li> <span class="tex-span">[2, 1, 3, 2]</span> or <span class="tex-span">[1, 2, 3, 2]</span> </li></ol><p>So the answer is <span class="tex-span">3 - 1 = 2</span></p><p>In second sample wealth will remain the same for each person.</p>
