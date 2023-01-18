## Description

<div><p>Dima, Inna and Seryozha have gathered in a room. That's right, someone's got to go. To cheer Seryozha up and inspire him to have a walk, Inna decided to cook something. </p><p>Dima and Seryozha have <span class="tex-span"><i>n</i></span> fruits in the fridge. Each fruit has two parameters: the taste and the number of calories. Inna decided to make a fruit salad, so she wants to take some fruits from the fridge for it. Inna follows a certain principle as she chooses the fruits: the total taste to the total calories ratio of the chosen fruits must equal <span class="tex-span"><i>k</i></span>. In other words, <img align="middle" class="tex-formula" src="file://rQado8uz.png" style="max-width: 100.0%;max-height: 100.0%;"> , where <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is the taste of the <span class="tex-span"><i>j</i></span>-th chosen fruit and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is its calories.</p><p>Inna hasn't chosen the fruits yet, she is thinking: what is the maximum taste of the chosen fruits if she strictly follows her principle? Help Inna solve this culinary problem — now the happiness of a young couple is in your hands!</p><p>Inna loves Dima very much so she wants to make the salad from at least one fruit.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 10)</span>. The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the fruits' tastes. The third line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the fruits' calories. Fruit number <span class="tex-span"><i>i</i></span> has taste <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and calories <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>If there is no way Inna can choose the fruits for the salad, print in the single line number -1. Otherwise, print a single integer — the maximum possible sum of the taste values of the chosen fruits.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 10)</span>. The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the fruits' tastes. The third line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the fruits' calories. Fruit number <span class="tex-span"><i>i</i></span> has taste <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and calories <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>If there is no way Inna can choose the fruits for the salad, print in the single line number -1. Otherwise, print a single integer — the maximum possible sum of the taste values of the chosen fruits.</p>





```input1
3 2
10 8 1
2 7 1

```




```input2
5 3
4 4 4 4 4
2 2 2 2 2

```




```output1
18

```




```output2
-1

```



## Note

<p>In the first test sample we can get the total taste of the fruits equal to 18 if we choose fruit number 1 and fruit number 2, then the total calories will equal 9. The condition <img align="middle" class="tex-formula" src="file://stj5t2mZ.png" style="max-width: 100.0%;max-height: 100.0%;"> fulfills, that's exactly what Inna wants.</p><p>In the second test sample we cannot choose the fruits so as to follow Inna's principle.</p>
