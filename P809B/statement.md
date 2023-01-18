## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. In the output section below you will see the information about flushing the output.</span></p><p>On Sunday Leha the hacker took Nura from the house where she lives and went with her to one of the most luxurious restaurants in Vičkopolis. Upon arrival, they left the car in a huge parking lot near the restaurant and hurried inside the building.</p><p>In the restaurant a polite waiter immediately brought the menu to Leha and Noora, consisting of <span class="tex-span"><i>n</i></span> dishes. It is interesting that all dishes in the menu are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. After a little thought, the girl ordered exactly <span class="tex-span"><i>k</i></span> different dishes from available in the menu. To pass the waiting time while the chefs prepare ordered dishes, the girl invited the hacker to play a game that will help them get to know each other better.</p><p>The game itself is very simple: Noora wants Leha to guess any two dishes among all ordered. At the same time, she is ready to answer only one type of questions. Leha can say two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>. After that Noora chooses some dish <span class="tex-span"><i>a</i></span> for the number <span class="tex-span"><i>x</i></span> such that, at first, <span class="tex-span"><i>a</i></span> is among the dishes Noora ordered (<span class="tex-span"><i>x</i></span> can be equal to <span class="tex-span"><i>a</i></span>), and, secondly, the value <img align="middle" class="tex-formula" src="file://93m0HMlq.png" style="max-width: 100.0%;max-height: 100.0%;"> is the minimum possible. By the same rules the girl chooses dish <span class="tex-span"><i>b</i></span> for <span class="tex-span"><i>y</i></span>. After that Noora says «<span class="tex-font-style-tt">TAK</span>» to Leha, if <img align="middle" class="tex-formula" src="file://nxhTEnPG.png" style="max-width: 100.0%;max-height: 100.0%;">, and «<span class="tex-font-style-tt">NIE</span>» otherwise. However, the restaurant is preparing quickly, so Leha has enough time to ask no more than <span class="tex-span">60</span> questions. After that he should name numbers of any two dishes Noora ordered.</p><p>Help Leha to solve this problem!</p></div><div class="input-specification"><p>There are two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> in the single line of input denoting the number of dishes in the menu and the number of dishes Noora ordered.</p></div><div class="output-specification"><p>If you want to provide an answer, output a string of the form <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i>)</span>, if you think the dishes <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> was among dishes ordered by Noora. After that, flush the output and terminate your program.</p></div><div><h2>Interaction</h2><p>While helping Leha, you can ask queries to Noora no more than <span class="tex-span">60</span> times. Each query should be printed in it's own line and have the form <span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>. You have to both print the end-of-line character and flush the output. After flushing you should read the answer for this query from input.</p><p>After each query jury's program will print one line «<span class="tex-font-style-tt">TAK</span>» or «<span class="tex-font-style-tt">NIE</span>» (without quotes) in input stream depending on the girl's answer.</p><p>To flush you can use (just after printing an integer and end-of-line):</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacking</span></p><p>For hacking you should write numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> in the first line and, for describing dishes Noora ordered, <span class="tex-span"><i>k</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, <span class="tex-font-style-it">written in ascending order</span> in the second line. Of course, solution you want to hack won't be able to read the numbers of ordered dishes.</p></div>

## Input

<p>There are two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> in the single line of input denoting the number of dishes in the menu and the number of dishes Noora ordered.</p>

## Output

<p>If you want to provide an answer, output a string of the form <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i>)</span>, if you think the dishes <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> was among dishes ordered by Noora. After that, flush the output and terminate your program.</p>





```input1
3 2
NIE
TAK
NIE
TAK
TAK
TAK

```




```output1
1 1 2
1 2 1
1 1 3
1 3 1
1 2 3
1 3 2
2 2 3

```



## Note

<p>There are three dishes in sample. Noora ordered dished numberes <span class="tex-span">2</span> and <span class="tex-span">3</span>, which Leha should guess. If Noora receive requests for the first dish (<span class="tex-span"><i>x</i> = 1</span>), then she'll choose the second dish (<span class="tex-span"><i>a</i> = 2</span>) as the dish with the minimum value <img align="middle" class="tex-formula" src="file://WaOfiJyv.png" style="max-width: 100.0%;max-height: 100.0%;">. For the second (<span class="tex-span"><i>x</i> = 2</span>) and the third (<span class="tex-span"><i>x</i> = 3</span>) dishes themselves will be optimal, because in that case <img align="middle" class="tex-formula" src="file://up2fUb5K.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Let Leha asks Noora about the next couple of dishes:</p><ul> <li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 2</span>, then he'll recieve «<span class="tex-font-style-tt">NIE</span>» answer, because <span class="tex-span">|1 - 2| &gt; |2 - 2|</span> </li><li> <span class="tex-span"><i>x</i> = 2</span>, <span class="tex-span"><i>y</i> = 1</span>, then he'll recieve «<span class="tex-font-style-tt">TAK</span>» answer, because <span class="tex-span">|2 - 2| ≤ |1 - 2|</span> </li><li> <span class="tex-span"><i>x</i> = 1</span>, <span class="tex-span"><i>y</i> = 3</span>, then he'll recieve «<span class="tex-font-style-tt">NIE</span>» answer, because <span class="tex-span">|1 - 2| &gt; |3 - 3|</span> </li><li> <span class="tex-span"><i>x</i> = 3</span>, <span class="tex-span"><i>y</i> = 1</span>, then he'll recieve «<span class="tex-font-style-tt">TAK</span>» answer, because <span class="tex-span">|3 - 3| ≤ |1 - 2|</span> </li><li> <span class="tex-span"><i>x</i> = 2</span>, <span class="tex-span"><i>y</i> = 3</span>, then he'll recieve «<span class="tex-font-style-tt">TAK</span>» answer, because <span class="tex-span">|2 - 2| ≤ |3 - 3|</span> </li><li> <span class="tex-span"><i>x</i> = 3</span>, <span class="tex-span"><i>y</i> = 2</span>, then he'll recieve «<span class="tex-font-style-tt">TAK</span>» answer, because <span class="tex-span">|3 - 3| ≤ |2 - 2|</span> </li></ul><p>According to the available information, it is possible to say that Nura ordered dishes with numbers <span class="tex-span">2</span> and <span class="tex-span">3</span>.</p>
