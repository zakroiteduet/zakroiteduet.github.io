---
layout: page
title: Гауссова оптика (решения)
permalink: /gauss-ans/
---

<hr> 
<a href="/gauss">**Условия задач**</a>
<hr> 


## Решения

**1.** Пусть $a$ --- искомое расстояние. Выходя из источника, пучок лучей имеет вид
\begin{equation}
\begin{pmatrix}
0\\\
1^\circ
\end{pmatrix}s
\end{equation}
где $s$ принимает различные значения для различных лучей. Пройдя расстояние $a$, пучок превратится в 
\begin{equation}
\begin{pmatrix}
a^\circ\\\ 
1^\circ
\end{pmatrix}s
=
\begin{pmatrix}
1 & a\\\ 
0 & 1
\end{pmatrix}
\begin{pmatrix}
0\\\ 
1^\circ
\end{pmatrix}s
\end{equation}
По условиям задачи
\begin{equation}
\begin{pmatrix}
a^\circ\\\ 
1^\circ
\end{pmatrix}s
=
\begin{pmatrix}
1\,\text{мм}\\\ 
1^\circ
\end{pmatrix}t
\end{equation}
Следовательно $s=t$, а $a^\circ=1\,\text{мм}$. Вспоминаем, что $180^\circ=\pi$, и тогда $a=57\,\text{мм}$.

  
**2.** Чтобы найти матрицу линзы, нужно, как и в случае бокала, перемножить три матрицы. Но, так как линза тонкая, средней матрицей можно пренебречь (она примерно единична). Тогда
\begin{equation}
\begin{pmatrix}
1 & 0 \\\ 
-(\tfrac{1}{R_1}+\tfrac{1}{R_2})(n-1)& 1
\end{pmatrix} 
=
\begin{pmatrix}
1 & 0 \\\ 
\tfrac{1-n}{R_2}& 1
\end{pmatrix} \cdot
\begin{pmatrix}
1 & 0 \\\ 
\tfrac{n-1}{-R_1}& 1
\end{pmatrix}
\end{equation}
Значит
\begin{equation}
\dfrac{1}{f} = \left(\dfrac{1}{R_1}+\dfrac{1}{R_2}\right)(n-1)
\end{equation}
Формула доказана.



**3.** Выходя из источника, пучок лучей имеет вид
\begin{equation}
\begin{pmatrix}
0\\\ 
1
\end{pmatrix}t
\end{equation}
Ему нужно пройти расстояние $a$, преломиться в линзе и пройти еще расстояние $b$
\begin{equation}
\begin{pmatrix}
a+b-\tfrac{ab}{f}\\\ 
1-\tfrac{a}{f}
\end{pmatrix}t
=
\begin{pmatrix}
1 & b\\\ 
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0\\\ 
-\tfrac{1}{f} & 1
\end{pmatrix}
\begin{pmatrix}
1 & a\\\ 
0 & 1
\end{pmatrix}
\begin{pmatrix}
0\\\ 
1
\end{pmatrix}t
\end{equation}
Для того, чтобы лучи сошлись на оптической оси, необходимо занулить первую компоненту вектора, то есть потребовать $a+b=\dfrac{ab}{f}$, или что то же самое
\begin{equation}
\dfrac{1}{a}+\dfrac{1}{b}=\dfrac{1}{f}
\end{equation}
Это не только необходимо, но и достаточно, так как тогда вектор приобретает вид
\begin{equation}
\begin{pmatrix}
0\\\ 
1
\end{pmatrix}(1-\tfrac{a}{f})t
\end{equation}
множитель $1-\tfrac{a}{f}$ говорит о том, что лучи сходятся под другим углом по сравнению с тем, как расходятся из источника.

К сожалению, в рамках гауссовой оптики мы не можем говорить о случае, когда источник не находится на оптической оси, а значит и об увеличении с помощью линзы. Для этого надо отказаться от цилиндрической симметрии и перейти у линейной оптике. Однако после этого непростого перехода мы придем формулам аналогичным формулам гауссовой оптики. Но это другая история. 



**4.** Все, что нужно для решения этой задачи, --- это возвести найденную нами в видео матрицу в шестую степень. Вот она, если подставить в нее $n=4/3$:
\begin{equation}
\begin{pmatrix}
\tfrac{1}{2} & \tfrac{3R}{2}\\\ 
-\tfrac{1}{2R} & \tfrac{1}{2}
\end{pmatrix}
\end{equation}
вот она в третьей степени
\begin{equation}
\begin{pmatrix}
-1 & 0\\\ 
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
\tfrac{1}{2} & \tfrac{3R}{2}\\\ 
-\tfrac{1}{2R} & \tfrac{1}{2}
\end{pmatrix}
\begin{pmatrix}
\tfrac{1}{2} & \tfrac{3R}{2}\\\ 
-\tfrac{1}{2R} & \tfrac{1}{2}
\end{pmatrix}
\begin{pmatrix}
\tfrac{1}{2} & \tfrac{3R}{2}\\\ 
-\tfrac{1}{2R} & \tfrac{1}{2}
\end{pmatrix}
\end{equation}
а вот в шестой
\begin{equation}
\begin{pmatrix}
1 & 0\\\ 
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
-1 & 0\\\ 
0 & -1
\end{pmatrix}
\begin{pmatrix}
-1 & 0\\\ 
0 & -1
\end{pmatrix}
\end{equation}
Единичный вид матрицы говорит, что шесть бокалов ничего не делают со светом. Не в смысле, что их можно просто убрать, так как если их просто убрать, то получилась бы матрица
\begin{equation}
\begin{pmatrix}
1 & 12R\\\ 
0 & 1
\end{pmatrix}
\end{equation}
а в смысле, что свет как бы телепортируется, как будто даже никакого пространства, занимаемого бокалами, нет. Заметим, что внутри системы свет даже <<выворачивается наизнанку>>, но на выходе оказывается таким же как на входе (если не считать аберраций, которые накапливаются в такой системе, и оставляют без изменение только самые близкие к оптической оси лучи).
<center><img src="/images/gauss-ans-1.png" width="600"/></center>

 

**5.** Параллельный пучок описывается вектор-столбцами
\begin{equation}
\begin{pmatrix}
1 \\\ 
0
\end{pmatrix}t
\end{equation}
В первом случае имеем произведение 
\begin{equation}
\begin{pmatrix}
1 \\\ 
-\tfrac{n-1}{R} 
\end{pmatrix}t
=
\begin{pmatrix}
1 & 0\\\ 
-\tfrac{n-1}{R} & 1
\end{pmatrix}
\begin{pmatrix}
1 & \tfrac{R}{n}\\\ 
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\\ 
0
\end{pmatrix}t
\end{equation}
Значит пучок сфокусируется, пройдя расстояние $\tfrac{R}{n-1}$ после выхода из полушара. 
<center><img src="/images/gauss-ans-2.png" width="600"/></center>

Во втором случае порядок множителей иной
\begin{equation}
\begin{pmatrix}
\tfrac{1}{n} \\\ 
-\tfrac{n-1}{R} 
\end{pmatrix}t
=
\begin{pmatrix}
1 & \tfrac{R}{n}\\\ 
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0\\\ 
-\tfrac{n-1}{R} & 1
\end{pmatrix}
\begin{pmatrix}
1 \\\ 
0
\end{pmatrix}t
\end{equation}
Значит пучок сфокусируется на расстоянии $\tfrac{nR}{n-1}$ за полушаром.
<center><img src="/images/gauss-ans-3.png" width="600"/></center>



