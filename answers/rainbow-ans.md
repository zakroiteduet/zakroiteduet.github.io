---
layout: page
title: Радуга (решения)
permalink: /rainbow-ans/
---

<hr> 
<a href="/rainbow">**Условия задач**</a>
<hr> 


## Теория

Угол $\theta$, на который поворачивается луч, рассеиваясь на шаре, складывается из нескольких слагаемых. На входе и выходе из шара свет преломляется, оба раза на угол $\alpha-\beta$. И при каждом отражении внутри шара свет поворачивается на угол $180^\circ-2\beta$. Итого 
\begin{equation}
\theta = 2(\alpha-\beta) + k(180^\circ-2\beta)
\end{equation}
то есть
\begin{equation}
\theta = k\,180^\circ + 2\alpha-2(k+1)\beta
\end{equation}

где $k$ --- это количество отражений. В видео мы рассматривали третью компоненту рассеяния, у которой $k=1$. Во второй компоненте не происходит отражения, только преломление, поэтому $k=0$. Немного удивительно, но для первой компоненты эта формула тоже верна, если положить $k=-1$, получится $\theta = 2\alpha-180^\circ$. 

Учитывая связь углов $\alpha$ и $\beta$ --- закон Снелла
\begin{equation}
\sin\alpha = n\sin\beta
\end{equation}

мы получаем функцию $\theta(\alpha)$
\begin{equation}
\theta = k\,180^\circ + 2\alpha-2(k+1)\mathrm{arcsin}\dfrac{\sin\alpha}{n}
\end{equation}

 Чтобы найти, под каким углом концентрируются лучи, приравниваем производную этой функции к нулю
\begin{equation}
\theta'(\alpha) = 2-2(k+1)\dfrac{\cos\alpha}{\sqrt{n^2-\sin^2\alpha}}=0
\end{equation} 

и после некоторых преобразований (умножения на знаменатель, возведение в квадрат, использования основного тригонометрического тождества) получаем одну единственную $\alpha^*$:
\begin{equation}
\alpha^* = \mathrm{arctg}\sqrt{\dfrac{(k+1)^2-n^2}{n^2-1}}
\end{equation}

Такую $\alpha^*$ называют стационарной точкой функции $\theta(\alpha)$, она может быть минимумом или максимумом, а может не быть ни тем, ни другим. Но важно не это, а то, что производная в этой точке равна нулю, а значит функция <<задерживается>> на своем значении в этой точке $\theta^*=\theta(\alpha^*)$ дольше, чем на значениях в других точках. Это и есть концентрация света.


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
