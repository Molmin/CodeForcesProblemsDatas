## Description

<div><p>Little Vitaly loves different algorithms. Today he has invented a new algorithm just for you. Vitaly's algorithm works with string <span class="tex-span"><i>s</i></span>, consisting of characters "<span class="tex-font-style-tt">x</span>" and "<span class="tex-font-style-tt">y</span>", and uses two following operations at runtime:</p><ol> <li> Find two consecutive characters in the string, such that the first of them equals "<span class="tex-font-style-tt">y</span>", and the second one equals "<span class="tex-font-style-tt">x</span>" and swap them. If there are several suitable pairs of characters, we choose the pair of characters that is located closer to the beginning of the string. </li><li> Find in the string two consecutive characters, such that the first of them equals "<span class="tex-font-style-tt">x</span>" and the second one equals "<span class="tex-font-style-tt">y</span>". Remove these characters from the string. If there are several suitable pairs of characters, we choose the pair of characters that is located closer to the beginning of the string. </li></ol><p>The input for the new algorithm is string <span class="tex-span"><i>s</i></span>, and the algorithm works as follows:</p><ol> <li> If you can apply at least one of the described operations to the string, go to step 2 of the algorithm. Otherwise, stop executing the algorithm and print the current string. </li><li> If you can apply operation 1, then apply it. Otherwise, apply operation 2. After you apply the operation, go to step 1 of the algorithm. </li></ol><p>Now Vitaly wonders, what is going to be printed as the result of the algorithm's work, if the input receives string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>. </p><p>It is guaranteed that the string only consists of characters "<span class="tex-font-style-tt">x</span>" and "<span class="tex-font-style-tt">y</span>". It is guaranteed that the string consists of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. It is guaranteed that as the result of the algorithm's execution won't be an empty string.</p></div><div class="output-specification"><p>In the only line print the string that is printed as the result of the algorithm's work, if the input of the algorithm input receives string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>. </p><p>It is guaranteed that the string only consists of characters "<span class="tex-font-style-tt">x</span>" and "<span class="tex-font-style-tt">y</span>". It is guaranteed that the string consists of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. It is guaranteed that as the result of the algorithm's execution won't be an empty string.</p>

## Output

<p>In the only line print the string that is printed as the result of the algorithm's work, if the input of the algorithm input receives string <span class="tex-span"><i>s</i></span>.</p>





```input1
x

```




```input2
yxyxy

```




```input3
xxxxxy

```




```output1
x

```




```output2
y

```




```output3
xxxx

```



## Note

<p>In the first test the algorithm will end after the first step of the algorithm, as it is impossible to apply any operation. Thus, the string won't change.</p><p>In the second test the transformation will be like this:</p><ol> <li> string "<span class="tex-font-style-tt">yxyxy</span>" transforms into string "<span class="tex-font-style-tt">xyyxy</span>"; </li><li> string "<span class="tex-font-style-tt">xyyxy</span>" transforms into string "<span class="tex-font-style-tt">xyxyy</span>"; </li><li> string "<span class="tex-font-style-tt">xyxyy</span>" transforms into string "<span class="tex-font-style-tt">xxyyy</span>"; </li><li> string "<span class="tex-font-style-tt">xxyyy</span>" transforms into string "<span class="tex-font-style-tt">xyy</span>"; </li><li> string "<span class="tex-font-style-tt">xyy</span>" transforms into string "<span class="tex-font-style-tt">y</span>". </li></ol><p>As a result, we've got string "<span class="tex-font-style-tt">y</span>". </p><p>In the third test case only one transformation will take place: string "<span class="tex-font-style-tt">xxxxxy</span>" transforms into string "<span class="tex-font-style-tt">xxxx</span>". Thus, the answer will be string "<span class="tex-font-style-tt">xxxx</span>".</p>
