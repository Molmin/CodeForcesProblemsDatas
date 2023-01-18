## Description

<div><p>Hibiki and Dita are in love with each other, but belong to communities that are in a long lasting conflict. Hibiki is deeply concerned with the state of affairs, and wants to figure out if his relationship with Dita is an act of love or an act of treason.</p><center> <img class="tex-graphics" height="268px" src="file://G3hW4Osx.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>Hibiki prepared several binary features his decision will depend on, and built a three layer logical circuit on top of them, each layer consisting of one or more <a href="https://en.wikipedia.org/wiki/Logic_gate">logic gates</a>. Each gate in the circuit is either "<span class="tex-font-style-tt">or</span>", "<span class="tex-font-style-tt">and</span>", "<span class="tex-font-style-tt">nor</span>" (not or) or "<span class="tex-font-style-tt">nand</span>" (not and). Each gate in the first layer is connected to exactly two features. Each gate in the second layer is connected to exactly two gates in the first layer. The third layer has only one "<span class="tex-font-style-tt">or</span>" gate, which is connected to all the gates in the second layer (in other words, the entire circuit produces 1 if and only if at least one gate in the second layer produces 1).</p><p>The problem is, Hibiki knows very well that when the person is in love, his ability to think logically degrades drastically. In particular, it is well known that when a person in love evaluates a logical circuit in his mind, every gate evaluates to a value that is the opposite of what it was supposed to evaluate to. For example, "<span class="tex-font-style-tt">or</span>" gates return 1 if and only if both inputs are zero, "t{nand}" gates produce 1 if and only if both inputs are one etc.</p><p>In particular, the "<span class="tex-font-style-tt">or</span>" gate in the last layer also produces opposite results, and as such if Hibiki is in love, the entire circuit produces 1 if and only if all the gates on the second layer produced 0.</p><p>Hibiki can’t allow love to affect his decision. He wants to know what is the smallest number of gates that needs to be removed from the second layer so that the output of the circuit for all possible inputs doesn't depend on whether Hibiki is in love or not.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, $k$ ($2 \le n, m \le 50$; $1 \le k \le 50$) — the number of input features, the number of gates in the first layer, and the number of gates in the second layer correspondingly.</p><p>The second line contains $m$ pairs of strings separated by spaces describing the first layer. The first string in each pair describes the gate ("<span class="tex-font-style-tt">and</span>", "<span class="tex-font-style-tt">or</span>", "<span class="tex-font-style-tt">nand</span>" or "<span class="tex-font-style-tt">nor</span>"), and the second string describes the two input features the gate is connected two as a string consisting of exactly $n$ characters, with exactly two characters (that correspond to the input features the gate is connected to) equal to '<span class="tex-font-style-tt">x</span>' and the remaining characters equal to "<span class="tex-font-style-tt">.</span>'.</p><p>The third line contains $k$ pairs of strings separated by spaces describing the second layer in the same format, where the strings that describe the input parameters have length $m$ and correspond to the gates of the first layer.</p></div><div class="output-specification"><p>Print the number of gates that need to be removed from the second layer so that the output of the remaining circuit doesn't depend on whether Hibiki is in love or not.</p><p>If no matter how many gates are removed the output of the circuit continues to depend on Hibiki's feelings, print $-1$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, $k$ ($2 \le n, m \le 50$; $1 \le k \le 50$) — the number of input features, the number of gates in the first layer, and the number of gates in the second layer correspondingly.</p><p>The second line contains $m$ pairs of strings separated by spaces describing the first layer. The first string in each pair describes the gate ("<span class="tex-font-style-tt">and</span>", "<span class="tex-font-style-tt">or</span>", "<span class="tex-font-style-tt">nand</span>" or "<span class="tex-font-style-tt">nor</span>"), and the second string describes the two input features the gate is connected two as a string consisting of exactly $n$ characters, with exactly two characters (that correspond to the input features the gate is connected to) equal to '<span class="tex-font-style-tt">x</span>' and the remaining characters equal to "<span class="tex-font-style-tt">.</span>'.</p><p>The third line contains $k$ pairs of strings separated by spaces describing the second layer in the same format, where the strings that describe the input parameters have length $m$ and correspond to the gates of the first layer.</p>

## Output

<p>Print the number of gates that need to be removed from the second layer so that the output of the remaining circuit doesn't depend on whether Hibiki is in love or not.</p><p>If no matter how many gates are removed the output of the circuit continues to depend on Hibiki's feelings, print $-1$.</p>





```input1
2 2 2
and xx nand xx
and xx or xx

```




```input2
3 2 2
and xx. nor .xx
and xx nor xx

```




```input3
4 4 5
nor x..x and ..xx and xx.. nand xx..
nand ..xx nor ..xx and xx.. nor ..xx or ..xx

```




```output1
1

```




```output2
-1

```




```output3
2

```



## Note

<p>In the first example the two gates in the first layer are connected to the same inputs, but first computes "<span class="tex-font-style-tt">and</span>" while second computes "<span class="tex-font-style-tt">nand</span>", and as such their output is always different no matter what the input is and whether Hibiki is in love or not. The second layer has "<span class="tex-font-style-tt">or</span>" and "<span class="tex-font-style-tt">and</span>" gates both connected to the two gates in the first layer. If Hibiki is not in love, the "<span class="tex-font-style-tt">and</span>" gate will produce 0 and the "<span class="tex-font-style-tt">or</span>" gate will produce 1 no matter what input features are equal to, with the final "<span class="tex-font-style-tt">or</span>" gate in the third layer always producing the final answer of 1. If Hibiki is in love, "<span class="tex-font-style-tt">and</span>" gate in the second layer will produce 1 and "<span class="tex-font-style-tt">or</span>" gate will produce 0 no matter what the input is, with the final "<span class="tex-font-style-tt">or</span>" gate in the third layer producing the final answer of 0. Thus, if both gates in the second layer are kept, the output of the circuit does depend on whether Hibiki is in love. If any of the two gates in the second layer is dropped, the output of the circuit will no longer depend on whether Hibiki is in love or not, and hence the answer is 1.</p><p>In the second example no matter what gates are left in the second layer, the output of the circuit will depend on whether Hibiki is in love or not.</p><p>In the third example if Hibiki keeps second, third and fourth gates in the second layer, the circuit will not depend on whether Hibiki is in love or not. Alternatively, he can keep the first and the last gates. The former requires removing two gates, the latter requires removing three gates, so the former is better, and the answer is 2.</p>
