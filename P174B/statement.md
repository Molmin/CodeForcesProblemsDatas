## Description

<div><p>Eudokimus, a system administrator is in trouble again. As a result of an error in some script, a list of names of very important files has been damaged. Since they were files in the BerFS file system, it is known that each file name has a form "<span class="tex-font-style-tt">name.ext</span>", where: </p><ul> <li> <span class="tex-font-style-tt">name</span> is a string consisting of lowercase Latin letters, its length is from 1 to 8 characters; </li><li> <span class="tex-font-style-tt">ext</span> is a string consisting of lowercase Latin letters, its length is from 1 to 3 characters. </li></ul><p>For example, "<span class="tex-font-style-tt">read.me</span>", "<span class="tex-font-style-tt">example.txt</span>" and "<span class="tex-font-style-tt">b.cpp</span>" are valid file names and "<span class="tex-font-style-tt">version.info</span>", "<span class="tex-font-style-tt">ntldr</span>" and "<span class="tex-font-style-tt">contestdata.zip</span>" are not.</p><p>Damage to the list meant that all the file names were recorded one after another, without any separators. So now Eudokimus has a single string.</p><p>Eudokimus needs to set everything right as soon as possible. He should divide the resulting string into parts so that each part would be a valid file name in BerFS. Since Eudokimus has already proved that he is not good at programming, help him. The resulting file list can contain the same file names.</p></div><div class="input-specification"><p>The input data consists of a single string <span class="tex-span"><i>s</i></span>, its length is from <span class="tex-span">1</span> to <span class="tex-span">4·10<sup class="upper-index">5</sup></span> characters. The string can contain only lowercase Latin letters ('<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">z</span>') and periods ('<span class="tex-font-style-tt">.</span>').</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to divide <span class="tex-span"><i>s</i></span> into parts as required. In this case, the following lines should contain the parts of the required partition, one per line in the order in which they appear in <span class="tex-span"><i>s</i></span>. The required partition can contain the same file names. If there are multiple solutions, print any of them.</p><p>If the solution does not exist, then print in a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The input data consists of a single string <span class="tex-span"><i>s</i></span>, its length is from <span class="tex-span">1</span> to <span class="tex-span">4·10<sup class="upper-index">5</sup></span> characters. The string can contain only lowercase Latin letters ('<span class="tex-font-style-tt">a</span>' - '<span class="tex-font-style-tt">z</span>') and periods ('<span class="tex-font-style-tt">.</span>').</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to divide <span class="tex-span"><i>s</i></span> into parts as required. In this case, the following lines should contain the parts of the required partition, one per line in the order in which they appear in <span class="tex-span"><i>s</i></span>. The required partition can contain the same file names. If there are multiple solutions, print any of them.</p><p>If the solution does not exist, then print in a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
read.meexample.txtb.cpp

```




```input2
version.infontldrcontestdata.zip

```




```output1
YES
read.m
eexample.t
xtb.cpp

```




```output2
NO

```


