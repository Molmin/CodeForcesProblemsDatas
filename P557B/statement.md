## Description

<div><p>Pasha decided to invite his friends to a tea party. For that occasion, he has a large teapot with the capacity of <span class="tex-span"><i>w</i></span> milliliters and <span class="tex-span">2<i>n</i></span> tea cups, each cup is for one of Pasha's friends. The <span class="tex-span"><i>i</i></span>-th cup can hold at most <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> milliliters of water.</p><p>It turned out that among Pasha's friends there are exactly <span class="tex-span"><i>n</i></span> boys and exactly <span class="tex-span"><i>n</i></span> girls and all of them are going to come to the tea party. To please everyone, Pasha decided to pour the water for the tea as follows:</p><ul> <li> Pasha can boil the teapot exactly once by pouring there at most <span class="tex-span"><i>w</i></span> milliliters of water; </li><li> Pasha pours the same amount of water to each girl; </li><li> Pasha pours the same amount of water to each boy; </li><li> if each girl gets <span class="tex-span"><i>x</i></span> milliliters of water, then each boy gets <span class="tex-span">2<i>x</i></span> milliliters of water. </li></ul><p>In the other words, each boy should get two times more water than each girl does.</p><p>Pasha is very kind and polite, so he wants to maximize the total amount of the water that he pours to his friends. Your task is to help him and determine the optimum distribution of cups between Pasha's friends.</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of Pasha's friends that are boys (equal to the number of Pasha's friends that are girls) and the capacity of Pasha's teapot in milliliters.</p><p>The second line of the input contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ 2<i>n</i></span>)&nbsp;—&nbsp;the capacities of Pasha's tea cups in milliliters.</p></div><div class="output-specification"><p>Print a single real number — the maximum total amount of water in milliliters that Pasha can pour to his friends without violating the given conditions. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of Pasha's friends that are boys (equal to the number of Pasha's friends that are girls) and the capacity of Pasha's teapot in milliliters.</p><p>The second line of the input contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ 2<i>n</i></span>)&nbsp;—&nbsp;the capacities of Pasha's tea cups in milliliters.</p>

## Output

<p>Print a single real number — the maximum total amount of water in milliliters that Pasha can pour to his friends without violating the given conditions. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 4
1 1 1 1

```




```input2
3 18
4 4 4 2 2 2

```




```input3
1 5
2 3

```




```output1
3
```




```output2
18
```




```output3
4.5
```



## Note

<p>Pasha also has candies that he is going to give to girls but that is another task...</p>
