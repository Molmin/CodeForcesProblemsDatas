## Description

<div><p>There are <span class="tex-span"><i>n</i></span> knights sitting at the Round Table at an equal distance from each other. Each of them is either in a good or in a bad mood.</p><p>Merlin, the wizard predicted to King Arthur that the next month will turn out to be particularly fortunate if the <span class="tex-font-style-it">regular</span> polygon can be found. On all vertices of the polygon knights in a good mood should be located. Otherwise, the next month will bring misfortunes.</p><p>A convex polygon is regular if all its sides have same length and all his angles are equal. In this problem we consider only regular polygons with at least 3 vertices, i. e. only nondegenerated.</p><p>On a picture below some examples of such polygons are present. Green points mean knights in a good mood. Red points mean ones in a bad mood.</p><center> <img class="tex-graphics" src="file://jZw6yG5U.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>King Arthur knows the knights' moods. Help him find out if the next month will be fortunate or not.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span>, which is the number of knights at the round table (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains space-separated moods of all the <span class="tex-span"><i>n</i></span> knights in the order of passing them around the table. "1" means that the knight is in a good mood an "0" means that he is in a bad mood.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" without the quotes if the following month will turn out to be lucky. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span>, which is the number of knights at the round table (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains space-separated moods of all the <span class="tex-span"><i>n</i></span> knights in the order of passing them around the table. "1" means that the knight is in a good mood an "0" means that he is in a bad mood.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" without the quotes if the following month will turn out to be lucky. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3
1 1 1

```




```input2
6
1 0 1 1 1 0

```




```input3
6
1 0 0 1 0 1

```




```output1
YES
```




```output2
YES
```




```output3
NO
```


