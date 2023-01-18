## Description

<div><p>There is the following puzzle popular among nuclear physicists.</p><p>A reactor contains a set of <span class="tex-span"><i>n</i></span> atoms of some chemical elements. We shall understand the phrase "atomic number" as the number of this atom's element in the periodic table of the chemical elements.</p><p>You are allowed to take any two different atoms and fuse a new one from them. That results in a new atom, whose number is equal to the sum of the numbers of original atoms. The fusion operation can be performed several times.</p><p>The aim is getting a new pregiven set of <span class="tex-span"><i>k</i></span> atoms.</p><p>The puzzle's difficulty is that it is only allowed to fuse two atoms into one, it is not allowed to split an atom into several atoms. You are suggested to try to solve the puzzle.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 17</span>). The second line contains space-separated symbols of elements of <span class="tex-span"><i>n</i></span> atoms, which are available from the start. The third line contains space-separated symbols of elements of <span class="tex-span"><i>k</i></span> atoms which need to be the result of the fusion. The symbols of the elements coincide with the symbols from the periodic table of the chemical elements. The atomic numbers do not exceed <span class="tex-span">100</span> (elements possessing larger numbers are highly unstable). Some atoms can have identical numbers (that is, there can be several atoms of the same element). The sum of numbers of initial atoms is equal to the sum of numbers of the atoms that need to be synthesized.</p></div><div class="output-specification"><p>If it is impossible to synthesize the required atoms, print "<span class="tex-font-style-tt">NO</span>" without the quotes. Otherwise, print on the first line «<span class="tex-font-style-tt">YES</span>», and on the next <span class="tex-span"><i>k</i></span> lines print the way of synthesizing each of <span class="tex-span"><i>k</i></span> atoms as equations. Each equation has the following form: "<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span><span class="tex-font-style-tt">+</span><span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span><span class="tex-font-style-tt">+</span><span class="tex-span">...</span><span class="tex-font-style-tt">+</span><span class="tex-span"><i>x</i><sub class="lower-index"><i>t</i></sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> is the symbol of the element of some atom from the original set, and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the symbol of the element of some atom from the resulting set. Each atom from the input data should occur in the output data exactly one time. The order of summands in the equations, as well as the output order does not matter. If there are several solutions, print any of them. For a better understanding of the output format, see the samples.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 17</span>). The second line contains space-separated symbols of elements of <span class="tex-span"><i>n</i></span> atoms, which are available from the start. The third line contains space-separated symbols of elements of <span class="tex-span"><i>k</i></span> atoms which need to be the result of the fusion. The symbols of the elements coincide with the symbols from the periodic table of the chemical elements. The atomic numbers do not exceed <span class="tex-span">100</span> (elements possessing larger numbers are highly unstable). Some atoms can have identical numbers (that is, there can be several atoms of the same element). The sum of numbers of initial atoms is equal to the sum of numbers of the atoms that need to be synthesized.</p>

## Output

<p>If it is impossible to synthesize the required atoms, print "<span class="tex-font-style-tt">NO</span>" without the quotes. Otherwise, print on the first line «<span class="tex-font-style-tt">YES</span>», and on the next <span class="tex-span"><i>k</i></span> lines print the way of synthesizing each of <span class="tex-span"><i>k</i></span> atoms as equations. Each equation has the following form: "<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span><span class="tex-font-style-tt">+</span><span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span><span class="tex-font-style-tt">+</span><span class="tex-span">...</span><span class="tex-font-style-tt">+</span><span class="tex-span"><i>x</i><sub class="lower-index"><i>t</i></sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> is the symbol of the element of some atom from the original set, and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the symbol of the element of some atom from the resulting set. Each atom from the input data should occur in the output data exactly one time. The order of summands in the equations, as well as the output order does not matter. If there are several solutions, print any of them. For a better understanding of the output format, see the samples.</p>





```input1
10 3
Mn Co Li Mg C P F Zn Sc K
Sn Pt Y

```




```input2
2 1
H H
He

```




```input3
2 2
Bk Fm
Cf Es

```




```output1
YES
Mn+C+K-&gt;Sn
Co+Zn+Sc-&gt;Pt
Li+Mg+P+F-&gt;Y

```




```output2
YES
H+H-&gt;He

```




```output3
NO

```



## Note

<p>The reactions from the first example possess the following form (the atomic number is written below and to the left of the element):</p><p><img align="middle" class="tex-formula" src="file://O9CoQlyB.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://IyH7uEJv.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://rkOjSV8O.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>To find a periodic table of the chemical elements, you may use your favorite search engine.</p><p>The pretest set contains each of the first <span class="tex-span">100</span> elements of the periodic table at least once. You can use that information to check for misprints.</p>
