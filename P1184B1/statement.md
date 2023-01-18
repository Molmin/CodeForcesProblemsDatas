## Description

<div><p>Heidi and Doctor Who hopped out of the TARDIS and found themselves at EPFL in 2018. They were surrounded by stormtroopers and Darth Vader was approaching. Miraculously, they managed to escape to a nearby rebel base but the Doctor was very confused. Heidi reminded him that last year's HC2 theme was Star Wars. Now he understood, and he's ready to face the evils of the Empire!</p><p>The rebels have $s$ spaceships, each with a certain attacking power $a$.</p><p>They want to send their spaceships to destroy the empire bases and steal enough gold and supplies in order to keep the rebellion alive.</p><p>The empire has $b$ bases, each with a certain defensive power $d$, and a certain amount of gold $g$.</p><p>A spaceship can attack all the bases which have a defensive power less than or equal to its attacking power.</p><p>If a spaceship attacks a base, it steals all the gold in that base.</p><p>The rebels are still undecided which spaceship to send out first, so they asked for the Doctor's help. They would like to know, for each spaceship, the maximum amount of gold it can steal.</p></div><div class="input-specification"><p>The first line contains integers $s$ and $b$ ($1 \leq s, b \leq 10^5$), the number of spaceships and the number of bases, respectively.</p><p>The second line contains $s$ integers $a$ ($0 \leq a \leq 10^9$), the attacking power of each spaceship.</p><p>The next $b$ lines contain integers $d, g$ ($0 \leq d \leq 10^9$, $0 \leq g \leq 10^4$), the defensive power and the gold of each base, respectively.</p></div><div class="output-specification"><p>Print $s$ integers, the maximum amount of gold each spaceship can steal, in the same order as the spaceships are given in the input.</p></div>

## Input

<p>The first line contains integers $s$ and $b$ ($1 \leq s, b \leq 10^5$), the number of spaceships and the number of bases, respectively.</p><p>The second line contains $s$ integers $a$ ($0 \leq a \leq 10^9$), the attacking power of each spaceship.</p><p>The next $b$ lines contain integers $d, g$ ($0 \leq d \leq 10^9$, $0 \leq g \leq 10^4$), the defensive power and the gold of each base, respectively.</p>

## Output

<p>Print $s$ integers, the maximum amount of gold each spaceship can steal, in the same order as the spaceships are given in the input.</p>





```input1
5 4
1 3 5 2 4
0 1
4 2
2 8
9 4
```




```output1
1 9 11 9 11
```



## Note

<p>The first spaceship can only attack the first base.</p><p>The second spaceship can attack the first and third bases.</p><p>The third spaceship can attack the first, second and third bases.</p>
