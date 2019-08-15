---
layout: page
title: Тесты
permalink: /tests/
---
# Заголовок \\(\alpha\\)

## Заголовок \\(\beta\\)

### Заголовок \\(\gamma\\)

#### Заголовок \\(\delta\\)

Test2

Test $x=1$ test

Сноска[[^1]].


Сноска[^2].


Расшифровка аббревиатуры СССР

*[СССР]: Союз Советских социалистических республик


Программный код:

    def power(x, y=0):
    	return x**y


{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}


+   *Red*{: style="color: red"}
+   <span style="color: green">Green</span>
+   <span style="color: blue">Blue</span>

Эмоджи

:angry: :skull: :scream:

Таблицы

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |



| Header1     | Header2    | Header3    |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|----
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=====
| Foot1   | Foot2   | Foot3
{: rules="groups"}


Test text
{: style="color:gray; font-size: 80%; text-align: center;"}

Исходя из этого мы найдем заряд электрона. Он, будучи атомной единицей электрического заряда, равен отношению атомной единицы энергии к атомной единице напряжения, поэтому
\begin{equation}
e_0 = N^{-2/3}\,\text{Кл}=  10^{-18,3}\,\text{Кл}
\end{equation} 
На самом деле
\begin{equation}
e =  10^{-18,8}\,\text{Кл}
\end{equation}


\begin{array}{|c|c|}
  \hline 
  X  & P(X = i) \\\ 
  \hline
  1  & 1/6 \\\ 
  2  & 1/6 \\\
  \hline
\end{array}

\begin{equation}
\left{\begin{array}{rl}
	Н: & 1=\alpha+\delta \\\ 
	м: & -1=\gamma+2\delta \\\
	с: & -1=-\beta-\gamma \\\
	Кл: & 0=-\alpha-2\delta \\\
\end{array}\right.
\end{equation}

Visualize it:


[^2]:
    And here is the definition.

    > With a quote!


This is *red*{: style="color: red"}.

This is <span style="color: red">written in
red</span>.

This *is*{:.underline} some `code`{:#id}{:.class}.
A [link](test.html){:rel='something'} and some **tools**{:.tools}.


[^1]: And here is the definition.
