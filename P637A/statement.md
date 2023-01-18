## Description

<div><p>After celebrating the midcourse the students of one of the faculties of the Berland State University decided to conduct a vote for the best photo. They published the photos in the social network and agreed on the rules to choose a winner: the photo which gets most likes wins. If multiple photoes get most likes, the winner is the photo that gets this number first.</p><p>Help guys determine the winner photo by the records of likes.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the total likes to the published photoes. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the identifier of the photo which got the <span class="tex-span"><i>i</i></span>-th like.</p></div><div class="output-specification"><p>Print the identifier of the photo which won the elections.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the total likes to the published photoes. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the identifier of the photo which got the <span class="tex-span"><i>i</i></span>-th like.</p>

## Output

<p>Print the identifier of the photo which won the elections.</p>





```input1
5
1 3 2 2 1

```




```input2
9
100 200 300 200 100 300 300 100 200

```




```output1
2

```




```output2
300

```



## Note

<p>In the first test sample the photo with id <span class="tex-font-style-tt">1</span> got two likes (first and fifth), photo with id <span class="tex-font-style-tt">2</span> got two likes (third and fourth), and photo with id <span class="tex-font-style-tt">3</span> got one like (second). </p><p>Thus, the winner is the photo with identifier <span class="tex-font-style-tt">2</span>, as it got:</p><ul> <li> more likes than the photo with id <span class="tex-font-style-tt">3</span>; </li><li> as many likes as the photo with id <span class="tex-font-style-tt">1</span>, but the photo with the identifier <span class="tex-font-style-tt">2</span> got its second like earlier. </li></ul>
