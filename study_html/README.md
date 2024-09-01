

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

## atribute
 - [lang](#lang)
 - [title](#title)
 - [style](#style)

---

## [Cmment](#comment)

 

---


# Description Elements

 ## pre 
 - Элемент HTML \<**pre**>определяет предварительно отформатированный текст.
 Текст внутри \<**pre**> элемента отображается шрифтом фиксированной ширины (обычно Courier), при этом сохраняются как пробелы, так и переносы строк:

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

    ```html
    <h1>This is heading 1</h1>
    <p>This is some text.</p>
    <hr>
    <h2>This is heading 2</h2>
    <p>This is some other text.</p>
    <hr>
    ```
## example

 ```html
    <em>This text is emphasized</em>
    <strong>This text is important!</strong>
    <b>This text is bold</b>
 ```

---

# Description **Atribute**

 ## lang
- Вы всегда должны включать **lang** атрибут внутри <**html**>тега, чтобы объявить язык веб-страницы. Это предназначено для помощи поисковым системам и браузерам.

    ```html
    <!DOCTYPE html>
        <html lang="en">
            <body>
            ...
            </body>
        </html>
    ```
 - Коды стран также могут быть добавлены к коду языка в lang атрибуте. Таким образом, первые два символа определяют язык HTML-страницы, а последние два символа определяют страну.

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
Значение атрибута title будет отображаться в виде подсказки при наведении курсора мыши на элемент:
    ```html
        <p title="I'm a tooltip">This is a paragraph.</p>
    ```
 ---
 
 ## style
 - Задать стиль HTML-элемента можно с помощью атрибута style.
 Атрибут HTML styleимеет следующий синтаксис:

    ```html
    <tagname style="property:value;">
    <h1 style="text-align:center;">Centered Heading</h1>
    <p style="text-align:center;">Centered paragraph.</p>
    <h1 style="font-size:300%;">This is a heading</h1>
    <p style="font-size:160%;">This is a paragraph.</p>
    ```
---

 ## comment

 - first method

    ```html
        <p>This is a paragraph.</p>
        <!-- <p>This is another paragraph </p> -->
        <p>This is a paragraph too.</p>
    ```

 - second method

    ```html
        <p>This is a paragraph.</p>
        <!--
        <p>Look at this cool image:</p>
        <img border="0" src="pic_trulli.jpg" alt="Trulli">
        -->
        <p>This is a paragraph too.</p>
    ```

---