## Description

<div><p>Autocomplete is a program function that enables inputting the text (in editors, command line shells, browsers etc.) completing the text by its inputted part. Vasya is busy working on a new browser called 'BERowser'. He happens to be working on the autocomplete function in the address line at this very moment. A list consisting of <span class="tex-span"><i>n</i></span> last visited by the user pages and the inputted part <span class="tex-span"><i>s</i></span> are known. Your task is to complete <span class="tex-span"><i>s</i></span> to make it an address of one of the pages from the list. You have to find the lexicographically smallest address having a prefix <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains the <span class="tex-span"><i>s</i></span> line which is the inputted part. The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of visited pages. Then follow <span class="tex-span"><i>n</i></span> lines which are the visited pages, one on each line. All the lines have lengths of from <span class="tex-span">1</span> to <span class="tex-span">100</span> symbols inclusively and consist of lowercase Latin letters only.</p></div><div class="output-specification"><p>If <span class="tex-span"><i>s</i></span> is not the beginning of any of <span class="tex-span"><i>n</i></span> addresses of the visited pages, print <span class="tex-span"><i>s</i></span>. Otherwise, print the lexicographically minimal address of one of the visited pages starting from <span class="tex-span"><i>s</i></span>.</p><p>The lexicographical order is the order of words in a dictionary. The lexicographical comparison of lines is realized by the <span class="tex-font-style-tt">'&lt;'</span> operator in the modern programming languages.</p></div>

## Input

<p>The first line contains the <span class="tex-span"><i>s</i></span> line which is the inputted part. The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of visited pages. Then follow <span class="tex-span"><i>n</i></span> lines which are the visited pages, one on each line. All the lines have lengths of from <span class="tex-span">1</span> to <span class="tex-span">100</span> symbols inclusively and consist of lowercase Latin letters only.</p>

## Output

<p>If <span class="tex-span"><i>s</i></span> is not the beginning of any of <span class="tex-span"><i>n</i></span> addresses of the visited pages, print <span class="tex-span"><i>s</i></span>. Otherwise, print the lexicographically minimal address of one of the visited pages starting from <span class="tex-span"><i>s</i></span>.</p><p>The lexicographical order is the order of words in a dictionary. The lexicographical comparison of lines is realized by the <span class="tex-font-style-tt">'&lt;'</span> operator in the modern programming languages.</p>





```input1
next
2
nextpermutation
nextelement

```




```input2
find
4
find
findfirstof
findit
fand

```




```input3
find
4
fondfind
fondfirstof
fondit
fand

```




```output1
nextelement

```




```output2
find

```




```output3
find

```


