## Description

<div><p>In this problem, your task is to use ASCII graphics to paint a cardiogram. </p><p>A cardiogram is a polyline with the following corners:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://1yJwenU3.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>That is, a cardiogram is fully defined by a sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Your task is to paint a cardiogram by given sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span>. The next line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>. It is guaranteed that the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>max</i>&nbsp;|<i>y</i><sub class="lower-index"><i>i</i></sub> - <i>y</i><sub class="lower-index"><i>j</i></sub>|</span> lines (where <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> is the <span class="tex-span"><i>y</i></span> coordinate of the <span class="tex-span"><i>k</i></span>-th point of the polyline), in each line print <img align="middle" class="tex-formula" src="file://yMecuRp8.png" style="max-width: 100.0%;max-height: 100.0%;"> characters. Each character must equal either «<span class="tex-span"> / </span>» (slash), « <span class="tex-span">\</span> » (backslash), «<span class="tex-font-style-tt"> </span>» (space). The printed image must be the image of the given polyline. Please study the test samples for better understanding of how to print a cardiogram.</p><p><span class="tex-font-style-bf">Note</span> that in this problem the checker checks your answer taking spaces into consideration. Do not print any extra characters. Remember that the wrong answer to the first pretest doesn't give you a penalty.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span>. The next line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>. It is guaranteed that the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">1000</span>.</p>

## Output

<p>Print <span class="tex-span"><i>max</i>&nbsp;|<i>y</i><sub class="lower-index"><i>i</i></sub> - <i>y</i><sub class="lower-index"><i>j</i></sub>|</span> lines (where <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> is the <span class="tex-span"><i>y</i></span> coordinate of the <span class="tex-span"><i>k</i></span>-th point of the polyline), in each line print <img align="middle" class="tex-formula" src="file://yMecuRp8.png" style="max-width: 100.0%;max-height: 100.0%;"> characters. Each character must equal either «<span class="tex-span"> / </span>» (slash), « <span class="tex-span">\</span> » (backslash), «<span class="tex-font-style-tt"> </span>» (space). The printed image must be the image of the given polyline. Please study the test samples for better understanding of how to print a cardiogram.</p><p><span class="tex-font-style-bf">Note</span> that in this problem the checker checks your answer taking spaces into consideration. Do not print any extra characters. Remember that the wrong answer to the first pretest doesn't give you a penalty.</p>





```input1
5
3 1 2 5 1

```




```input2
3
1 5 1

```




```output1
<span class="tex-span"> / </span><span class="tex-span">\</span>     
  <span class="tex-span"> / </span><span class="tex-span">\</span><span class="tex-span"> / </span>  <span class="tex-span">\</span>    
 <span class="tex-span"> / </span>      <span class="tex-span">\</span>   
<span class="tex-span"> / </span>        <span class="tex-span">\</span>  
          <span class="tex-span">\</span><span class="tex-span"> / </span>

```




```output2
<span class="tex-span"> / </span><span class="tex-span">\</span>     
  <span class="tex-span">\</span>    
   <span class="tex-span">\</span>   
    <span class="tex-span">\</span>  
     <span class="tex-span">\</span><span class="tex-span"> / </span>

```



## Note

<p>Due to the technical reasons the answers for the samples cannot be copied from the statement. We've attached two text documents with the answers below.</p><p><span class="tex-font-style-tt">http://assets.codeforces.com/rounds/435/1.txt</span></p><p><span class="tex-font-style-tt">http://assets.codeforces.com/rounds/435/2.txt</span></p>
