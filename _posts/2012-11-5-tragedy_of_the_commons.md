---
layout: post
title: Трагедия общин
---
Всегда ли строительство дорог решает проблему пробок? На самом деле нет, но об этом чуть позже. А пока давайте решим классическую экономическую задачку под названием «трагедия общин».

Суть такова. Есть деревня с \\(N\\) фермерами, которые разводят коров, и есть пастбище, на котором эти коровы пасутся. Пусть i-й фермер имеет стадо из \\(x_i\\) коров.  От каждой коровы есть прибыль с продажи ее молока \\(g\left(x_1,x_2...\right)=a-b\sum_k{x_k}\\). Эта прибыль зависит от общего числа коров, потому что ресурс пастбища ограничен, чем больше коров, тем меньше травы приходится на каждую из них, тем меньше удои молока, и тем меньше доход с коровы.

Каждый фермер стремится максимизировать свою прибыль, которая равна \\(y_i\left(x_1,x_2...\right)=x_ig\left(x_1,x_2...\right)\\), но при этом в его власти менять только размер своего стада \\(x_i\\). На языке математики это выглядит так:
\\[y_i\left(x_1,x_2...\right)\to {max}_{x_i}\\]

Чтобы найти этот максимум, необходимо, как известно, приравнять к нулю производную \\(\partial y_i/\partial x_i\\). Получается \\(\frac{\partial y_i}{\partial x_i}=g+x_i\frac{\partial g}{\partial x_i}=a-b\sum_k{x_k}-bx_i=0\\).

Отсюда, если предположить, что все N фермеров рассуждают точно так же, а значит все стада равны по численности, получается общее стадо \\(\sum_k{x_k}=\frac{aN}{b\left(N+1\right)}\\), а суммарный доход

\\[\sum_k{y_k}=\frac{aN}{b\left(N+1\right)}\left(a-b\frac{aN}{b\left(N+1\right)}\right)=\frac{a^2 N}{b{\left(N+1\right)}^2}\\]

Это называется равновесие Нэша (того самого, про которого фильм «Игры разума»), когда каждый максимизирует собственную выгоду используя только те параметры, которыми может непосредственно управлять.


Но представим себе, что фермеры могут договариваться друг с другом или вообще вести совместное хозяйство. Тогда уже нужно максимизировать суммарную прибыль \\(Y(X)=X(a-bX)\\), меняя суммарную численность стад \\(X\\).
\\[Y\to {max}_X\\]

Эту задачу с легкостью решит любой школьник, приравнивая производную к нулю \\(\frac{\partial Y}{\partial X}=a-2bX=0\ \\). Откуда \\(X=\frac{a}{2b}\\),
\\[Y=\frac{a^2}{4b}\\]

Легко видеть, что во втором случае размер стада  в \\(\frac{2N}{N+1}\\) раз меньше, а получаемый доход в \\(\frac{ {\left(N+1\right)}^2}{4N}\\) раз больше (при \\(N=20\\) это где-то в 5 раз!)

![На этой картинке зависимость прибыли от величины стада. Точка N=1 - это второй случай, когда есть одно общее стадо, а точка N=20 - это первый случай с двадцатью независимыми фермерами.]({{ site.url }}/images/nesh.jpg)

На этой картинке зависимость прибыли от величины стада. Точка \\(N=1\\) - это второй случай, когда есть одно общее стадо, а точка \\(N=20\\) - это первый случай с двадцатью независимыми фермерами.

Почему отличия столь существенны? В первом случае каждый фермер доход от своей коровы получал сам, а от издержек (уменьшение количества травы на пастбище) страдали все вместе. То есть, зарабатывая рубль, он лишал десяти рублей всех остальных. Во втором случае управление поголовьем скота переходит, скажем, старейшине, который максимизирует общую полезность, тем самым такую ситуацию исключая.

 Кстати говоря, второй случай иллюстрирует равновесие Парэто (итальянский экономист), которое означает, что любое изменение нанесет кому-то вред. Действительно, если кто-либо увеличит размер своего стада хотя бы на одну корову, то он, конечно, поимеет с этого прибыль. Но вместе с тем все остальные понесут убытки.