## Description

<div><p>Sergei B., the young coach of Pokemons, has found the big house which consists of <span class="tex-span"><i>n</i></span> flats ordered in a row from left to right. It is possible to enter each flat from the street. It is possible to go out from each flat. Also, each flat is connected with the flat to the left and the flat to the right. Flat number <span class="tex-span">1</span> is only connected with the flat number <span class="tex-span">2</span> and the flat number <span class="tex-span"><i>n</i></span> is only connected with the flat number <span class="tex-span"><i>n</i> - 1</span>.</p><p>There is exactly one Pokemon of some type in each of these flats. Sergei B. asked residents of the house to let him enter their flats in order to catch Pokemons. After consulting the residents of the house decided to let Sergei B. enter one flat from the street, visit several flats and then go out from some flat. But they won't let him visit the same flat more than once. </p><p>Sergei B. was very pleased, and now he wants to visit as few flats as possible in order to collect Pokemons of all types that appear in this house. Your task is to help him and determine this minimum number of flats he has to visit. </p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of flats in the house.</p><p>The second line contains the row <span class="tex-span"><i>s</i></span> with the length <span class="tex-span"><i>n</i></span>, it consists of uppercase and lowercase letters of English alphabet, the <span class="tex-span"><i>i</i></span>-th letter equals the type of Pokemon, which is in the flat number <span class="tex-span"><i>i</i></span>. </p></div><div class="output-specification"><p>Print the minimum number of flats which Sergei B. should visit in order to catch Pokemons of all types which there are in the house. </p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of flats in the house.</p><p>The second line contains the row <span class="tex-span"><i>s</i></span> with the length <span class="tex-span"><i>n</i></span>, it consists of uppercase and lowercase letters of English alphabet, the <span class="tex-span"><i>i</i></span>-th letter equals the type of Pokemon, which is in the flat number <span class="tex-span"><i>i</i></span>. </p>

## Output

<p>Print the minimum number of flats which Sergei B. should visit in order to catch Pokemons of all types which there are in the house. </p>





```input1
3
AaA

```




```input2
7
bcAAcbc

```




```input3
6
aaBCCe

```




```output1
2

```




```output2
3

```




```output3
5

```



## Note

<p>In the first test Sergei B. can begin, for example, from the flat number <span class="tex-span">1</span> and end in the flat number <span class="tex-span">2</span>.</p><p>In the second test Sergei B. can begin, for example, from the flat number <span class="tex-span">4</span> and end in the flat number <span class="tex-span">6</span>. </p><p>In the third test Sergei B. must begin from the flat number <span class="tex-span">2</span> and end in the flat number <span class="tex-span">6</span>.</p>
