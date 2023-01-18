## Description

<div><p>Little Petya often travels to his grandmother in the countryside. The grandmother has a large garden, which can be represented as a rectangle <span class="tex-span">1 × <i>n</i></span> in size, when viewed from above. This rectangle is divided into <span class="tex-span"><i>n</i></span> equal square sections. The garden is very unusual as each of the square sections possesses its own fixed height and due to the newest irrigation system we can create artificial rain above each section.</p><p>Creating artificial rain is an expensive operation. That's why we limit ourselves to creating the artificial rain only above one section. At that, the water from each watered section will flow into its neighbouring sections if their height does not exceed the height of the section. That is, for example, the garden can be represented by a <span class="tex-span">1 × 5</span> rectangle, where the section heights are equal to 4, 2, 3, 3, 2. Then if we create an artificial rain over any of the sections with the height of 3, the water will flow over all the sections, except the ones with the height of 4. See the illustration of this example at the picture:</p><center> <img class="tex-graphics" src="file://5dstjQND.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As Petya is keen on programming, he decided to find such a section that if we create artificial rain above it, the number of watered sections will be maximal. Help him. </p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>n</i></span> positive integers which are the height of the sections. All the numbers are no less than 1 and not more than 1000.</p></div><div class="output-specification"><p>Print a single number, the maximal number of watered sections if we create artificial rain above exactly one section.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The second line contains <span class="tex-span"><i>n</i></span> positive integers which are the height of the sections. All the numbers are no less than 1 and not more than 1000.</p>

## Output

<p>Print a single number, the maximal number of watered sections if we create artificial rain above exactly one section.</p>





```input1
1
2

```




```input2
5
1 2 1 2 1

```




```input3
8
1 2 1 1 1 3 3 4

```




```output1
1

```




```output2
3

```




```output3
6

```


