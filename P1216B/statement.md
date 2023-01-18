## Description

<div><p>Recently Vasya decided to improve his pistol shooting skills. Today his coach offered him the following exercise. He placed $n$ cans in a row on a table. Cans are numbered from left to right from $1$ to $n$. Vasya has to knock down each can exactly once to finish the exercise. He is allowed to choose <span class="tex-font-style-bf">the order</span> in which he will knock the cans down.</p><p>Vasya knows that the <span class="tex-font-style-it">durability</span> of the $i$-th can is $a_i$. It means that if Vasya has already knocked $x$ cans down and is now about to start shooting the $i$-th one, he will need $(a_i \cdot x + 1)$ shots to knock it down. You can assume that if Vasya starts shooting the $i$-th can, he will be shooting it until he knocks it down.</p><p>Your task is to choose such an order of shooting so that the number of shots required to knock each of the $n$ given cans down exactly once is minimum possible.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ $(2 \le n \le 1\,000)$ — the number of cans.</p><p>The second line of the input contains the sequence $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 1\,000)$, where $a_i$ is the durability of the $i$-th can.</p></div><div class="output-specification"><p>In the first line print the minimum number of shots required to knock each of the $n$ given cans down exactly once.</p><p>In the second line print the sequence consisting of $n$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $n$ — the order of indices of cans that minimizes the number of shots required. If there are several answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ $(2 \le n \le 1\,000)$ — the number of cans.</p><p>The second line of the input contains the sequence $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 1\,000)$, where $a_i$ is the durability of the $i$-th can.</p>

## Output

<p>In the first line print the minimum number of shots required to knock each of the $n$ given cans down exactly once.</p><p>In the second line print the sequence consisting of $n$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $n$ — the order of indices of cans that minimizes the number of shots required. If there are several answers, you can print any of them.</p>





```input1
3
20 10 20
```




```input2
4
10 10 10 10
```




```input3
6
5 4 5 4 4 5
```




```input4
2
1 4
```




```output1
43
1 3 2
```




```output2
64
2 1 4 3
```




```output3
69
6 1 3 5 2 4
```




```output4
3
2 1
```



## Note

<p>In the first example Vasya can start shooting from the first can. He knocks it down with the first shot because he haven't knocked any other cans down before. After that he has to shoot the third can. To knock it down he shoots $20 \cdot 1 + 1 = 21$ times. After that only second can remains. To knock it down Vasya shoots $10 \cdot 2 + 1 = 21$ times. So the total number of shots is $1 + 21 + 21 = 43$.</p><p>In the second example the order of shooting does not matter because all cans have the same durability.</p>
