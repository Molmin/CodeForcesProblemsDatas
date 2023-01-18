## Description

<div><p>It’s riot time on football stadium Ramacana! Raging fans have entered the field and the police find themselves in a difficult situation. The field can be represented as a square in the coordinate system defined by two diagonal vertices in (0,0) and (<span class="tex-span">10<sup class="upper-index">5</sup></span>, <span class="tex-span">10<sup class="upper-index">5</sup></span>). The sides of that square are also considered to be <span class="tex-font-style-bf">inside</span> the field, everything else is <span class="tex-font-style-bf">outside</span>.</p><p>In the beginning, there are <span class="tex-span"><i>N</i></span> fans on the field. For each fan we are given his speed, an integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> as well as his integer coordinates (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>). A fan with those coordinates might move and after one second he might be at any point (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>p</i></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> + <i>q</i></span>) where <span class="tex-span">0 ≤ |<i>p</i>| + |<i>q</i>| ≤ <i>v</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> are both integers.</p><p>Points that go <span class="tex-font-style-bf">outside</span> of the square that represents the field are excluded and all others have equal probability of being the location of that specific fan after one second.</p><p>Andrej, a young and promising police officer, has sent a flying drone to take a photo of the riot from above. The drone’s camera works like this:</p><ol> <li> It selects three points with <span class="tex-font-style-bf">integer coordinates</span> such that there is a chance of a fan appearing there after one second. They must not be collinear or the camera won’t work. It is guaranteed that not all of the initial positions of fans will be on the same line. </li><li> Camera focuses those points and creates a circle that passes through those three points. A photo is taken after one second (one second after the initial state). </li><li> Everything that is on the circle or inside it at the moment of taking the photo (one second after focusing the points) will be on the photo. </li></ol><p>Your goal is to select those three points so that the expected number of fans seen on the photo is maximized. If there are more such selections, select those three points that give the circle with <span class="tex-font-style-bf">largest radius</span> among them. If there are still more suitable selections, <span class="tex-font-style-bf">any one</span> of them will be accepted. If your answer follows conditions above and radius of circle you return is smaller then the optimal one by 0.01, your output will be considered as correct.</p><p>No test will have optimal radius bigger than <span class="tex-span">10<sup class="upper-index">10</sup></span>.</p></div><div class="input-specification"><p>The first line contains the number of fans on the field, <span class="tex-span"><i>N</i></span>. The next <span class="tex-span"><i>N</i></span> lines contain three integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ,<span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. They are the <span class="tex-span"><i>x</i></span>-coordinate, <span class="tex-span"><i>y</i></span>-coordinate and speed of fan <span class="tex-span"><i>i</i></span> at the beginning of the one second interval considered in the task.</p><ul> <li> <span class="tex-span">3 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span> </li><li> All numbers are integers </li></ul></div><div class="output-specification"><p>You need to output the three points that camera needs to select. Print them in three lines, with every line containing the <span class="tex-span"><i>x</i></span>-coordinate, then <span class="tex-span"><i>y</i></span>-coordinate, separated by a single space. The order of points does not matter.</p></div>

## Input

<p>The first line contains the number of fans on the field, <span class="tex-span"><i>N</i></span>. The next <span class="tex-span"><i>N</i></span> lines contain three integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ,<span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. They are the <span class="tex-span"><i>x</i></span>-coordinate, <span class="tex-span"><i>y</i></span>-coordinate and speed of fan <span class="tex-span"><i>i</i></span> at the beginning of the one second interval considered in the task.</p><ul> <li> <span class="tex-span">3 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span> </li><li> All numbers are integers </li></ul>

## Output

<p>You need to output the three points that camera needs to select. Print them in three lines, with every line containing the <span class="tex-span"><i>x</i></span>-coordinate, then <span class="tex-span"><i>y</i></span>-coordinate, separated by a single space. The order of points does not matter.</p>





```input1
3
1 1 1
1 1 1
1 2 1

```




```output1
2 2
2 1
1 0

```


