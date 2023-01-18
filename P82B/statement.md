## Description

<div><p>Little Vasya likes very much to play with sets consisting of positive integers. To make the game more interesting, Vasya chose <span class="tex-span"><i>n</i></span> non-empty sets in such a way, that no two of them have common elements.</p><p>One day he wanted to show his friends just how interesting playing with numbers is. For that he wrote out all possible unions of two different sets on <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> pieces of paper. Then he shuffled the pieces of paper. He had written out the numbers in the unions in an arbitrary order.</p><p>For example, if <span class="tex-span"><i>n</i> = 4</span>, and the actual sets have the following form <span class="tex-span">{1, 3}</span>, <span class="tex-span">{5}</span>, <span class="tex-span">{2, 4}</span>, <span class="tex-span">{7}</span>, then the number of set pairs equals to six. The six pieces of paper can contain the following numbers: </p><ul> <li> <span class="tex-span">2, 7, 4</span>. </li><li> <span class="tex-span">1, 7, 3</span>; </li><li> <span class="tex-span">5, 4, 2</span>; </li><li> <span class="tex-span">1, 3, 5</span>; </li><li> <span class="tex-span">3, 1, 2, 4</span>; </li><li> <span class="tex-span">5, 7</span>. </li></ul><p>Then Vasya showed the pieces of paper to his friends, but kept the <span class="tex-span"><i>n</i></span> sets secret from them. His friends managed to calculate which sets Vasya had thought of in the first place. And how about you, can you restore the sets by the given pieces of paper?</p></div><div class="input-specification"><p>The first input file line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>), <span class="tex-span"><i>n</i></span> is the number of sets at Vasya's disposal. Then follow sets of numbers from the pieces of paper written on <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> lines. Each set starts with the number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), which is the number of numbers written of the <span class="tex-span"><i>i</i></span>-th piece of paper, and then follow <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 200</span>). All the numbers on the lines are separated by exactly one space. It is guaranteed that the input data is constructed according to the above given rules from <span class="tex-span"><i>n</i></span> non-intersecting sets.</p></div><div class="output-specification"><p>Print on <span class="tex-span"><i>n</i></span> lines Vasya's sets' description. The first number on the line shows how many numbers the current set has. Then the set should be recorded by listing its elements. Separate the numbers by spaces. Each number and each set should be printed exactly once. Print the sets and the numbers in the sets in any order. If there are several answers to that problem, print any of them.</p><p>It is guaranteed that there is a solution.</p></div>

## Input

<p>The first input file line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>), <span class="tex-span"><i>n</i></span> is the number of sets at Vasya's disposal. Then follow sets of numbers from the pieces of paper written on <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> lines. Each set starts with the number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), which is the number of numbers written of the <span class="tex-span"><i>i</i></span>-th piece of paper, and then follow <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 200</span>). All the numbers on the lines are separated by exactly one space. It is guaranteed that the input data is constructed according to the above given rules from <span class="tex-span"><i>n</i></span> non-intersecting sets.</p>

## Output

<p>Print on <span class="tex-span"><i>n</i></span> lines Vasya's sets' description. The first number on the line shows how many numbers the current set has. Then the set should be recorded by listing its elements. Separate the numbers by spaces. Each number and each set should be printed exactly once. Print the sets and the numbers in the sets in any order. If there are several answers to that problem, print any of them.</p><p>It is guaranteed that there is a solution.</p>





```input1
4
3 2 7 4
3 1 7 3
3 5 4 2
3 1 3 5
4 3 1 2 4
2 5 7

```




```input2
4
5 6 7 8 9 100
4 7 8 9 1
4 7 8 9 2
3 1 6 100
3 2 6 100
2 1 2

```




```input3
3
2 1 2
2 1 3
2 2 3

```




```output1
1 7 
2 2 4 
2 1 3 
1 5 

```




```output2
3 7 8 9 
2 6 100 
1 1 
1 2 

```




```output3
1 1 
1 2 
1 3 

```


