<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <title>Page</title>
    <style>
        A {
            color: azure;
        }

        A:visited {
            color: #BDBDBD
        }

        body {
            background-color: black;
            color: #FFFFFF;
        }

        a {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }

        ul {
            color: azure;
        }

        li {
            color: azure;
        }

        h3 {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            color: azure;
        }

        title {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            color: azure;
        }

        textarea {
            border-radius: 25px;
            border: 5px solid greenyellow;
            background-color: #FFFFFF;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            width: 250px;
            height: 250px;
            resize: none;
        }

        label {
            color: #FFFFFF;
            font-family: 'Courier New', Courier, monospace;
        }
    </style>
</head>



<body>
    <a id="element_id"></a>
    <a id="id1"></a>
    <a id="id2"></a>
    <a id="id3"></a>
    <ol>
        <li><a href="http://www.example.com">Абсолютная гиперссылка на главную страницу сайта example.com</a></li>
        <li><a href="https://www.example.com">Абсолютную гиперссылка на главную сайта example.com в протоколе https</a>
        </li>
        <li><a href="ftp://example.com/myfile.zip">Абсолютная гиперссылка на главную страницу сайта example.com</a></li>
        <li><a href="ftp://user:password@example.com/myfile.zip">Абсолютная гиперссылка на главную страницу сайта
                example.com</a></li>
        <li><a href="http://example.com/page#element_id">Cсылка с другого сайта</a></li>
        <li><a href="#element_id">Элемент на текущей странице</a></li>
        <li><a href="https://www.example.com?id=000&xid=111">Абсолютную гиперссылка на главную сайта example.com в
                протоколе https</a></li>
        <li>
            <!--<h3>Cписок ссылок основной навигации сайта с подписями title</h3>-->
            <nav>
                <ul>
                    <li><a href="#id1" title="About">About</a></li>
                    <li><a href="#id2" title="Contacts">Contacts</a></li>
                    <li><a href="#id2" title="News">News</a></li>
                </ul>
            </nav>
        </li>
        <li><a title="Ссылка без href">Ссылка без href</a></li>
        <li><a href="" title="Пустой href">Ссылка с пустым href</a></li>
        <li><a href="https://www.example.com/" rel="nofollow" title="Нельзя переходить">Ссылка по которой запрещен
                переход поисковикам</a></li>
        <li>
            <!--<noindex>-->
            <a href="https://www.example.com/" title="No index">Нельзя индексировать</a>
            <!--</noindex>-->
        </li>
        <li>
            <h3>
                Контекстная <a href="https://www.example.com/">ссылка</a>
            </h3>
        </li>
        <li><a href="https://www.example.com/" title="Img link"> <img src="image.jpg" width="150" height="115"
                    alt="Flower"></a></li>
        <li>
            <img src="c_a_s.png" width="200" height="200" usemap="#CaS" alt="CircleandSquare">
            <map name="CaS">
                <area shape="rect" coords="76,96,192,158" href="https://www.example.com" alt="rect">
                <area shape="circle" coords="40,45,33" href="https://www.example.com" alt="circle">
            </map>
        </li>
        <li><a href="def.html">относительная ссылка на документ в текущем каталоге</a></li>
        <li><a href="/about/def.html">относительная ссылка на страницу в каталоге about</a></li>
        <li><a href="../def.html">относительная ссылка на документ в каталоге уровнем выше</a></li>
        <li><a href="../../def.html">относительная ссылка на документ в каталоге на два уровня выше</a></li>
        <li><a href="/">сокращенная на главную</a></li>
        <li><a href="/def.html">сокращенная на внутреннюю</a></li>
    </ol>
    <form action="/" method="POST">

        <label>
            Имя:<br />
            <input name="field-name-1" value="" />
        </label><br />

        <label>
            email:<br />
            <input name="field-email" type="email" placeholder="Введите вашу почту" />
        </label><br />

        <label>
            Дата рождения:<br />
            <input name="field-date" value="2019-08-13" type="date" />
        </label><br />

        Пол:<br />
        <label><input type="radio" checked="checked" name="s" value="М" />
            М </label>
        <label><input type="radio" name="s" value="Ж" />
            Ж </label><br />

        Кол-во конечностей:<br />
        <label><input type="radio" checked="checked" name="count" value="1" />
            1 </label>
        <label><input type="radio" name="count" value="2" />
            2 </label><br />
        <label><input type="radio" name="count" value="3" />
            3 </label><br />
        <label><input type="radio" name="count" value="4" />
            4 </label><br />

        <label>
            Сверхспособности:
            <br />
            <select name="field-name-4[]" multiple="multiple">
                <option value="Значение1">бессмертие</option>
                <option value="Значение2" selected="selected">прохождение сквозь стены</option>
                <option value="Значение3" selected="selected">левитация</option>
            </select>
        </label><br />

        <label>
            Биография:<br />
            <textarea name="field-name-2"></textarea>
        </label><br />


        Чекбокс:<br />
        <label><input type="checkbox" checked="checked" name="check-1" />
            С контрактом ознакомлен (а) </label><br />

        кнопка «Отправить».
        <input type="submit" value="Отправить" />
    </form>

</body>

</html>
