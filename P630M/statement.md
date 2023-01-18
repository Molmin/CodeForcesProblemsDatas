## Description

<div><p>Vasya started working in a machine vision company of IT City. Vasya's team creates software and hardware for identification of people by their face.</p><p>One of the project's know-how is a camera rotating around its optical axis on shooting. People see an eye-catching gadget — a rotating camera — come up to it to see it better, look into it. And the camera takes their photo at that time. What could be better for high quality identification?</p><p>But not everything is so simple. The pictures from camera appear rotated too (on clockwise camera rotation frame the content becomes rotated counter-clockwise). But the identification algorithm can work only with faces that are just slightly deviated from vertical.</p><p>Vasya was entrusted to correct the situation — to rotate a captured image so that image would be minimally deviated from vertical. Requirements were severe. Firstly, the picture should be rotated only on angle divisible by 90 degrees to not lose a bit of information about the image. Secondly, the frames from the camera are so huge and FPS is so big that adequate rotation speed is provided by hardware FPGA solution only. And this solution can rotate only by 90 degrees clockwise. Of course, one can apply 90 degrees turn several times but for the sake of performance the number of turns should be minimized.</p><p>Help Vasya implement the program that by the given rotation angle of the camera can determine the minimum number of 90 degrees clockwise turns necessary to get a picture in which up direction deviation from vertical is minimum.</p><p>The next figure contains frames taken from an unrotated camera, then from rotated 90 degrees clockwise, then from rotated 90 degrees counter-clockwise. Arrows show direction to "true up".</p><center> <img class="tex-graphics" src="file://8lfxGyBA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The next figure shows 90 degrees clockwise turn by FPGA hardware.</p><center> <img class="tex-graphics" src="file://GQPqFrSr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The only line of the input contains one integer <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>) — camera angle in degrees. Positive value denotes clockwise camera rotation, negative — counter-clockwise.</p></div><div class="output-specification"><p>Output one integer — the minimum required number of 90 degrees clockwise turns.</p></div>

## Input

<p>The only line of the input contains one integer <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>) — camera angle in degrees. Positive value denotes clockwise camera rotation, negative — counter-clockwise.</p>

## Output

<p>Output one integer — the minimum required number of 90 degrees clockwise turns.</p>





```input1
60

```




```input2
-60

```




```output1
1

```




```output2
3

```



## Note

<p>When the camera is rotated <span class="tex-span">60</span> degrees counter-clockwise (the second example), an image from it is rotated <span class="tex-span">60</span> degrees clockwise. One <span class="tex-span">90</span> degrees clockwise turn of the image result in <span class="tex-span">150</span> degrees clockwise total rotation and deviation from "true up" for one turn is <span class="tex-span">150</span> degrees. Two <span class="tex-span">90</span> degrees clockwise turns of the image result in <span class="tex-span">240</span> degrees clockwise total rotation and deviation from "true up" for two turns is <span class="tex-span">120</span> degrees because <span class="tex-span">240</span> degrees clockwise equal to <span class="tex-span">120</span> degrees counter-clockwise. Three <span class="tex-span">90</span> degrees clockwise turns of the image result in <span class="tex-span">330</span> degrees clockwise total rotation and deviation from "true up" for three turns is <span class="tex-span">30</span> degrees because <span class="tex-span">330</span> degrees clockwise equal to <span class="tex-span">30</span> degrees counter-clockwise.</p><p>From <span class="tex-span">60</span>, <span class="tex-span">150</span>, <span class="tex-span">120</span> and <span class="tex-span">30</span> degrees deviations the smallest is <span class="tex-span">30</span>, and it it achieved in three <span class="tex-span">90</span> degrees clockwise turns.</p>
