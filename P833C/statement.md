## Description

<div><center> <img class="tex-graphics" src="file://SaxrB6tk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Recently, a wild Krakozyabra appeared at Jelly Castle. It is, truth to be said, always eager to have something for dinner.</p><p>Its favorite meal is natural numbers (typically served with honey sauce), or, to be more precise, the zeros in their corresponding decimal representations. As for other digits, Krakozyabra dislikes them; moreover, they often cause it indigestion! So, as a necessary precaution, Krakozyabra prefers to sort the digits of a number in non-descending order before proceeding to feast. Then, the leading zeros of the resulting number are eaten and the remaining part is discarded as an <span class="tex-font-style-it">inedible tail</span>.</p><p>For example, if Krakozyabra is to have the number <span class="tex-span">57040</span> for dinner, its <span class="tex-font-style-it">inedible tail</span> would be the number <span class="tex-span">457</span>.</p><p>Slastyona is not really fond of the idea of Krakozyabra living in her castle. Hovewer, her natural hospitality prevents her from leaving her guest without food. Slastyona has a range of natural numbers from <span class="tex-span"><i>L</i></span> to <span class="tex-span"><i>R</i></span>, which she is going to feed the guest with. Help her determine how many distinct <span class="tex-font-style-it">inedible tails</span> are going to be discarded by Krakozyabra by the end of the dinner.</p></div><div class="input-specification"><p>In the first and only string, the numbers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> are given&nbsp;– the boundaries of the range <span class="tex-span">(1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Output the sole number&nbsp;– the answer for the problem.</p></div>

## Input

<p>In the first and only string, the numbers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> are given&nbsp;– the boundaries of the range <span class="tex-span">(1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Output the sole number&nbsp;– the answer for the problem.</p>





```input1
1 10

```




```input2
40 57

```




```input3
157 165

```




```output1
9

```




```output2
17

```




```output3
9

```



## Note

<p>In the first sample case, the <span class="tex-font-style-it">inedible tails</span> are the numbers from <span class="tex-span">1</span> to <span class="tex-span">9</span>. Note that <span class="tex-span">10</span> and <span class="tex-span">1</span> have the same <span class="tex-font-style-it">inedible tail</span>&nbsp;– the number <span class="tex-span">1</span>.</p><p>In the second sample case, each number has a unique <span class="tex-font-style-it">inedible tail</span>, except for the pair <span class="tex-span">45, 54</span>. The answer to this sample case is going to be <span class="tex-span">(57 - 40 + 1) - 1 = 17</span>.</p>
