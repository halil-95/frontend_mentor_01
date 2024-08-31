# Study HTML

What is an HTML Element?
An HTML element is defined by a start tag, some content, and an end tag:

<tagname> Content goes here... </tagname>
The HTML element is everything from the start tag to the end tag:

<h1>My First Heading</h1>
<p>My first paragraph.</p>

## elements
 - \<h1>
 - \<p></p>
 - \<br/>
 - [\<pre>](#pre)
 - [\<hr>](#hr)


## atribute
 - [lang](#lang)
 - [title](#title)
 - [style](#style)
 




    



 



# Description elements

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


# Description atribute

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

 ## title
 - Атрибут titleопределяет некоторую дополнительную информацию об элементе.
Значение атрибута title будет отображаться в виде подсказки при наведении курсора мыши на элемент:
    ```html
        <p title="I'm a tooltip">This is a paragraph.</p>
    ```
