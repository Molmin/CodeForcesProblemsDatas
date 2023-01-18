## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=MtN1YnoL46Q">The Duck song</a></div></div><p>For simplicity, we'll assume that there are only three types of grapes: green grapes, purple grapes and black grapes.</p><p>Andrew, Dmitry and Michal are all grapes' lovers, however their preferences of grapes are different. To make all of them happy, the following should happen:</p><ul><li> Andrew, Dmitry and Michal should eat at least $x$, $y$ and $z$ grapes, respectively.</li><li> Andrew has an extreme affinity for green grapes, thus he will eat green grapes and green grapes only.</li><li> On the other hand, Dmitry is not a fan of black grapes&nbsp;— any types of grapes except black would do for him. In other words, Dmitry can eat green and purple grapes.</li><li> Michal has a common taste&nbsp;— he enjoys grapes in general and will be pleased with any types of grapes, as long as the quantity is sufficient.</li></ul><p>Knowing that his friends are so fond of grapes, Aki decided to host a grape party with them. He has prepared a box with $a$ green grapes, $b$ purple grapes and $c$ black grapes.</p><p>However, Aki isn't sure if the box he prepared contains enough grapes to make everyone happy. Can you please find out whether it's possible to distribute grapes so that everyone is happy or Aki has to buy some more grapes?</p><p>It is not required to distribute all the grapes, so it's possible that some of them will remain unused.</p></div><div class="input-specification"><p>The first line contains three integers $x$, $y$ and $z$ ($1 \le x, y, z \le 10^5$)&nbsp;— the number of grapes Andrew, Dmitry and Michal want to eat.</p><p>The second line contains three integers $a$, $b$, $c$ ($1 \le a, b, c \le 10^5$)&nbsp;— the number of green, purple and black grapes in the box.</p></div><div class="output-specification"><p>If there is a grape distribution that allows everyone to be happy, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains three integers $x$, $y$ and $z$ ($1 \le x, y, z \le 10^5$)&nbsp;— the number of grapes Andrew, Dmitry and Michal want to eat.</p><p>The second line contains three integers $a$, $b$, $c$ ($1 \le a, b, c \le 10^5$)&nbsp;— the number of green, purple and black grapes in the box.</p>

## Output

<p>If there is a grape distribution that allows everyone to be happy, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
1 6 2
4 3 3

```




```input2
5 1 1
4 3 2

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example, there is only one possible distribution:</p><p>Andrew should take $1$ green grape, Dmitry should take $3$ remaining green grapes and $3$ purple grapes, and Michal will take $2$ out of $3$ available black grapes.</p><p>In the second test, there is no possible distribution, since Andrew is not be able to eat enough green grapes. :(</p>
