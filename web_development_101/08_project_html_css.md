# Проект: HTML/CSS

Для этого мини-проекта вы разберете существующую веб-страницу и воссоздадите её снова. Не беспокойтесь, если ссылки не будут никуда вести и поисковая форма не будет работать, когда вы её отправите. Цель в том, чтобы начать думать о том, как элементы размещаются на странице, как они выравниваются и стилизуются. Возможно, некоторые из вас пробуют создать что-то с помощью HTML впервые (волнующе, не правда ли?).

Используйте инструменты разработчика из вашего браузера (правый клик на любом месте страницы и клик по пункту "исследовать элемент"), они станут вашими лучшими друзьями. Создайте страницу в текстовом файле с расширением .html и откройте её в своем браузере, чтобы увидеть, как она выглядит (или попробуйте использовать [CodePen](http://codepen.io/pen/) или [jsfiddle.net](http://www.jsfiddle.net)).

## Попробуйте это, прежде чем начинать

Эти навыки будут полезными, когда вы начнете писать код. Вы можете попробовать их, или, по крайней мере, убедиться, что знаете, как это делать:

1. Два способа двигать div по странице
1. Зафиксировать div внизу или вверху страницы
1. Определить цвета существующей страницы
1. Взять URL изображения с существующей страницы
1. Выровнять элемент по центру (по горизонтали)
1. Определить три способа, при помощи которых вы можете включить CSS-стили на страницу
1. Понимание, как использовать классы и id, чтобы присвоить CSS-стили конкретным элементам на странице
1. Создать очень простую форму (даже если она никуда не ведет)

## Настройка Github-репозитория для вашего проекта (не обязательно)

Вам наверняка захочется упорядочить все проекты по мере прохождения этого курса, и лучшим способом сделать это будет использование Гитхаба. Он похож на систему хранения файлов. Сервис хранит файлы с исходным кодом в облаке и позволяет любому желающему просмотреть их. Вы уже создали ваш аккаунт в уроке ["Проект: Установки"](/basics-of-web-development/project-installations), настало время им воспользоваться.

Эти инструкции будут одинаковыми для каждого выполняемого нами проекта. Поначалу они могут показаться странными (особенно, если вы еще ничего не знаете о Git, этот пробел мы восполним позднее), но не стоит беспокоиться - вы освоитесь с ними, поскольку будете проделаете эти действия еще множество раз. Если же у вас что-то пошло не так - не раздражайтесь и не расстраивайтесь, это можно отложить на некоторое время. Написание кода сейчас важнее, чем Git!



1. Если вы еще этого не сделали, создайте на своем компьютере папку и назовите её `codenamecrud`. В ней мы будем хранить все наши проекты.
2. Залогиньтесь в свой аккаунт на Github.com
3. Создайте репозиторий для проекта, [следуя инструкциям на Github](https://help.github.com/articles/create-a-repo) и назовите его `google-homepage` (вместо `Hello-World`). Пометьте ваш репозиторий как "Публичный" (Public).
4. Перейдите в свежесозданный репозиторий (`http://github.com/ВАШ_ЛОГИН/google-homepage`) и взгляните на его содержимое. Если вы прокрутите страницу вниз, вы увидите, что файл `README` был только что создан и вы просматриваете его содержимое.
5. Скачайте созданный репозиторий на свой компьютер, используя команду `$ git clone`. [Эта статья может быть полезной](http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository)(смотрите вторую часть). В общем, вам нужно будет получить URL вашего репозитория (он заканчивается на `.git`), чтобы команда `clone` знала, откуда брать репозиторий. Вы можете найти URL для клонирования репозитория в правой колонке (называется "HTTPS clone URL") на главной странице вашего репозитория на Гитхабе. Полная команда будет выглядеть как-то наподобие `git clone https://github.com/codenamecrud/curriculum.git`. Она скачает репозитория с вашего аккаунта на Гитхабе на ваш компьютер.
6. Командой `cd` перейдите в директорию вашего проекта (она должна была быть создана при клонировании) и откройте файл `README` в текстовом редакторе. Измените его, написав название проекта и ссылку на этот урок-проект на codenamecrud.ru.
6. Сделайте коммит (сохранение) обновленного `README` в ваш репозиторий на Github, используя следующие команды:

    ```language-bash
    # добавляет все файлы, которые есть в текущей директории и которые вы недавно
    # изменили (теперь они помечены как "готовые к коммиту")
    $ git add -A

    # делает коммит для всех "подготовленных" файлов в ваш локальный репозиторий
    $ git commit -m "update README"

    # отправляет содержимое вашего локального репозитория на Github, обновляя
    # удаленный репозиторий вашего проекта
    $ git push origin master
    ```

*Когда вы будете работать над проектами, вы, вероятно, несколько раз выполните команды `git add` + `git commit`, прежде чем будете готовить отправить изменения на Github командой `git push`.*

Вы должны увидеть изменения на вашей странице README на Github после обновления страницы.

*Если вы еще не чувствуете себя комфортно, используя Git из командной строки, вы можете просто нажать кнопку "Редактировать" в веб-интерфейсе Github и отредактировать файл прямо на сайте. Об этом рассказывается во второй части [упомянутой выше статьи](https://help.github.com/articles/create-a-repo) о том, как создавать репозиторий*

Заметка: Все команды Git должны выполняться внутри директории вашего проекта (в той, в которой вы вводили `git init`), иначе вы получите ошибку в ответ!

Окей, хватит пока с нас Git - настало время писать код!

## Легкая версия: Создаем главную страницу [Google.com](http://www.google.com)
(простейшую, с одним лишь полем для поиска).


Внутри директории вашего проекта создайте файл index.html

  1. Подсказки:
    * НЕ БУДЬТЕ ПЕРФЕКЦИОНИСТОМ! Вы только пытаетесь сделать её *похожей* на google.com, а не полностью заставить работать, как поисковик, и страница не должна выглядеть полной копией, пиксель в пиксель. Любые выпадающие меню или отправка формы, или подсветка при наведении должны быть проигнорированы.
    * ИСПОЛЬЗУЙТЕ GOOGLE! Вы, вероятнее всего, встретитесь с какими-либо препятствиями, разобраться самостоятельно с которыми не сможете. Сделайте то, ч��о делают в таком случае разработчики... погуглите вашу проблему!
    * Если вы исполнились раздражения, пытаясь заставить кнопки или поля ввода выглядеть так, как вы хотите (например, они попросту не изменяют свой внешний вид), посмотрите в css-свойство `-webkit-appearance: none;` или `-moz-appearance`, если используете Firefox.
  2. Для начала просто поместите основные элементы на страницу (картинку логотипа и поисковую форму), затем установите их на свои места по горизонтали. Вы можете скачать логотип Google или напрямую использовать ссылку на него внутри вашего тега `<img>`.

  3. Далее сделайте навигационную панель наверху страницы, сначала добавьте содержимое, а потом попробуйте позиционировать его. Посмотрите, [как создать горизонтальную панель при помощи CSSS](http://www.w3schools.com/css/css_navbar.asp), если у вас возникли с этим проблемы.
  4. Наконец, создайте футер, который должен быть очень похож на верхнюю навигационную панель.
  5. В общем, постарайтесь самостоятельно сделать как можно больше, прежде чем обратитесь к инструментам разработчика (или просмотру исходного кода страницы) за дальнейшей помощью.
  6. Отправьте ваш проект на Github, следуя инструкции выше!

## Сложная версия (не обязательно): Создаем [страницу поисковых результатов Google.com](https://www.google.com/search?q=создать+эту+страницу)

Вы должны уметь повторно использовать большую часть кода из написанного ранее, если начинаете выполнять это задание. Еще раз, не стоит беспокоиться о неработающих ссылках, не отправляющихся формах и жестко прописанных результатах поисковой выдачи (которую вы, конечно же, будете делать), просто сосредоточьтесь на размещении и упорядочивании содержимого на странице.

Заметка: имена всех классов и id, которые вы можете увидеть, исследовав исходный код главной страницы Google, являются бессмысленными строками (вроде `<div class='srg'>`). Причиной этому является *Минификация* ([посмотрите запись на Википедии](http://en.wikipedia.org/wiki/Minification_(programming))), которая убирает или сокращает ненужные символы и названия, чтобы ускорить загрузку страницы. HTML (или Javascript, или CSS) файл будет меньше, но браузер по-прежнему сможет его читать.

## Дополнительные ресурсы

*Этот раздел содержит полезные ссылки на дополнительные материалы. Они не обязательны, так что расценивайте их как нечто полезное, если вы хотите поглубже погрузиться в тему*

Если вы все еще чувствуете неуверенность в своем понимании HTML и CSS, это нормально! Пока вам не нужно быть во всем этом экспертом. Эти ресурсы должны помочь, если вы хотите укрепить свежеприобретенные знания и облегчить понимание узнанного:


* Посмотрите все [бесплатные видео по HTML](http://teamtreehouse.com/library/websites/html/introduction) от Treehouse и пройдите тест.
* Посмотрите [быстрое введение в CSS](http://teamtreehouse.com/library/websites/build-a-simple-website/website-basics/introduction-to-css) от тех же авторов.
* Если вы хотите увидеть искусство CSS, загляните в [Сад дзен CSS](http://www.csszengarden.com/), который собирает присланные примеры использования HTML и CSS, выглядящие как настоящие произведения.
* Прочтите [Руководство по HTML&CSS Шэя Хоува](http://learn.shayhowe.com/html-css/terminology-syntax-intro). Первый урок даст вам прочный фундамент и вы можете изучить все остальное для более глубокого понимания.
* Узнайте больше о Github, используя это руководство: https://try.github.io или прочтите больше в этой статье: http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1
