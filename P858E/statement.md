## Description

<div><p>The All-Berland National Olympiad in Informatics has just ended! Now Vladimir wants to upload the contest from the Olympiad as a gym to a popular Codehorses website.</p><p>Unfortunately, the archive with Olympiad's data is a mess. For example, the files with tests are named arbitrary without any logic.</p><p>Vladimir wants to rename the files with tests so that their names are distinct integers starting from <span class="tex-span">1</span> without any gaps, namely, "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", ..., "<span class="tex-span"><i>n</i></span>', where <span class="tex-span"><i>n</i></span> is the total number of tests.</p><p>Some of the files contain tests from statements (examples), while others contain regular tests. It is possible that there are no examples, and it is possible that all tests are examples. Vladimir wants to rename the files so that the examples are the first several tests, all all the next files contain regular tests only.</p><p>The only operation Vladimir can perform is the "<span class="tex-font-style-tt">move</span>" command. Vladimir wants to write a script file, each of the lines in which is "<span class="tex-font-style-tt">move file_1 file_2</span>", that means that the file "<span class="tex-font-style-tt">file_1</span>" is to be renamed to "<span class="tex-font-style-tt">file_2</span>". If there is a file "<span class="tex-font-style-tt">file_2</span>" at the moment of this line being run, then this file is to be rewritten. After the line "<span class="tex-font-style-tt">move file_1 file_2</span>" the file "<span class="tex-font-style-tt">file_1</span>" doesn't exist, but there is a file "<span class="tex-font-style-tt">file_2</span>" with content equal to the content of "<span class="tex-font-style-tt">file_1</span>" before the "<span class="tex-font-style-tt">move</span>" command.</p><p>Help Vladimir to write the script file with the minimum possible number of lines so that after this script is run:</p><ul> <li> all examples are the first several tests having filenames "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", ..., "<span class="tex-span"><i>e</i></span>", where <span class="tex-span"><i>e</i></span> is the total number of examples; </li><li> all other files contain regular tests with filenames "<span class="tex-font-style-tt"><span class="tex-span"><i>e</i> + 1</span></span>", "<span class="tex-font-style-tt"><span class="tex-span"><i>e</i> + 2</span></span>", ..., "<span class="tex-span"><i>n</i></span>", where <span class="tex-span"><i>n</i></span> is the total number of all tests. </li></ul></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of files with tests.</p><p><span class="tex-span"><i>n</i></span> lines follow, each describing a file with test. Each line has a form of "<span class="tex-font-style-tt">name_i type_i</span>", where "<span class="tex-font-style-tt">name_i</span>" is the filename, and "<span class="tex-font-style-tt">type_i</span>" equals "<span class="tex-font-style-tt">1</span>", if the <span class="tex-span"><i>i</i></span>-th file contains an example test, and "<span class="tex-font-style-tt">0</span>" if it contains a regular test. Filenames of each file are strings of digits and small English letters with length from <span class="tex-span">1</span> to <span class="tex-span">6</span> characters. The filenames are guaranteed to be distinct.</p></div><div class="output-specification"><p>In the first line print the minimum number of lines in Vladimir's script file.</p><p>After that print the script file, each line should be "<span class="tex-font-style-tt">move file_1 file_2</span>", where "<span class="tex-font-style-tt">file_1</span>" is an existing at the moment of this line being run filename, and "<span class="tex-font-style-tt">file_2</span>" — is a string of digits and small English letters with length from <span class="tex-span">1</span> to <span class="tex-span">6</span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of files with tests.</p><p><span class="tex-span"><i>n</i></span> lines follow, each describing a file with test. Each line has a form of "<span class="tex-font-style-tt">name_i type_i</span>", where "<span class="tex-font-style-tt">name_i</span>" is the filename, and "<span class="tex-font-style-tt">type_i</span>" equals "<span class="tex-font-style-tt">1</span>", if the <span class="tex-span"><i>i</i></span>-th file contains an example test, and "<span class="tex-font-style-tt">0</span>" if it contains a regular test. Filenames of each file are strings of digits and small English letters with length from <span class="tex-span">1</span> to <span class="tex-span">6</span> characters. The filenames are guaranteed to be distinct.</p>

## Output

<p>In the first line print the minimum number of lines in Vladimir's script file.</p><p>After that print the script file, each line should be "<span class="tex-font-style-tt">move file_1 file_2</span>", where "<span class="tex-font-style-tt">file_1</span>" is an existing at the moment of this line being run filename, and "<span class="tex-font-style-tt">file_2</span>" — is a string of digits and small English letters with length from <span class="tex-span">1</span> to <span class="tex-span">6</span>.</p>





```input1
5
01 0
2 1
2extra 0
3 1
99 0

```




```input2
2
1 0
2 1

```




```input3
5
1 0
11 1
111 0
1111 1
11111 0

```




```output1
4
move 3 1
move 01 5
move 2extra 4
move 99 3

```




```output2
3
move 1 3
move 2 1
move 3 2
```




```output3
5
move 1 5
move 11 1
move 1111 2
move 111 4
move 11111 3

```


