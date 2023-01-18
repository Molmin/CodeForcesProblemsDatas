## Description

<div><p>The INI file format is a de facto standard for configuration files. INI files are simple text files with a basic structure. They are commonly associated with Microsoft Windows, but are also used on other platforms.</p><p>Each line in INI-file stands for key-value mapping or defines new section. A key-value line has a format "<span class="tex-font-style-tt">key=value</span>",where <span class="tex-font-style-tt">key</span> — is the name of some property, and <span class="tex-font-style-tt">value</span> — it's value. It is possible that it will be spaces from the both sides of <span class="tex-font-style-tt">key</span> and/or <span class="tex-font-style-tt">value</span>, the spaces should be ignored.</p><p>A section line has a format "<span class="tex-font-style-tt">[section]</span>". It means that all key-value lines after it define properties of the specified section. Of cause, the following section line changes the current section. A section line may have spaces around any of brackets.</p><p>Also you should ignore comment lines — the first non-space character of comment line is "<span class="tex-font-style-tt">;</span>".</p><p>You task is to write the program which will format given INI-file in a special way: </p><ul> <li> first, print key-value lines which do not belong to any section; </li><li> print all the sections in the lexicographical (alphabetical) order of their names; </li><li> inside each of two previous items, order key-value lines lexicographically by "<span class="tex-font-style-tt">key</span>"; </li><li> if there are more than one key-value lines with the same key inside a single section (or outside any sections), leave only one line (which appears later in the input data); </li><li> remove all redundant spaces and lines. </li></ul></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 510</span>) — the number of lines in given INI-file.</p><p>The rest of the input contains a valid INI-file in <span class="tex-span"><i>n</i></span> lines. Values of <span class="tex-font-style-tt">section</span>, <span class="tex-font-style-tt">key</span> and <span class="tex-font-style-tt">value</span> contain only Latin letters, digits, "<span class="tex-font-style-tt">.</span>" and/or "<span class="tex-font-style-tt">-</span>".</p><p>Each line has length not exceeding 255 characters and not less than 1 character. The total length of all the lines does’t exceed 10000.</p></div><div class="output-specification"><p>Print formatted INI-file.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 510</span>) — the number of lines in given INI-file.</p><p>The rest of the input contains a valid INI-file in <span class="tex-span"><i>n</i></span> lines. Values of <span class="tex-font-style-tt">section</span>, <span class="tex-font-style-tt">key</span> and <span class="tex-font-style-tt">value</span> contain only Latin letters, digits, "<span class="tex-font-style-tt">.</span>" and/or "<span class="tex-font-style-tt">-</span>".</p><p>Each line has length not exceeding 255 characters and not less than 1 character. The total length of all the lines does’t exceed 10000.</p>

## Output

<p>Print formatted INI-file.</p>





```input1
11
a= 1
b=a
a = 2
 ; comment
[z]
1=2
[y]
2=3
[z]
2=1
[w]

```




```output1
a=2
b=a
[w]
[y]
2=3
[z]
1=2
2=1

```


