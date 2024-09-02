

# Study HTML

What is an HTML Element?
An HTML element is defined by a start tag, some content, and an end tag:

<tagname> Content goes here... </tagname>
The HTML element is everything from the start tag to the end tag:

<h1>My First Heading</h1>
<p>My first paragraph.</p>

---

## elements (tag)
 - \<h1>
 - \<p></p>
 - \<br/>
 - [\<pre>](#pre)
 - [\<hr>](#hr)
 - [\<a>](#a)

    - [**Элементы форматирования HTML**](#example)

        - \<**strong**> <strong>- Важный текст
        - \<**b**> <b>- Жирный текст
        - \<**i**> <i>- Курсивный текст
        - \<**em**> <em>- Выделенный текст
        - \<**mark**> <mark>- Выделенный текст
        - \<**small**> <small>- Меньший текст
        - \<**del**> <del>- Удаленный текст
        - \<**ins**> <ins>- Вставленный текст
        - \<**sub**> <sub>- Подстрочный текст
        - \<**sup**> <sup>- Надстрочный текст

    - **элементы цитат и цитирования**

        - \<**abbr**> - Defines an abbreviation or acronym
        - \<**address**> - Defines contact information for the author/owner of a document
        - \<**bdo**> - Defines the text direction
        - \<**blockquote**> -  Defines a section that is quoted from another source
        - \<**cite**> - Defines the title of a work
        - \<**q**> - Defines a short inline quotation


---

## Atribute
 - [lang](#lang)
 - [title](#title)
 - [style](#style)
 - [<a>](#href)


---

## Atribute_Propertions
 - [Color](#Color)
    - **define name**
        - [Red Green Blue](#rgb)
        - [Red Green Blue alpha ](#rgba) 
        - [Шестнадцатеричный цвет](#rrggbb)
        - [HSL and HSLA Colors](#hsl)
        - [HSL and HSLA Colors alpha](#hsla)
    

---

## [Cmment](#comment)

---


# Description Elements

 ## pre 
 - Элемент HTML \<**pre**>определяет предварительно отформатированный текст.
 Текст внутри \<**pre**> элемента отображается шрифтом фиксированной ширины (обычно Courier), при этом сохраняются как пробелы, так и переносы строк:

    >example

    ```html
    <pre>
        My Bonnie lies over the ocean.

        My Bonnie lies over the sea.

        My Bonnie lies over the ocean.

        Oh, bring back my Bonnie to me.
    </pre>
    ```

---

 ## hr
 - Тег \<hr> <hr>определяет тематический разрыв на HTML-странице и чаще всего отображается в виде горизонтальной линии.
Элемент \<hr> используется для разделения содержимого (или определения изменения) на HTML-странице:

    >example

    ```html
    <h1>This is heading 1</h1>
    <p>This is some text.</p>
    <hr>
    <h2>This is heading 2</h2>
    <p>This is some other text.</p>
    <hr>
    ```


    >example

    ```html
        <em>This text is emphasized</em>
        <strong>This text is important!</strong>
        <b>This text is bold</b>
    ```

---

# Description **Atribute**

 ## lang
- Вы всегда должны включать **lang** атрибут внутри <**html**>тега, чтобы объявить язык веб-страницы. Это предназначено для помощи поисковым системам и браузерам.

    >example

    ```html
    <!DOCTYPE html>
        <html lang="en">
            <body>
            ...
            </body>
        </html>
    ```
 - Коды стран также могут быть добавлены к коду языка в lang атрибуте. Таким образом, первые два символа определяют язык HTML-страницы, а последние два символа определяют страну.

    >example

    ```html
    <!DOCTYPE html>
        <html lang="en-US">
            <body>
            ...
            </body>
        </html>
    ```

---

 ## title
 - Атрибут titleопределяет некоторую дополнительную информацию об элементе.
Значение атрибута title будет отображаться в виде подсказки при 
    >example
    наведении курсора мыши на элемент:
    ```html
        <p title="I'm a tooltip">This is a paragraph.</p>
    ```
 ---
 
 ## style
 - Задать стиль HTML-элемента можно с помощью атрибута style.
 Атрибут HTML styleимеет следующий синтаксис:

    >example

    ```html
    <tagname style="property:value;">
    <h1 style="text-align:center;">Centered Heading</h1>
    <p style="text-align:center;">Centered paragraph.</p>
    <h1 style="font-size:300%;">This is a heading</h1>
    <p style="font-size:160%;">This is a paragraph.</p>
    ```
---
## href

- Абсолютные URL-адреса против относительных URL-адресов
В обоих приведенных выше примерах в атрибуте используется абсолютный URL (полный веб-адрес) href.

    ```html    
    <h2>Absolute URLs</h2>
    <p><a href="https://www.w3.org/">W3C</a></p>
    <p><a href="https://www.google.com/">Google</a></p>

    <h2>Relative URLs</h2>
    <p><a href="html_images.asp">HTML Images</a></p>
    <p><a href="/css/default.asp">CSS Tutorial</a></p>
    ```

Локальная ссылка (ссылка на страницу того же веб-сайта) указывается с помощью относительного URL (без части «https://www»):

Ссылки HTML — используйте изображение в качестве ссылки
Чтобы использовать изображение в качестве ссылки, просто поместите <img> тег внутрь <a>тега:

>>example
```html

    <a href="default.asp">
    <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
    </a>

```

 -  **_self** - Default. Opens the document in the same window/tab as it was clicked
 - **_blank** - Opens the document in a new window or tab
 - **_parent** - Opens the document in the parent frame
 - **_top** - Opens the document in the full body of the window

>>example
 ```html
    <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
 ```


- Ссылка на адрес электронной почты
    Используйте **mailto:внутри** hrefатрибута для создания ссылки, которая открывает почтовую программу пользователя (чтобы он мог отправить новое электронное письмо):
    <br/>

    >>example

```html 
<a href="mailto:someone@example.com">Send email</a>
```
Кнопка как ссылка
Чтобы использовать HTML-кнопку в качестве ссылки, необходимо добавить код JavaScript.

JavaScript позволяет указать, что произойдет при определенных событиях, на>>example
 при нажатии кнопки:

>>example

```html
    <button onclick="document.location='default.asp'">HTML Tutorial</button>
```
Совет: узнайте больше о JavaScript в нашем руководстве по JavaScript .

Заголовки ссылок
Атрибут titleопределяет дополнительную информацию об элементе. Информация чаще всего отображается в виде текста подсказки при наведении мыши на элемент.

>>example

```<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our
html HTML Tutorial</a>
```
Подробнее об абсолютных и относительных URL-адресах

>>example

Используйте полный URL-адрес для ссылки на веб-страницу: 

```html
    <a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>
```

>>example

Ссылка на страницу, расположенную в папке html на текущем веб-сайте: 

```html
    <a href="/html/default.asp">HTML tutorial</a>
```

>>example

Ссылка на страницу, расположенную в той же папке, что и текущая страница: 

```html
    <a href="default.asp">HTML tutorial</a>
```

Подробнее о путях к файлам можно прочитать в главе Пути к файлам HTML .

- Краткое содержание главы
- Используйте <a>элемент для определения ссылки
- Используйте hrefатрибут для определения адреса ссылки.
- Используйте targetатрибут, чтобы определить, где открыть связанный документ.
- Используйте <img>элемент (внутри <a>), чтобы использовать изображение в качестве ссылки
- Используйте mailto:схему внутри hrefатрибута для создания ссылки, которая открывает - программу электронной почты пользователя.

---

>## Color
 - Цвета HTML указываются с помощью предопределенных названий цветов или значений RGB, HEX, HSL, RGBA или HSLA.

Названия цветов
В HTML цвет можно указать с помощью имени цвета:
- Помидор
- Апельсин
- DodgerBlue
- СреднийSeaGreen
- Серый
- Сланцево-голубой
- Фиолетовый
- Светло-серый

> example 

    >example

```html

    <h1 style="background-color:DodgerBlue;">Hello World</h1>
    <p style="background-color:Tomato;">Lorem ipsum...</p>

```

 >> ## rgb
   Значения цветов RGB <br>
   В HTML цвет можно указать как значение RGB, используя    следующую формулу:
   ```html
    rgb( красный, зеленый , синий )
   ```
   Каждый параметр (красный, зеленый и синий) определяет     интенсивность цвета со значением от 0 до 255.
   
   Это означает, что существует 256 x 256 x 256 =   16777216    возможных цветов!<br>
   Например, `rgb(255, 0, 0)` отображается красным    цветом,    поскольку для красного цвета установлено   максимальное    значение (255), а для двух других   (зеленого и синего) — 0.<br>
   Другой пример:` rgb(0, 255, 0)` отображается зеленым   цветом,    поскольку для зеленого установлено   максимальное значение    (255), а для двух других   (красного и синего) установлено    значение 0.  <br>
   Чтобы отобразить черный цвет, установите все   параметры    цвета на 0, например:` rgb(0, 0, 0)`.<br/>
   Чтобы отобразить белый цвет, установите все параметры   цвета  на 255, например:` rgb(255, 255, 255).` <br/>

>>>### rgba

- Цветовые значения RGBA представляют собой расширение    цветовых значений RGB с помощью альфа-канала, который    определяет непрозрачность цвета.

    Значение цвета RGBA указывается с помощью:

    rgba( красный, зеленый , синий, альфа )

    Параметр альфа — это число от 0,0 (полностью прозрачный)    до  1,0 (совсем непрозрачный):

    Поэкспериментируйте, смешивая значения RGBA ниже:

>example

```html

    rgba(255, 99, 71, 0.5)  

```

## rrggbb
 - Значения цвета HEX
В HTML цвет можно указать с помощью шестнадцатеричного значения в форме:<br/>
    rrggbb<br/>
    Где rr (красный), gg (зеленый) и bb (синий) — шестнадцатеричные значения от 00 до ff (то же самое, что и десятичные 0-255).<br/>
    Например, #ff0000 отображается красным цветом, поскольку для красного цвета установлено максимальное значение (ff), а для двух других (зеленого и синего) установлено значение 00.

    Другой пример: #00ff00 отображается зеленым цветом, поскольку для зеленого цвета установлено максимальное значение (ff), а для двух других (красного и синего) установлено значение 00.<br/>
    Чтобы отобразить черный цвет, установите все параметры цвета на 00, например: #000000.<br/>
    Чтобы отобразить белый цвет, установите все параметры цвета на ff, например: #ffffff.<br/>
    Поэкспериментируйте, смешивая указанные ниже значения HEX:

```html
    <h1 style="background-color:#ff0000;">#ff0000</h1>
    <h1 style="background-color:#0000ff;">#0000ff</h1>
    <h1 style="background-color:#3cb371;">#3cb371</h1>
    <h1 style="background-color:#ee82ee;">#ee82ee</h1>
    <h1 style="background-color:#ffa500;">#ffa500</h1>
    <h1 style="background-color:#6a5acd;">#6a5acd</h1>
```

>> ## hsl


- HSL означает оттенок, насыщенность и яркость.<br/>
    Цветовые значения HSLA являются расширением HSL с альфа-каналом (непрозрачностью).<br/>
    Значения цвета HSL
    В HTML цвет можно задать с помощью оттенка, насыщенности и яркости (HSL) в следующей форме:<br/>
    hsl( оттенок , насыщенность , яркость )<br/>
    Оттенок — это градус на цветовом круге от 0 до 360. 0 — красный, 120 — зеленый, а 240 — синий.<br/>
    Насыщенность — это процентное значение. 0% означает оттенок серого, а 100% — полный цвет.<br/>
    Яркость также является процентным значением. 0% — черный, 100% — белый.<br/>
    Поэкспериментируйте, смешивая значения HSL ниже:

    >> [example](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_color_hsl)
    
    ```html

        <h1 style="background-color:hsl(0, 100%, 50%);">hsl(0, 100%, 50%)</h1>
        <h1 style="background-color:hsl(240, 100%, 50%);">hsl(240, 100%, 50%)</h1>
        <h1 style="background-color:hsl(147, 50%, 47%);">hsl(147, 50%, 47%)</h1>
        <h1 style="background-color:hsl(300, 76%, 72%);">hsl(300, 76%, 72%)</h1>
        <h1 style="background-color:hsl(39, 100%, 50%);">hsl(39, 100%, 50%)</h1>
        <h1 style="background-color:hsl(248, 53%, 58%);">hsl(248, 53%, 58%)</h1>

    ```
>> ## hsla
    
>>example

    ```html

        <h1 style="background-color:hsla(9, 100%, 64%, 0);">hsla(9, 100%, 64%, 0)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 0.2);">hsla(9, 100%, 64%, 0.2)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 0.4);">hsla(9, 100%, 64%, 0.4)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 0.6);">hsla(9, 100%, 64%, 0.6)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 0.8);">hsla(9, 100%, 64%, 0.8)</h1>
        <h1 style="background-color:hsla(9, 100%, 64%, 1);">hsla(9, 100%, 64%, 1)</h1>
   
    ```
---


 ## comment

 - first method

    >example

    ```html
        <p>This is a paragraph.</p>
        <!-- <p>This is another paragraph </p> -->
        <p>This is a paragraph too.</p>
    ```

 - second method

    >example

    ```html
        <p>This is a paragraph.</p>
        <!--
        <p>Look at this cool image:</p>
        <img border="0" src="pic_trulli.jpg" alt="Trulli">
        -->
        <p>This is a paragraph too.</p>
    ```

---