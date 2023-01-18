## Description

<div><p>A very tense moment: <span class="tex-span"><i>n</i></span> cowboys stand in a circle and each one points his colt at a neighbor. Each cowboy can point the colt to the person who follows or precedes him in clockwise direction. Human life is worthless, just like in any real western.</p><p>The picture changes each second! Every second the cowboys analyse the situation and, if a pair of cowboys realize that they aim at each other, they turn around. In a second all such pairs of neighboring cowboys aiming at each other turn around. All actions happen instantaneously and simultaneously in a second.</p><p>We'll use character "<span class="tex-font-style-tt">A</span>" to denote a cowboy who aims at his neighbour in the clockwise direction, and character "<span class="tex-font-style-tt">B</span>" for a cowboy who aims at his neighbour in the counter clockwise direction. Then a string of letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">B</span>" will denote the circle of cowboys, the record is made from the first of them in a clockwise direction.</p><p>For example, a circle that looks like "<span class="tex-font-style-tt">ABBBABBBA</span>" after a second transforms into "<span class="tex-font-style-tt">BABBBABBA</span>" and a circle that looks like "<span class="tex-font-style-tt">BABBA</span>" transforms into "<span class="tex-font-style-tt">ABABB</span>".</p><center> <img class="tex-graphics" src="file://jNlRhsNH.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-script"> This picture illustrates how the circle "<span class="tex-font-style-tt">BABBA</span>" transforms into "<span class="tex-font-style-tt">ABABB</span>" </span> </center><p>A second passed and now the cowboys' position is described by string <span class="tex-span"><i>s</i></span>. Your task is to determine the number of possible states that lead to <span class="tex-span"><i>s</i></span> in a second. Two states are considered distinct if there is a cowboy who aims at his clockwise neighbor in one state and at his counter clockwise neighbor in the other state.</p></div><div class="input-specification"><p>The input data consists of a single string <span class="tex-span"><i>s</i></span>. Its length is from 3 to 100 characters, inclusive. Line <span class="tex-span"><i>s</i></span> consists of letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">B</span>".</p></div><div class="output-specification"><p>Print the sought number of states.</p></div>

## Input

<p>The input data consists of a single string <span class="tex-span"><i>s</i></span>. Its length is from 3 to 100 characters, inclusive. Line <span class="tex-span"><i>s</i></span> consists of letters "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">B</span>".</p>

## Output

<p>Print the sought number of states.</p>





```input1
BABBBABBA

```




```input2
ABABB

```




```input3
ABABAB

```




```output1
2

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample the possible initial states are "<span class="tex-font-style-tt">ABBBABBAB</span>" and "<span class="tex-font-style-tt">ABBBABBBA</span>".</p><p>In the second sample the possible initial states are "<span class="tex-font-style-tt">AABBB</span>" and "<span class="tex-font-style-tt">BABBA</span>".</p>
