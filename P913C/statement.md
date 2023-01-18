## Description

<div><p>A New Year party is not a New Year party without lemonade! As usual, you are expecting a lot of guests, and buying lemonade has already become a pleasant necessity.</p><p>Your favorite store sells lemonade in bottles of <span class="tex-span"><i>n</i></span> different volumes at different costs. A single bottle of type <span class="tex-span"><i>i</i></span> has volume <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup></span> liters and costs <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> roubles. The number of bottles of each type in the store can be considered infinite.</p><p>You want to buy at least <span class="tex-span"><i>L</i></span> liters of lemonade. How many roubles do you have to spend?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>L</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>; <span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of types of bottles in the store and the required amount of lemonade in liters, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the costs of bottles of different types.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the smallest number of roubles you have to pay in order to buy at least <span class="tex-span"><i>L</i></span> liters of lemonade.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>L</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>; <span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of types of bottles in the store and the required amount of lemonade in liters, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the costs of bottles of different types.</p>

## Output

<p>Output a single integer&nbsp;— the smallest number of roubles you have to pay in order to buy at least <span class="tex-span"><i>L</i></span> liters of lemonade.</p>





```input1
4 12
20 30 70 90

```




```input2
4 3
10000 1000 100 10

```




```input3
4 3
10 100 1000 10000

```




```input4
5 787787787
123456789 234567890 345678901 456789012 987654321

```




```output1
150

```




```output2
10

```




```output3
30

```




```output4
44981600785557577

```



## Note

<p>In the first example you should buy one 8-liter bottle for 90 roubles and two 2-liter bottles for 30 roubles each. In total you'll get 12 liters of lemonade for just 150 roubles.</p><p>In the second example, even though you need only 3 liters, it's cheaper to buy a single 8-liter bottle for 10 roubles.</p><p>In the third example it's best to buy three 1-liter bottles for 10 roubles each, getting three liters for 30 roubles.</p>
