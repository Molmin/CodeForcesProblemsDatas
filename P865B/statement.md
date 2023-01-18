## Description

<div><p>It's another Start[c]up finals, and that means there is pizza to order for the onsite contestants. There are only 2 types of pizza (obviously not, but let's just pretend for the sake of the problem), and all pizzas contain exactly <span class="tex-span"><i>S</i></span> slices.</p><p>It is known that the <span class="tex-span"><i>i</i></span>-th contestant will eat <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> slices of pizza, and gain <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> happiness for each slice of type 1 pizza they eat, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> happiness for each slice of type 2 pizza they eat. We can order any number of type 1 and type 2 pizzas, but we want to buy the minimum possible number of pizzas for all of the contestants to be able to eat their required number of slices. Given that restriction, what is the maximum possible total happiness that can be achieved?</p></div><div class="input-specification"><p>The first line of input will contain integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>S</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>S</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of contestants and the number of slices per pizza, respectively. <span class="tex-span"><i>N</i></span> lines follow.</p><p>The <span class="tex-span"><i>i</i></span>-th such line contains integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of slices the <span class="tex-span"><i>i</i></span>-th contestant will eat, the happiness they will gain from each type 1 slice they eat, and the happiness they will gain from each type 2 slice they eat, respectively.</p></div><div class="output-specification"><p>Print the maximum total happiness that can be achieved.</p></div>

## Input

<p>The first line of input will contain integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>S</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>S</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of contestants and the number of slices per pizza, respectively. <span class="tex-span"><i>N</i></span> lines follow.</p><p>The <span class="tex-span"><i>i</i></span>-th such line contains integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of slices the <span class="tex-span"><i>i</i></span>-th contestant will eat, the happiness they will gain from each type 1 slice they eat, and the happiness they will gain from each type 2 slice they eat, respectively.</p>

## Output

<p>Print the maximum total happiness that can be achieved.</p>





```input1
3 12
3 5 7
4 6 7
5 9 5

```




```input2
6 10
7 4 7
5 8 8
12 5 8
6 11 6
3 3 7
5 9 6

```




```output1
84

```




```output2
314

```



## Note

<p>In the first example, you only need to buy one pizza. If you buy a type 1 pizza, the total happiness will be <span class="tex-span">3·5 + 4·6 + 5·9 = 84</span>, and if you buy a type 2 pizza, the total happiness will be <span class="tex-span">3·7 + 4·7 + 5·5 = 74</span>.</p>
