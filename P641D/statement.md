## Description

<div><p>Little Artyom decided to study probability theory. He found a book with a lot of nice exercises and now wants you to help him with one of them.</p><p>Consider two dices. When thrown each dice shows some integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive. For each dice the probability of each outcome is given (of course, their sum is <span class="tex-span">1</span>), and different dices may have different probability distributions.</p><p>We throw both dices simultaneously and then calculate values <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>)</span> and <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span>, where <span class="tex-span"><i>a</i></span> is equal to the outcome of the first dice, while <span class="tex-span"><i>b</i></span> is equal to the outcome of the second dice. You don't know the probability distributions for particular values on each dice, but you know the probability distributions for <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>)</span> and <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span>. That is, for each <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> you know the probability that <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>)</span> would be equal to <span class="tex-span"><i>x</i></span> and the probability that <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span> would be equal to <span class="tex-span"><i>x</i></span>. Find any valid probability distribution for values on the dices. It's guaranteed that the input data is consistent, that is, at least one solution exists.</p></div><div class="input-specification"><p>First line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of different values for both dices.</p><p>Second line contains an array consisting of <span class="tex-span"><i>n</i></span> real values with up to 8 digits after the decimal point &nbsp;— probability distribution for <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>)</span>, the <span class="tex-span"><i>i</i></span>-th of these values equals to the probability that <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>) = <i>i</i></span>. It's guaranteed that the sum of these values for one dice is <span class="tex-span">1</span>. The third line contains the description of the distribution <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span> in the same format.</p></div><div class="output-specification"><p>Output two descriptions of the probability distribution for <span class="tex-span"><i>a</i></span> on the first line and for <span class="tex-span"><i>b</i></span> on the second line. </p><p>The answer will be considered correct if each value of max(<span class="tex-span"><i>a</i>, <i>b</i></span>) and min(<span class="tex-span"><i>a</i>, <i>b</i></span>) probability distribution values does not differ by more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> from ones given in input. Also, probabilities should be non-negative and their sums should differ from <span class="tex-span">1</span> by no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>First line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of different values for both dices.</p><p>Second line contains an array consisting of <span class="tex-span"><i>n</i></span> real values with up to 8 digits after the decimal point &nbsp;— probability distribution for <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>)</span>, the <span class="tex-span"><i>i</i></span>-th of these values equals to the probability that <span class="tex-span"><i>max</i>(<i>a</i>, <i>b</i>) = <i>i</i></span>. It's guaranteed that the sum of these values for one dice is <span class="tex-span">1</span>. The third line contains the description of the distribution <span class="tex-span"><i>min</i>(<i>a</i>, <i>b</i>)</span> in the same format.</p>

## Output

<p>Output two descriptions of the probability distribution for <span class="tex-span"><i>a</i></span> on the first line and for <span class="tex-span"><i>b</i></span> on the second line. </p><p>The answer will be considered correct if each value of max(<span class="tex-span"><i>a</i>, <i>b</i></span>) and min(<span class="tex-span"><i>a</i>, <i>b</i></span>) probability distribution values does not differ by more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> from ones given in input. Also, probabilities should be non-negative and their sums should differ from <span class="tex-span">1</span> by no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
0.25 0.75
0.75 0.25

```




```input2
3
0.125 0.25 0.625
0.625 0.25 0.125

```




```output1
0.5 0.5 
0.5 0.5 

```




```output2
0.25 0.25 0.5 
0.5 0.25 0.25 

```


