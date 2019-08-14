---
layout: page
title: Полное внутреннее отражение (решения)
permalink: /scattering-ans/
---

<hr> 
<a href="/reflection">**Условия задач**</a>
<hr> 


## Решения

**1.** Каков цвет неба в RGB?

Ответим на этот вопрос очень грубо. Возьмем три длины волны: $\lambda_R=0{,}65\,\text{мкм}$ (красный), $\lambda_G=0{,}55\,\text{мкм}$ (зеленый), $\lambda_B=0{,}45\,\text{мкм}$ (синий). Возведем их в минус четвертую степень: $\lambda_R^{-4}=5{,}6\,\text{мкм}^{-4}$,  $\lambda_G^{-4}=10{,}9\,\text{мкм}^{-4}$, $\lambda_B^{-4}=24{,}4\,\text{мкм}^{-4}$. То есть, отношение интенсивностей рассеяния этих длин волн согласно формуле Релея равно примерно $1:2:5$. Поэтому цвет $(50,100,250)=#3264FA$ должен примерно соответсвовать цвету неба. На картинке он слева.

Добавим, что, если бы наша атмосфера была бы более плотной, то цвет получился бы менее насыщенным, а в очень плотной атмосфере цвет неба получился бы и вовсе серым (как в пасмурную погоду), так как весь солнечный свет рассеивался бы полностью. На картинке справа цвет $(80,120,200)=#5078C8$, это цвет примерно того же тона и светлоты, но меньшей насыщенности.

<center><img src="/images/scattering-ans-1.png" width="400"/></center>




Однако, мы совсем не учли многократное рассеяние.
На самом деле, необходимо добавить, что наша атмосфера не очень толстая и не очень плотная, и поэтому рассеивает мало света, не более нескольких процентов. Поэтому наши расчеты верны. Для более толстых и плотных атмосфер необходимо учитывать многократное рассеивание, которое делает цвет неба менее насыщенным, то есть более серым как в пасмурную погоду.

**2.** Расстояние от точки наблюдения до полюсов диполя равно согласно теореме Пифагора $\sqrt{r^2+\ell^2/4}$. Поэтому электрические поля, создаваемые в этой точке равны $E_{\pm}=kq/(r^2+\ell^2/4)$. В горизонтальном направлении они компенсируют друг друга, а в вертикальном нет. Чтобы найти вертикальную компоненту пользуемся подобием закрашенных треугольников

<center><img src="/images/scattering-ans-2.png" width="500"/></center>

\begin{equation} \frac{E}{E_+} = \frac{\ell}{\sqrt{r^2+\ell^2/4}} \end{equation}
\begin{equation} E=k\frac{q\ell}{(r^2+\ell^2/4)^{3/2}} \end{equation}
На больших расстояниях $r\gg\ell$, поэтому $\ell$ в знаменателе можно пренебречь. Можно сказать, диполи любой формы и размера издалека выглядят примерно одиаково. Мы получаем формулу
\begin{equation} E=k\frac{d}{r^3} \end{equation}
