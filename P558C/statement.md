## Description

<div><p>Amr loves Chemistry, and specially doing experiments. He is preparing for a new interesting experiment.</p><p>Amr has <span class="tex-span"><i>n</i></span> different types of chemicals. Each chemical <span class="tex-span"><i>i</i></span> has an initial volume of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> liters. For this experiment, Amr has to mix all the chemicals together, but all the chemicals volumes must be equal first. So his task is to make all the chemicals volumes equal.</p><p>To do this, Amr can do two different kind of operations. </p><ul> <li> Choose some chemical <span class="tex-span"><i>i</i></span> and double its current volume so the new volume will be <span class="tex-span">2<i>a</i><sub class="lower-index"><i>i</i></sub></span> </li><li> Choose some chemical <span class="tex-span"><i>i</i></span> and divide its volume by two (integer division) so the new volume will be <img align="middle" class="tex-formula" src="file://tk7RZfXJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul><p>Suppose that each chemical is contained in a vessel of infinite volume. Now Amr wonders what is the minimum number of operations required to make all the chemicals volumes equal?</p></div><div class="input-specification"><p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of chemicals.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), representing the initial volume of the <span class="tex-span"><i>i</i></span>-th chemical in liters.</p></div><div class="output-specification"><p>Output one integer the minimum number of operations required to make all the chemicals volumes equal.</p></div>

## Input

<p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of chemicals.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), representing the initial volume of the <span class="tex-span"><i>i</i></span>-th chemical in liters.</p>

## Output

<p>Output one integer the minimum number of operations required to make all the chemicals volumes equal.</p>





```input1
3
4 8 2

```




```input2
3
3 5 6

```




```output1
2
```




```output2
5
```



## Note

<p>In the first sample test, the optimal solution is to divide the second chemical volume by two, and multiply the third chemical volume by two to make all the volumes equal <span class="tex-span">4</span>.</p><p>In the second sample test, the optimal solution is to divide the first chemical volume by two, and divide the second and the third chemical volumes by two twice to make all the volumes equal <span class="tex-span">1</span>.</p>
