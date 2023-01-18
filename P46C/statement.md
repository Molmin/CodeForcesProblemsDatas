## Description

<div><p>Today there is going to be an unusual performance at the circus — hamsters and tigers will perform together! All of them stand in circle along the arena edge and now the trainer faces a difficult task: he wants to swap the animals' positions so that all the hamsters stood together and all the tigers also stood together. The trainer swaps the animals in pairs not to create a mess. He orders two animals to step out of the circle and swap places. As hamsters feel highly uncomfortable when tigers are nearby as well as tigers get nervous when there's so much potential prey around (consisting not only of hamsters but also of yummier spectators), the trainer wants to spend as little time as possible moving the animals, i.e. he wants to achieve it with the minimal number of swaps. Your task is to help him.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) which indicates the total number of animals in the arena. The second line contains the description of the animals' positions. The line consists of <span class="tex-span"><i>n</i></span> symbols "H" and "T". The "H"s correspond to hamsters and the "T"s correspond to tigers. It is guaranteed that at least one hamster and one tiger are present on the arena. The animals are given in the order in which they are located circle-wise, in addition, the last animal stands near the first one.</p></div><div class="output-specification"><p>Print the single number which is the minimal number of swaps that let the trainer to achieve his goal.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) which indicates the total number of animals in the arena. The second line contains the description of the animals' positions. The line consists of <span class="tex-span"><i>n</i></span> symbols "H" and "T". The "H"s correspond to hamsters and the "T"s correspond to tigers. It is guaranteed that at least one hamster and one tiger are present on the arena. The animals are given in the order in which they are located circle-wise, in addition, the last animal stands near the first one.</p>

## Output

<p>Print the single number which is the minimal number of swaps that let the trainer to achieve his goal.</p>





```input1
3
HTH

```




```input2
9
HTHTHTHHT

```




```output1
0

```




```output2
2

```



## Note

<p>In the first example we shouldn't move anybody because the animals of each species already stand apart from the other species. In the second example you may swap, for example, the tiger in position <span class="tex-span">2</span> with the hamster in position <span class="tex-span">5</span> and then — the tiger in position <span class="tex-span">9</span> with the hamster in position <span class="tex-span">7</span>.</p>
