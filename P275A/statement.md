## Description

<div><p>Lenny is playing a game on a <span class="tex-span">3 × 3</span> grid of lights. In the beginning of the game all lights are switched on. Pressing any of the lights will toggle it and all side-adjacent lights. The goal of the game is to switch all the lights off. We consider the toggling as follows: if the light was switched on then it will be switched off, if it was switched off then it will be switched on.</p><p>Lenny has spent some time playing with the grid and by now he has pressed each light a certain number of times. Given the number of times each light is pressed, you have to print the current state of each light.</p></div><div class="input-specification"><p>The input consists of three rows. Each row contains three integers each between 0 to 100 inclusive. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th row is the number of times the <span class="tex-span"><i>j</i></span>-th light of the <span class="tex-span"><i>i</i></span>-th row of the grid is pressed.</p></div><div class="output-specification"><p>Print three lines, each containing three characters. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is "<span class="tex-font-style-tt">1</span>" if and only if the corresponding light is switched on, otherwise it's "<span class="tex-font-style-tt">0</span>".</p></div>

## Input

<p>The input consists of three rows. Each row contains three integers each between 0 to 100 inclusive. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th row is the number of times the <span class="tex-span"><i>j</i></span>-th light of the <span class="tex-span"><i>i</i></span>-th row of the grid is pressed.</p>

## Output

<p>Print three lines, each containing three characters. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is "<span class="tex-font-style-tt">1</span>" if and only if the corresponding light is switched on, otherwise it's "<span class="tex-font-style-tt">0</span>".</p>





```input1
1 0 0
0 0 0
0 0 1

```




```input2
1 0 1
8 8 8
2 0 3

```




```output1
001
010
100

```




```output2
010
011
100

```


