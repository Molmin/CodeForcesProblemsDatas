## Description

<div><p>The stardate is 1983, and Princess Heidi is getting better at detecting the Death Stars. This time, two Rebel spies have yet again given Heidi two maps with the possible locations of the Death Star. Since she got rid of all double agents last time, she knows that both maps are correct, and indeed show the map of the solar system that contains the Death Star. However, this time the Empire has hidden the Death Star very well, and Heidi needs to find a place that appears on both maps in order to detect the Death Star.</p><p>The first map is an <span class="tex-span"><i>N</i> × <i>M</i></span> grid, each cell of which shows some type of cosmic object that is present in the corresponding quadrant of space. The second map is an <span class="tex-span"><i>M</i> × <i>N</i></span> grid. Heidi needs to align those two maps in such a way that they overlap over some <span class="tex-span"><i>M</i> × <i>M</i></span> section in which all cosmic objects are identical. Help Heidi by identifying where such an <span class="tex-span"><i>M</i> × <i>M</i></span> section lies within both maps.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>M</i> ≤ 200</span>, <span class="tex-span"><i>M</i> ≤ <i>N</i></span>). The next <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>M</i></span> lower-case Latin characters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span>), denoting the first map. Different characters correspond to different cosmic object types. The next <span class="tex-span"><i>M</i></span> lines each contain <span class="tex-span"><i>N</i></span> characters, describing the second map in the same format. </p></div><div class="output-specification"><p>The only line of the output should contain two space-separated integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, denoting that the section of size <span class="tex-span"><i>M</i> × <i>M</i></span> in the first map that starts at the <span class="tex-span"><i>i</i></span>-th row is equal to the section of the second map that starts at the <span class="tex-span"><i>j</i></span>-th column. Rows and columns are numbered starting from 1.</p><p>If there are several possible ways to align the maps, Heidi will be satisfied with any of those. It is guaranteed that a solution exists.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>M</i> ≤ 200</span>, <span class="tex-span"><i>M</i> ≤ <i>N</i></span>). The next <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>M</i></span> lower-case Latin characters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span>), denoting the first map. Different characters correspond to different cosmic object types. The next <span class="tex-span"><i>M</i></span> lines each contain <span class="tex-span"><i>N</i></span> characters, describing the second map in the same format. </p>

## Output

<p>The only line of the output should contain two space-separated integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, denoting that the section of size <span class="tex-span"><i>M</i> × <i>M</i></span> in the first map that starts at the <span class="tex-span"><i>i</i></span>-th row is equal to the section of the second map that starts at the <span class="tex-span"><i>j</i></span>-th column. Rows and columns are numbered starting from 1.</p><p>If there are several possible ways to align the maps, Heidi will be satisfied with any of those. It is guaranteed that a solution exists.</p>





```input1
10 5
somer
andom
noise
mayth
eforc
ebewi
thyou
hctwo
again
noise
somermayth
andomeforc
noiseebewi
againthyou
noisehctwo

```




```output1
4 6

```



## Note

<p>The 5-by-5 grid for the first test case looks like this: </p><pre class="verbatim"><br>mayth<br>eforc<br>ebewi<br>thyou<br>hctwo<br></pre>
