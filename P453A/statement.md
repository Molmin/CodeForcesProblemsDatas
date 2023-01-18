## Description

<div><p>Twilight Sparkle was playing Ludo with her friends Rainbow Dash, Apple Jack and Flutter Shy. But she kept losing. Having returned to the castle, Twilight Sparkle became interested in the dice that were used in the game.</p><p>The dice has <span class="tex-span"><i>m</i></span> faces: the first face of the dice contains a dot, the second one contains two dots, and so on, the <span class="tex-span"><i>m</i></span>-th face contains <span class="tex-span"><i>m</i></span> dots. Twilight Sparkle is sure that when the dice is tossed, each face appears with probability <img align="middle" class="tex-formula" src="file://QkKne504.png" style="max-width: 100.0%;max-height: 100.0%;">. Also she knows that each toss is independent from others. Help her to calculate the expected maximum number of dots she could get after tossing the dice <span class="tex-span"><i>n</i></span> times.</p></div><div class="input-specification"><p>A single line contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output a single real number corresponding to the expected maximum. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10 <sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>A single line contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output a single real number corresponding to the expected maximum. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10 <sup class="upper-index"> - 4</sup></span>.</p>





```input1
6 1

```




```input2
6 3

```




```input3
2 2

```




```output1
3.500000000000

```




```output2
4.958333333333

```




```output3
1.750000000000

```



## Note

<p>Consider the third test example. If you've made two tosses:</p><ol> <li> You can get 1 in the first toss, and 2 in the second. Maximum equals to 2. </li><li> You can get 1 in the first toss, and 1 in the second. Maximum equals to 1. </li><li> You can get 2 in the first toss, and 1 in the second. Maximum equals to 2. </li><li> You can get 2 in the first toss, and 2 in the second. Maximum equals to 2. </li></ol><p>The probability of each outcome is 0.25, that is expectation equals to: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://2T9iOPPO.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>You can read about expectation using the following link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Expected_value</span></p>
