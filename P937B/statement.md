## Description

<div><p>The weather is fine today and hence it's high time to climb the nearby pine and enjoy the landscape.</p><p>The pine's trunk includes several branches, located one above another and numbered from <span class="tex-span">2</span> to <span class="tex-span"><i>y</i></span>. Some of them (more precise, from <span class="tex-span">2</span> to <span class="tex-span"><i>p</i></span>) are occupied by tiny vile grasshoppers which you're at war with. These grasshoppers are known for their awesome jumping skills: the grasshopper at branch <span class="tex-span"><i>x</i></span> can jump to branches <img align="middle" class="tex-formula" src="file://lVOzVbS3.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Keeping this in mind, you wisely decided to choose such a branch that none of the grasshoppers could interrupt you. At the same time you wanna settle as high as possible since the view from up there is simply breathtaking.</p><p>In other words, your goal is to find the highest branch that cannot be reached by any of the grasshoppers or report that it's impossible.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(2 ≤ <i>p</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output the number of the highest suitable branch. If there are none, print <span class="tex-font-style-tt">-1</span> instead.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(2 ≤ <i>p</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output the number of the highest suitable branch. If there are none, print <span class="tex-font-style-tt">-1</span> instead.</p>





```input1
3 6

```




```input2
3 4

```




```output1
5

```




```output2
-1

```



## Note

<p>In the first sample case grasshopper from branch <span class="tex-span">2</span> reaches branches <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">6</span> while branch <span class="tex-span">3</span> is initially settled by another grasshopper. Therefore the answer is <span class="tex-span">5</span>.</p><p>It immediately follows that there are no valid branches in second sample case.</p>
