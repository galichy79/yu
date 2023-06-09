---
title: Елементи
feature_text: |
  Демонстрація Markdown та HTML елементів
feature_image: "https://www.google.com/url?sa=i&url=https%3A%2F%2Fua.depositphotos.com%2Fstock-photos%2F%25D0%25B3%25D0%25B0%25D1%2580%25D0%25BD%25D0%25B0-%25D0%25B4%25D1%2596%25D0%25B2%25D1%2587%25D0%25B8%25D0%25BD%25D0%25B0.html&psig=AOvVaw05HgNf0zyYb03S8Q3d9PCq&ust=1682164648320000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCLjjyOT1uv4CFQAAAAAdAAAAABAJ"
excerpt: "A demo of Markdown and HTML includes"
aside: true
---

# Heading 1

###### Heading 6

<small>Маленький текст</small>

[Посилання](https://david.darn.es "A link")

Так це виглядає * що тут? * ось так.

Посилання у тексті [Посилання](https://david.darn.es "A link") reprehenderit in voluptate velit esse cillum **Жирний текс** dolore eu fugiat nulla pariatur. Excepteur span element sint occaecat cupidatat non proident, sunt _італік шрифт_ in culpa qui officia deserunt mollit anim id `код` ось так.

* An item
* An item
* An item
* An item
* An item

1. Item one
2. Item two
3. Item three
4. Item four
5. Item five

> Проста цитата

 HTML...

``` html
<blockquote cite="http://www.imdb.com/title/tt0284978/quotes/qt1375101">
  <p>You planning a vacation, Mr. Sullivan?</p>
  <footer>
    <a href="http://www.imdb.com/title/tt0284978/quotes/qt1375101">Sunways Security Guard</a>
  </footer>
</blockquote>
```

...CSS...

``` css
blockquote {
  text-align: center;
  font-weight: bold;
}
blockquote footer {
  font-size: .8rem;
}
```

...і JavaScript

``` js
const blockquote = document.querySelector("blockquote")
const bolden = (keyString, string) =>
  string.replace(new RegExp(keyString, 'g'), '<strong>'+keyString+'</strong>')

blockquote.innerHTML = bolden("Mr. Sullivan", blockquote.innerHTML)
```

`Single line of code`

## HTML Includes

### Contact form

{% include site-form.html %}

``` html
{% raw %}{% include site-form.html %}{% endraw %}
```

### Demo map embed

{% include map.html id="1UT-2Z-Vg_MG_TrS5X2p8SthsJhc" title="Coffee shop map" %}

``` html
{% raw %}{% include map.html id="XXXXXX" title="Coffee shop map" %}{% endraw %}

```

<iframe src="https://www.google.com/maps/d/embed?mid=1ykll9YZCI1WkFf_d7y7V-3XJF0-lUcg&ehbc=2E312F" width="640" height="480"></iframe>

### Button include

{% include button.html text="Конпка" link="https://adagio-hostel-online" %}

{% include button.html text="A button with icon" link="https://twitter.com/#" icon="twitter" %}

``` html
{% raw %}{% include button.html text="A button" link="https://david.darn.es" %}
{% include button.html text="A button with icon" link="https://twitter.com/daviddarnes" icon="twitter" %}{% endraw %}
```

### Icon include

{% include icon.html id="twitter" title="twitter" %} [{% include icon.html id="linkedin" title="twitter" %}](https://www.linkedin.com/in/daviddarnes)

``` html
{% raw %}{% include icon.html id="twitter" title="twitter" %}
[{% include icon.html id="linkedin" title="twitter" %}](https://www.linkedin.com/in/daviddarnes){% endraw %}
```

### Video include

{% include video.html id="zrkcGL5H3MU" title="Siteleaf tutorial video" %}

``` html
{% raw %}{% include video.html id="zrkcGL5H3MU" title="Siteleaf tutorial video" %}{% endraw %}
```


### Image includes

{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Image with caption" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Right aligned image" position="right" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Left aligned image" position="left" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/1600/800?image=894" alt="Image with just alt text" %}

``` html
{% raw %}{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Image with caption" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Right aligned image" position="right" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/600/800?image=894" caption="Left aligned image" position="left" width="300" height="800" %}

{% include figure.html image="https://picsum.photos/1600/800?image=894" alt="Image with just alt text" %}{% endraw %}
```
