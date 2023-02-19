## Description

<div><p>Lena is the most economical girl in Moscow. So, when her dad asks her to buy some food for a trip to the country, she goes to the best store &nbsp;— "PriceFixed". Here are some rules of that store:</p><ul> <li> The store has an infinite number of items of every product. </li><li> All products have the same price: $2$ rubles per item. </li><li> For every product $i$ there is a discount for experienced buyers: if you buy $b_i$ items of products (<span class="tex-font-style-bf">of any type</span>, not necessarily type $i$), then for all future purchases of the $i$-th product there is a $50\%$ discount (so you can buy an item of the $i$-th product for $1$ ruble!). </li></ul><p>Lena needs to buy $n$ products: she must purchase at least $a_i$ items of the $i$-th product. Help Lena to calculate the minimum amount of money she needs to spend if she optimally chooses the order of purchasing. Note that if she wants, she can buy more items of some product than needed.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of products.</p><p>Each of next $n$ lines contains a product description. Each description consists of two integers $a_i$ and $b_i$ ($1 \leq a_i \leq 10^{14}$, $1 \leq b_i \leq 10^{14}$)&nbsp;— the required number of the $i$-th product and how many products you need to buy to get the discount on the $i$-th product. </p><p>The sum of all $a_i$ does not exceed $10^{14}$.</p></div><div class="output-specification"><p>Output the minimum sum that Lena needs to make all purchases. </p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of products.</p><p>Each of next $n$ lines contains a product description. Each description consists of two integers $a_i$ and $b_i$ ($1 \leq a_i \leq 10^{14}$, $1 \leq b_i \leq 10^{14}$)&nbsp;— the required number of the $i$-th product and how many products you need to buy to get the discount on the $i$-th product. </p><p>The sum of all $a_i$ does not exceed $10^{14}$.</p>

## Output

<p>Output the minimum sum that Lena needs to make all purchases. </p>





```input1
3
3 4
1 3
1 5
```




```input2
5
2 7
2 8
1 2
2 4
1 8
```




```output1
8
```




```output2
12
```



## Note

<p>In the first example, Lena can purchase the products in the following way:</p><ol> <li> one item of product $3$ for $2$ rubles, </li><li> one item of product $1$ for $2$ rubles, </li><li> one item of product $1$ for $2$ rubles, </li><li> one item of product $2$ for $1$ ruble (she can use the discount because $3$ items are already purchased), </li><li> one item of product $1$ for $1$ ruble (she can use the discount because $4$ items are already purchased). </li></ol><p>In total, she spends $8$ rubles. It can be proved that it is impossible to spend less.</p><p>In the second example Lena can purchase the products in the following way:</p><ol> <li> one item of product $1$ for $2$ rubles, </li><li> two items of product $2$ for $2$ rubles for each, </li><li> one item of product $5$ for $2$ rubles, </li><li> one item of product $3$ for $1$ ruble, </li><li> two items of product $4$ for $1$ ruble for each, </li><li> one item of product $1$ for $1$ ruble. </li></ol><p>In total, she spends $12$ rubles.</p>
