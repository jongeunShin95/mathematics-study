---
title: probability and statistics
sidebar: mydoc_sidebar
keywords: probability, Number of cases, Circular Permutation, Permutations with Repetition, Multiset Permutation
permalink: mydoc_probability_and_statistics.html
summary: "probability and statistics"
folder: mydoc
use_math: true

---

## Number of cases

### 1. Circular Permutation

n개의 서로 다른 것을 원형으로 배열하는 방법의 수 <br>

* ${n! \over n} = (n-1)!$

<br>

1, 2, 3을 일렬로 배열하는 경우의 수

    (1,2,3) (1,3,2) (2,1,3) (2,3,1) (3,1,2) (3,2,1)

위의 6가지를 원형으로 배열한 그림 <br>

{% include inline_image.html file="probability_and_statistics/number_of_cases/circular_permutation/circle_permutation.png" alt="circle_image" %}

위 그림에서 형관펜으로 칠한 수로 시작하는 경우 상대적인 위치가 같다. <br>
즉, (1->2->3) (1->3->2)의 두가지 순서로 나타난다. <br><br>

서로 다른 n개를 원형으로 배열하게 되면 상대적인 위치가 같은 경우가 n개 씩 있으므로, <br>
일렬로 나열하는 수에서 n을 나누어주면 된다.<br>

따라서 서로 다른 n개를 원형으로 배열하는 경우의 수는 *${n^2 \over n} = (n-1)!$* 가 된다.
<br><br>

원형이 아닌 다각형인 경우(대칭인 경우)의 순열의 수
* 정사각형의 식탁에 n명을 앉히는 방법의 수 => $(n-1)! \times {n \over 4}$
* 정삼각형의 식탁에 n명을 앉히는 방법의 수 => $(n-1)! \times {n \over 3}$
* 직사각형의 식탁에 n명을 앉히는 방법의 수 => $(n-1)! \times {n \over 2}$
<br>

{% include inline_image.html file="probability_and_statistics/number_of_cases/circular_permutation/another_permutation.png" alt="circle_image" %}


### 2. Permutations with Repetition

서로 다른 n개에서 중복을 허락하여 r개를 택하는 중복순열의 수는<br>

* $\_{n}\mathrm{\Pi}_{r} = n^r$

### 3. Multiset Permutation

n개 중 p개, q개, r개, $\cdots$, s개가 각각 같은 것일 때, 이들을 일렬로 나열하는 순열의 수는

* $\frac{n!}{p! \times q! \times r! \times \cdots \times s!}$ (단, $n = p + q + r + \cdots + s$)

<br>
1) example

{% include inline_image.html file="probability_and_statistics/number_of_cases/multiset_permutation/problem.png" alt="problem" %}

최단 경로로 가기 위해서는 왼쪽이나 아랫쪽으로 이동하면 안되며 그림에서 최단 경로 중 가장 쉬운 방법 한가지로는 오른쪽으로 4번, 위쪽으로 3번을 가는 것이다.
따라서 이 방법이 최단 경로가 되고 이 방법으로 A지점에서 B지점으로 가기 위한 경우의 수를 구해야되는데 오른쪽으로 가는 방법을 a, 위쪽으로 가는 방법을 b라고 했을 때
a,a,a,a,b,b,b를 나열하는 경우의 수로 문제를 풀 수 있다. 따라서 경우의 수는 $\frac{7!}{4! \times 3! = 35}$(가지) 가 된다.

### 4. Combination with Repetition

서로 다은 $n$개에서 $r$개를 택하는 중복조합의 수는
* $_{n}H_{r} = _{n+r-1}C_{n-1} = _{n+r-1}C_{r}$