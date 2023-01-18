## Description

<div><p>This night wasn't easy on Vasya. His favorite team lost, and he didn't find himself victorious either&nbsp;— although he played perfectly, his teammates let him down every time. He had to win at least one more time, but the losestreak only grew longer and longer... It's no wonder he didn't get any sleep this night at all.</p><p>In the morning, Vasya was waiting the bus to the university on the bus stop. Vasya's thoughts were hazy and so he couldn't remember the right bus' number quite right and got onto the bus with the number $n$.</p><p>In the bus, Vasya thought that he could get the order of the digits in the number of the bus wrong. Futhermore, he could "see" some digits several times, but the digits he saw were definitely in the real number of the bus. For example, if Vasya saw the number <span class="tex-font-style-tt">2028</span>, it could mean that the real bus number could be <span class="tex-font-style-tt">2028</span>, <span class="tex-font-style-tt">8022</span>, <span class="tex-font-style-tt">2820</span> or just <span class="tex-font-style-tt">820</span>. However, numbers <span class="tex-font-style-tt">80</span>, <span class="tex-font-style-tt">22208</span>, <span class="tex-font-style-tt">52</span> definitely couldn't be the number of the bus. Also, real bus number couldn't start with the digit <span class="tex-font-style-tt">0</span>, this meaning that, for example, number <span class="tex-font-style-tt">082</span> couldn't be the real bus number too.</p><p>Given $n$, determine the total number of possible bus number variants.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;— the number of the bus that was seen by Vasya. It is guaranteed that this number does not start with $0$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the amount of possible variants of the real bus number.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;— the number of the bus that was seen by Vasya. It is guaranteed that this number does not start with $0$.</p>

## Output

<p>Output a single integer&nbsp;— the amount of possible variants of the real bus number.</p>





```input1
97

```




```input2
2028

```




```output1
2

```




```output2
13

```



## Note

<p>In the first sample, only variants $97$ and $79$ are possible.</p><p>In the second sample, the variants (in the increasing order) are the following: $208$, $280$, $802$, $820$, $2028$, $2082$, $2208$, $2280$, $2802$, $2820$, $8022$, $8202$, $8220$.</p>
