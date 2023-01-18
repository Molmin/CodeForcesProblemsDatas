## Description

<div><p>One day a highly important task was commissioned to Vasya — writing a program in a night. The program consists of <span class="tex-span"><i>n</i></span> lines of code. Vasya is already exhausted, so he works like that: first he writes <span class="tex-span"><i>v</i></span> lines of code, drinks a cup of tea, then he writes as much as <img align="middle" class="tex-formula" src="file://a2oZaqbJ.png" style="max-width: 100.0%;max-height: 100.0%;"> lines, drinks another cup of tea, then he writes <img align="middle" class="tex-formula" src="file://X03WFwKk.png" style="max-width: 100.0%;max-height: 100.0%;"> lines and so on: <img align="middle" class="tex-formula" src="file://26tThEkq.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://wZVz7NHH.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://GKgc9ZpV.png" style="max-width: 100.0%;max-height: 100.0%;">, ...</p><p>The expression <img align="middle" class="tex-formula" src="file://YRA7QvFQ.png" style="max-width: 100.0%;max-height: 100.0%;"> is regarded as the integral part from dividing number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>b</i></span>.</p><p>The moment the current value <img align="middle" class="tex-formula" src="file://ftJ6od8a.png" style="max-width: 100.0%;max-height: 100.0%;"> equals 0, Vasya immediately falls asleep and he wakes up only in the morning, when the program should already be finished.</p><p>Vasya is wondering, what minimum allowable value <span class="tex-span"><i>v</i></span> can take to let him write <span class="tex-font-style-bf">not less</span> than <span class="tex-span"><i>n</i></span> lines of code before he falls asleep.</p></div><div class="input-specification"><p>The input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by spaces — the size of the program in lines and the productivity reduction coefficient, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>.</p></div><div class="output-specification"><p>Print the only integer — the minimum value of <span class="tex-span"><i>v</i></span> that lets Vasya write the program in one night.</p></div>

## Input

<p>The input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by spaces — the size of the program in lines and the productivity reduction coefficient, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>.</p>

## Output

<p>Print the only integer — the minimum value of <span class="tex-span"><i>v</i></span> that lets Vasya write the program in one night.</p>





```input1
7 2

```




```input2
59 9

```




```output1
4

```




```output2
54

```



## Note

<p>In the first sample the answer is <span class="tex-span"><i>v</i> = 4</span>. Vasya writes the code in the following portions: first <span class="tex-span">4</span> lines, then <span class="tex-span">2</span>, then <span class="tex-span">1</span>, and then Vasya falls asleep. Thus, he manages to write <span class="tex-span">4 + 2 + 1 = 7</span> lines in a night and complete the task.</p><p>In the second sample the answer is <span class="tex-span"><i>v</i> = 54</span>. Vasya writes the code in the following portions: <span class="tex-span">54</span>, <span class="tex-span">6</span>. The total sum is <span class="tex-span">54 + 6 = 60</span>, that's even more than <span class="tex-span"><i>n</i> = 59</span>.</p>
