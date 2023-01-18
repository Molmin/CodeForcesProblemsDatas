## Description

<div><p>Kolya Gerasimov loves kefir very much. He lives in year 1984 and knows all the details of buying this delicious drink. One day, as you probably know, he found himself in year 2084, and buying kefir there is much more complicated.</p><p>Kolya is hungry, so he went to the nearest milk shop. In 2084 you may buy kefir in a plastic liter bottle, that costs <span class="tex-span"><i>a</i></span> rubles, or in glass liter bottle, that costs <span class="tex-span"><i>b</i></span> rubles. Also, you may return empty glass bottle and get <span class="tex-span"><i>c</i></span> (<span class="tex-span"><i>c</i> &lt; <i>b</i></span>) rubles back, but you cannot return plastic bottles.</p><p>Kolya has <span class="tex-span"><i>n</i></span> rubles and he is really hungry, so he wants to drink as much kefir as possible. There were no plastic bottles in his 1984, so Kolya doesn't know how to act optimally and asks for your help.</p></div><div class="input-specification"><p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of rubles Kolya has at the beginning.</p><p>Then follow three lines containing integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>c</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the cost of one plastic liter bottle, the cost of one glass liter bottle and the money one can get back by returning an empty glass bottle, respectively.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— maximum number of liters of kefir, that Kolya can drink.</p></div>

## Input

<p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of rubles Kolya has at the beginning.</p><p>Then follow three lines containing integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>c</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the cost of one plastic liter bottle, the cost of one glass liter bottle and the money one can get back by returning an empty glass bottle, respectively.</p>

## Output

<p>Print the only integer&nbsp;— maximum number of liters of kefir, that Kolya can drink.</p>





```input1
10
11
9
8

```




```input2
10
5
6
1

```




```output1
2

```




```output2
2

```



## Note

<p>In the first sample, Kolya can buy one glass bottle, then return it and buy one more glass bottle. Thus he will drink <span class="tex-span">2</span> liters of kefir.</p><p>In the second sample, Kolya can buy two plastic bottle and get two liters of kefir, or he can buy one liter glass bottle, then return it and buy one plastic bottle. In both cases he will drink two liters of kefir.</p>
