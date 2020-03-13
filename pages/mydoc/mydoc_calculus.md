---
title: calculus
sidebar: mydoc_sidebar
keywords: calculus
permalink: mydoc_calculus.html
summary: "calculus"
folder: mydoc
use_math: true

---

## Limit of sequence

### 1. Convergent and Divergent Sequences

* Convergent <br>
수열 {$a_n$}에서 n이 한없이 커질 때, $a_n$이 일정한 값 $\alpha$에 한없이 가까워지면 수열 {$a_n$}은 $\alpha$에 수렴한다고 한다. <br>이때, $\alpha$를 수열 {$a_n$}의 극한값 또는 극한이라고 하고, 이것을 기호로
<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;${n \to \infty}$ 일 때 $\lim_{n \to \infty}a_n = \alpha$
<br><br>
와 같이 나타낸다. 여기서 $a_n$ = $\alpha$가 아니라 n이 무한대로 갈 때 $\alpha$로 가까워 지는것을 말한다.

* Divergent <br>
발산의 경우 {$a_n$}에서 n이 한없이 커질 때, $a_n$의 값이 한없이 커지면 수열 {$a_n$}은 양의 무한대로 발산한다고 하며 다음과 같이 나타낸다.
<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;$\lim_{n \to \infty}a_n = \infty$
<br><br>
{$a_n$}에서 n이 한없이 커질 때, $a_n$의 값이 음수이면서 그 절댓값이 한없이 커지면 {$a_n$}은 음의 무한대로 발산한다고 하며 다음과 같이 나타낸다.
<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;$\lim_{n \to \infty}a_n = -\infty$
<br><br>
수열 {$a_n$}이 수렴하지도 않고, 발산하지도 않으면 진동한다고 한다.

### 2. Limit Laws of Convergent Sequences

수열 {$a_n$}와 {$b_n$}이 모두 수렴하고 $\lim_{n \to \infty}a_n = \alpha$, $\lim_{n \to \infty}b_n = \beta$ 일 때 <br>
* $\lim_{n \to \infty}ka_n = k\lim_{n \to \infty}a_n = k\alpha$ ($k$는 상수)
* $\lim_{n \to \infty}(a_n \pm b_n) = \lim_{n \to \infty}a_n \pm \lim_{n \to \infty}b_n = \alpha \pm \beta$ (복부호동순)
* $\lim_{n \to \infty}(a_n b_n) = \lim_{n \to \infty}a_n \times \lim_{n \to \infty}b_n = \alpha\beta$
* $\lim_{n \to \infty}\frac{a_n}{b_n} = \frac{\lim_{n \to \infty}a_n}{\lim_{n \to \infty}b_n} = \frac{\alpha}{\beta} (b_n \neq 0, \beta \neq 0)$
* $\lim_{n \to \infty}(a_n)^k = (lim_{n \to \infty}a_n)^k = (\alpha)^k$ ($k$는 자연수)


### 2. Estimating the value of limits

1) $\frac{\infty}{\infty}$꼴: 분모의 최고차항으로 분모, 분자를 나눈다. <br>
    * (분자의 차수) > (분모의 차수) => $\lim_{n \to \infty}a_n = \infty 또는 -\infty$
    * (분자의 차수) = (분모의 차수) => $\lim_{n \to \infty}a_n = 최고차항의 계수의 비$
    * (분자의 차수) < (분모의 차수) => $\lim_{n \to \infty}a_n = 0$

2) $\infty - \infty$꼴
    1. 다항식의 극한은 최고차항으로 묶는다.
    2. 무리식의 극한은 분모 또는 분자를 유리화한다.