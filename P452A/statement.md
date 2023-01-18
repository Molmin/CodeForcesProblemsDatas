## Description

<div><p>You are solving the crossword problem K from IPSC 2014. You solved all the clues except for one: who does Eevee evolve into? You are not very into pokemons, but quick googling helped you find out, that Eevee can evolve into eight different pokemons: Vaporeon, Jolteon, Flareon, Espeon, Umbreon, Leafeon, Glaceon, and Sylveon.</p><p>You know the length of the word in the crossword, and you already know some letters. Designers of the crossword made sure that the answer is unambiguous, so you can assume that exactly one pokemon out of the 8 that Eevee evolves into fits the length and the letters given. Your task is to find it.</p></div><div class="input-specification"><p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">6 ≤ <i>n</i> ≤ 8</span>) – the length of the string.</p><p>Next line contains a string consisting of <span class="tex-span"><i>n</i></span> characters, each of which is either a lower case english letter (indicating a known letter) or a dot character (indicating an empty cell in the crossword).</p></div><div class="output-specification"><p>Print a name of the pokemon that Eevee can evolve into that matches the pattern in the input. Use lower case letters only to print the name (in particular, do not capitalize the first letter).</p></div>

## Input

<p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">6 ≤ <i>n</i> ≤ 8</span>) – the length of the string.</p><p>Next line contains a string consisting of <span class="tex-span"><i>n</i></span> characters, each of which is either a lower case english letter (indicating a known letter) or a dot character (indicating an empty cell in the crossword).</p>

## Output

<p>Print a name of the pokemon that Eevee can evolve into that matches the pattern in the input. Use lower case letters only to print the name (in particular, do not capitalize the first letter).</p>





```input1
7
j......

```




```input2
7
...feon

```




```input3
7
.l.r.o.

```




```output1
jolteon

```




```output2
leafeon

```




```output3
flareon

```



## Note

<p>Here's a set of names in a form you can paste into your solution:</p><p>["vaporeon", "jolteon", "flareon", "espeon", "umbreon", "leafeon", "glaceon", "sylveon"]</p><p>{"vaporeon", "jolteon", "flareon", "espeon", "umbreon", "leafeon", "glaceon", "sylveon"}</p>
