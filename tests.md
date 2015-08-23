---
layout: page
title: Тесты
permalink: /tests/
---
# Заголовок \\(\alpha\\)

## Заголовок \\(\beta\\)

### Заголовок \\(\gamma\\)

#### Заголовок \\(\delta\\)


Сноска[[^1]].


Сноска[^2].


Программный код:

    def power(x, y=0):
    	return x**y

~~~ ruby
def what?
  42
end
~~~

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
+   Green{: style="color: green"}
+   Blue{: style="color: blue"}

Эмоджи

:angry: :skull: :scream:

Табюлицы

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|----
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=====
| Foot1   | Foot2   | Foot3
{: rules="groups"}


|---
| Default aligned | Left aligned | Center aligned | Right aligned
|-|:-|:-:|-:
| First body part | Second cell | Third cell | fourth cell
| Second line |foo | **strong** | baz
| Third line |quux | baz | bar
|---
| Second body
| 2 line
|===
| Footer row



Исходя из этого мы найдем заряд электрона. Он, будучи атомной единицей электрического заряда, равен отношению атомной единицы энергии к атомной единице напряжения, поэтому
\begin{equation}
e_0 = N^{-2/3}\,\text{Кл}=  10^{-18,3}\,\text{Кл}
\end{equation} 
На самом деле
\begin{equation}
e =  10^{-18,8}\,\text{Кл}
\end{equation}

\newcommand\T{\Rule{0pt}{1em}{.3em}}
\begin{array}{|c|c|}
\hline X & P(X = i) \T \\\hline
  1 \T & 1/6 \\\hline
  2 \T & 1/6 \\\hline
  3 \T & 1/6 \\\hline
  4 \T & 1/6 \\\hline
  5 \T & 1/6 \\\hline
  6 \T & 1/6 \\\hline
\end{array}

Visualize it:

<iframe src="/mbostock/raw/4061502/0a200ddf998aa75dfdb1ff32e16b680a15e5cb01/" marginwidth="0" marginheight="0" scrolling="no"></iframe>


Расшифровка аббревиатуры СССР

*[СССР]: Союз Советских социалистических республик


[^2]:
    And here is the definition.

    > With a quote!


This is *red*{: style="color: red"}.

This is <span style="color: red">written in
red</span>.

This *is*{:.underline} some `code`{:#id}{:.class}.
A [link](test.html){:rel='something'} and some **tools**{:.tools}.


[^1]: And here is the definition.