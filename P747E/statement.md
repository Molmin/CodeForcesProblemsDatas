## Description

<div><p>A rare article in the Internet is posted without a possibility to comment it. On a Polycarp's website each article has comments feed.</p><p>Each comment on Polycarp's website is a non-empty string consisting of uppercase and lowercase letters of English alphabet. Comments have tree-like structure, that means each comment except root comments (comments of the highest level) has exactly one parent comment.</p><p>When Polycarp wants to save comments to his hard drive he uses the following format. Each comment he writes in the following format: </p><ul> <li> at first, the text of the comment is written; </li><li> after that the number of comments is written, for which this comment is a parent comment (i.&nbsp;e. the number of the replies to this comments); </li><li> after that the comments for which this comment is a parent comment are written (the writing of these comments uses the same algorithm). </li></ul> All elements in this format are separated by single comma. Similarly, the comments of the first level are separated by comma.<p>For example, if the comments look like:</p><center> <img class="tex-graphics" src="file://u5TKUFAb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>then the first comment is written as "<span class="tex-font-style-tt">hello,2,ok,0,bye,0</span>", the second is written as "<span class="tex-font-style-tt">test,0</span>", the third comment is written as "<span class="tex-font-style-tt">one,1,two,2,a,0,b,0</span>". The whole comments feed is written as: "<span class="tex-font-style-tt">hello,2,ok,0,bye,0,test,0,one,1,two,2,a,0,b,0</span>". For a given comments feed in the format specified above print the comments in a different format: </p><ul> <li> at first, print a integer <span class="tex-span"><i>d</i></span>&nbsp;— the maximum depth of nesting comments; </li><li> after that print <span class="tex-span"><i>d</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them corresponds to nesting level <span class="tex-span"><i>i</i></span>; </li><li> for the <span class="tex-span"><i>i</i></span>-th row print comments of nesting level <span class="tex-span"><i>i</i></span> in the order of their appearance in the Policarp's comments feed, separated by space. </li></ul></div><div class="input-specification"><p>The first line contains non-empty comments feed in the described format. It consists of uppercase and lowercase letters of English alphabet, digits and commas. </p><p>It is guaranteed that each comment is a non-empty string consisting of uppercase and lowercase English characters. Each of the number of comments is integer (consisting of at least one digit), and either equals <span class="tex-span">0</span> or does not contain leading zeros.</p><p>The length of the whole string does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. It is guaranteed that given structure of comments is valid. </p></div><div class="output-specification"><p>Print comments in a format that is given in the statement. For each level of nesting, comments should be printed in the order they are given in the input.</p></div>

## Input

<p>The first line contains non-empty comments feed in the described format. It consists of uppercase and lowercase letters of English alphabet, digits and commas. </p><p>It is guaranteed that each comment is a non-empty string consisting of uppercase and lowercase English characters. Each of the number of comments is integer (consisting of at least one digit), and either equals <span class="tex-span">0</span> or does not contain leading zeros.</p><p>The length of the whole string does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. It is guaranteed that given structure of comments is valid. </p>

## Output

<p>Print comments in a format that is given in the statement. For each level of nesting, comments should be printed in the order they are given in the input.</p>





```input1
hello,2,ok,0,bye,0,test,0,one,1,two,2,a,0,b,0

```




```input2
a,5,A,0,a,0,A,0,a,0,A,0

```




```input3
A,3,B,2,C,0,D,1,E,0,F,1,G,0,H,1,I,1,J,0,K,1,L,0,M,2,N,0,O,1,P,0

```




```output1
3
hello test one 
ok bye two 
a b 

```




```output2
2
a 
A a A a A 

```




```output3
4
A K M 
B F H L N O 
C D G I P 
E J 

```



## Note

<p>The first example is explained in the statements. </p>
