---
title: probability and statistics
sidebar: mydoc_sidebar
keywords: probability, statistics, permutation, circular
permalink: mydoc_probability_and_statistics.html
summary: "probability and statistics"
folder: mydoc
use_math: true

---

## number of cases

### 1. circular permutation

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