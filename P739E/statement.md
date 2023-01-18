## Description

<div><p>Gosha is hunting. His goal is to catch as many Pokemons as possible. Gosha has <span class="tex-span"><i>a</i></span> Poke Balls and <span class="tex-span"><i>b</i></span> Ultra Balls. There are <span class="tex-span"><i>n</i></span> Pokemons. They are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Gosha knows that if he throws a Poke Ball at the <span class="tex-span"><i>i</i></span>-th Pokemon he catches it with probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. If he throws an Ultra Ball at the <span class="tex-span"><i>i</i></span>-th Pokemon he catches it with probability <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. He can throw at most one Ball of each type at any Pokemon.</p><p>The hunting proceeds as follows: at first, Gosha chooses no more than <span class="tex-span"><i>a</i></span> Pokemons at which he will throw Poke Balls and no more than <span class="tex-span"><i>b</i></span> Pokemons at which he will throw Ultra Balls. After that, he throws the chosen Balls at the chosen Pokemons. If he throws both Ultra Ball and Poke Ball at some Pokemon, he is caught if and only if he is caught by any of these Balls. The outcome of a throw doesn't depend on the other throws.</p><p>Gosha would like to know what is the expected number of the Pokemons he catches if he acts in an optimal way. In other words, he would like to know the maximum possible expected number of Pokemons can catch.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of Pokemons, the number of Poke Balls and the number of Ultra Balls.</p><p>The second line contains <span class="tex-span"><i>n</i></span> real values <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the probability of catching the <span class="tex-span"><i>i</i></span>-th Pokemon if Gosha throws a Poke Ball to it.</p><p>The third line contains <span class="tex-span"><i>n</i></span> real values <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the probability of catching the <span class="tex-span"><i>i</i></span>-th Pokemon if Gosha throws an Ultra Ball to it.</p><p>All the probabilities are given with exactly three digits after the decimal separator.</p></div><div class="output-specification"><p>Print the maximum possible expected number of Pokemons Gosha can catch. The answer is considered correct if it's absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of Pokemons, the number of Poke Balls and the number of Ultra Balls.</p><p>The second line contains <span class="tex-span"><i>n</i></span> real values <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the probability of catching the <span class="tex-span"><i>i</i></span>-th Pokemon if Gosha throws a Poke Ball to it.</p><p>The third line contains <span class="tex-span"><i>n</i></span> real values <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the probability of catching the <span class="tex-span"><i>i</i></span>-th Pokemon if Gosha throws an Ultra Ball to it.</p><p>All the probabilities are given with exactly three digits after the decimal separator.</p>

## Output

<p>Print the maximum possible expected number of Pokemons Gosha can catch. The answer is considered correct if it's absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3 2 2
1.000 0.000 0.500
0.000 1.000 0.500

```




```input2
4 1 3
0.100 0.500 0.500 0.600
0.100 0.500 0.900 0.400

```




```input3
3 2 0
0.412 0.198 0.599
0.612 0.987 0.443

```




```output1
2.75

```




```output2
2.16

```




```output3
1.011
```


