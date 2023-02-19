## Description

<div><p>Alice is visiting New York City. To make the trip fun, Alice will take photos of the city skyline and give the set of photos as a present to Bob. However, she wants to find the set of photos with maximum beauty and she needs your help. </p><p>There are $n$ buildings in the city, the $i$-th of them has positive height $h_i$. All $n$ building heights in the city are different. In addition, each building has a beauty value $b_i$. Note that beauty can be positive or negative, as there are ugly buildings in the city too. </p><p>A set of photos consists of one or more photos of the buildings in the skyline. Each photo includes one or more buildings in the skyline that form a contiguous segment of indices. Each building needs to be in <span class="tex-font-style-bf">exactly one</span> photo. This means that if a building does not appear in any photo, or if a building appears in more than one photo, the set of pictures is not valid. </p><p>The beauty of a photo is equivalent to the beauty $b_i$ of the shortest building in it. The total beauty of a set of photos is the sum of the beauty of all photos in it. Help Alice to find the maximum beauty a valid set of photos can have. </p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 3 \cdot 10^5$), the number of buildings on the skyline. </p><p>The second line contains $n$ distinct integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le n$). The $i$-th number represents the height of building $i$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($-10^9 \le b_i \le 10^9$). The $i$-th number represents the beauty of building $i$.</p></div><div class="output-specification"><p>Print one number representing the maximum beauty Alice can achieve for a valid set of photos of the skyline. </p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 3 \cdot 10^5$), the number of buildings on the skyline. </p><p>The second line contains $n$ distinct integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le n$). The $i$-th number represents the height of building $i$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($-10^9 \le b_i \le 10^9$). The $i$-th number represents the beauty of building $i$.</p>

## Output

<p>Print one number representing the maximum beauty Alice can achieve for a valid set of photos of the skyline. </p>





```input1
5
1 2 3 5 4
1 5 3 2 4
```




```input2
5
1 4 3 2 5
-3 4 -10 2 7
```




```input3
2
2 1
-2 -3
```




```input4
10
4 7 3 2 5 1 9 10 6 8
-4 40 -46 -8 -16 4 -10 41 12 3
```




```output1
15
```




```output2
10
```




```output3
-3
```




```output4
96
```



## Note

<p>In the first example, Alice can achieve maximum beauty by taking five photos, each one containing one building. </p><p>In the second example, Alice can achieve a maximum beauty of $10$ by taking four pictures: three just containing one building, on buildings $1$, $2$ and $5$, each photo with beauty $-3$, $4$ and $7$ respectively, and another photo containing building $3$ and $4$, with beauty $2$. </p><p>In the third example, Alice will just take one picture of the whole city.</p><p>In the fourth example, Alice can take the following pictures to achieve maximum beauty: photos with just one building on buildings $1$, $2$, $8$, $9$, and $10$, and a single photo of buildings $3$, $4$, $5$, $6$, and $7$. </p>
