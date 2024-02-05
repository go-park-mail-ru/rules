# Go Course Rules

Правила курса по Go для студентов.

## В самом начале

Нужно объединиться в команды и выбрать себе ментора.

Менторы по фронтенду и Go - разные люди:

1. ментор по Go допускает к РК по Go и помогает вам с освоением бекенд разработки;
2. ментор по фронтенду допускает вас к РК по фронтенду и отвечает за продуктовые требования.

## Домашние задания

На курсе 2 домашних задания. Первое задание сделано, чтобы поиграться со стандартной библиотекой и просто попробовать Go в деле, второе - на понимание асинхронной модели Go. Если сделаете второе ДЗ, то познаете дзен асинхронной разработки в Go и сможете решить практически любую задачку. :)

Каждая домашка оценивается в 5 баллов.

Выполнить первое ДЗ нужно **до первого РК**, второе - **до второго РК**. Выполнить - значит получить галочку в ведомости напротив вашей фамилии.
Ведомость будем заполнять по мере появления команд.

Условие лежит в файликах
https://github.com/go-park-mail-ru/lectures/tree/master/1-basics/homework
и https://github.com/go-park-mail-ru/lectures/blob/master/2-async/99_hw.zip.

Для сдачи вам нужно в ПРИВАТНОМ репозитории на GitHub или GitLab написать код, дать доступ на чтение вашему ментору,
пройти ревью ментора, дать доступ пользователям `rvasily`, `skinass`, `KaymeKaydex`, `svetlanasadovnikova` и `K1ola` и кинуть на проверку
преподавателю.

### Списывание

Домашние задания предназначены для **самостоятельного** выполнения. Это значит что вы делаете домашку сами, не общаясь ни с кем кроме препода или менторов. Не общаясь с командой, не обсуждая, не вырабатывая общее решение.

За списывание будем штрафовать **-10 баллов** и у того кто списал, и у того кто дал списать. Несданная домашка - это не так больно, как штраф за списывание. Мы знаем как выглядит списанная домашка. Общее решение на команду приравнивается к списыванию.

Не рискуйте, оно того не стоит.

## Рубежный контроль

На курсе 4 РК. К каждому РК нужно получить допуск от ментора по Go. За сутки до РК в ведомости на каждую команду будет назначен проверяющий преподаватель.

Если вы не можете прийти на РК, нужно предупредить преподавателя лично в Telegram заранее. Тогда штрафы за пересдачу работать не будут.

### Продуктовые требования

На курсе мы делаем продукт. К каждому проекту из таблички есть требования к каждому РК. Это называется продуктовыми требованиями. Продуктовые требования обязательны во всей своей полноте. Это значит что если любое из продуктовых требований не выполнено - допуска на РК нет.

Решение которое вы показываете на РК должно быть полностью вашим. Любые заимствования и копи-паста караются немедленным отчислением.

На РК показывается продукт целиком. Это значит что у вас должен быть и фронт, и бек. Показывать фронт на моках бека нельзя, показывать фронт с беком на node.js нельзя, показывать бек без фронта на курл/постман запросах нельзя. 

Продуктовые требования не могут быть выполнены формально, фича должна полноценно работать и на фронте, и на беке. Например, если есть требование валидации емейла, то она должна быть и на клиенте, и на сервере.

Контент в проектах на РК должен быть настоящий. Мемасики, трешевые картинки, шмешнявочки и котики не допускаются. В текстах аналогично - test, tesst, sdfgh быть не должно. Во всех аватарах всегда должна быть настоящая фотка. Контент, который грузиться при демонстрации так же должен быть нормальным. За это будет снижаться балл.

Продуктовые требования не могут трактоваться в сторону уменьшения работы. Например, если есть что-то про оплату - значит там должна быть интеграция с ЮМани или любым другим платежным шлюзом. Если есть сомнения - лучше уточнить понимание у препода в общем чате.

### Технические требования

За неделю до РК на портал будет выложен пост с техниескими требованиями к РК и разбалловкой по каждому требованию. Все требования основаны на пройденном материале и выданных ДЗ после лекций.

Прежде чем проверять технические требования к РК, преподаватель проверит продуктовые требования. Если продуктовые требования не выполнены, то команда не допускается к РК и отправляется на пересдачу.

Оценка за технические требования. Если требование не выполнено - ставится 0 баллов, например если тестовое покрытие 48% при требовании 50% - это значит требование не выполнено. Если есть недочеты в реализации - по усмотрению преподавателя оценка может быть снижена или может быть проставлен 0.

Технические требования не могут быть выполнены формально, все должно быть сделано на совесть.

Тесты должны быть реализованы полноценно, а не ради тестового покрытия. Это значит что они должны тестировать правильность работы вашего кода, а не просто проверять что статус-код вернулся не 500. Кроме случае когда явно сказано что надо сделать мок-тесты (gomock, sqlmock на РК-2) - можно делать интеграционные сценарные тесты. Это когда вы последовательно дергаете апишки, проходя весь флоу работы фичи. Это сразу даст хороший объем покрытия.

### Пересдача

Пересдача РК возможна на следующем РК (при наличии допуска). За пересдачу можно получить не более 50% набранных баллов.

Тестовое покрытие пересдать нельзя. Если оно не готово к моменту РК - это окончательно. Потому что на следующем РК будет свое тествое покрытие.

После РК-4 пересдать ничего нельзя, потому что обычно через несколько дней защита.

## Доп баллы

Баллы выдаются за фуллстек (фронт+бек) фичу с новой сущностью, новым функционалом, то что надо будет хранить в отдельной новой таблице. Ну и конечно продуктово оно должно давать продукту какую-то ценность, вписываться в сам продукт. Например, подтверждение регистрации не тянет, потому что не является новой сущностью. Фичу (фичи) надо придумать с ментором, потом прислать преподу на согласование.

За такую фуллстек-фичу выдается 4 балла.

Стратегически выгоднее сначала делать все к РК, потому что за РК выдается значительно больше баллов. Не сделать что-то к РК потому что вы делали доп фичу - не выгодно.

Решать вопрос с доп баллами лучше сразу как появилась потребность в них, а не в конце семестра.

## Хакатон

В середине курса будет хакатон. Проводится он обычно в выходной день в офисе компании и длится весь день (8 часов).
На хакатон выдается задание (продуктовая фича), которое надо выполнить и сдать преподавателям в конце хакатона.

Если хакатон по каким либо причинам отменяется, то баллы вместо него ставятся за защиту.

## Защита

Без выступления на защите закончить курс нельзя. Допуск к защите выдается на курсе фронтенда.

Вам нужно показать работающий продукт после семестра обучения, поэтому для допуска нужно выполнить все продуктовые требования.

После защиты нельзя ничего досдать.

## Посещаемость

На курсе нет разделения фронт-бек, все лекции всех курсов **обязательны** к посещению, курс очный. При недостаточной посещаемости преподаватель может по желанию запросить всю группу (или только отсутствующих) писать конспект лекции. Конспект лекции в этом случае будет обязательный для завершения курса, без него курс будет закончить нельзя. Одинаковые конспекты будут приравниваться к списыванию и штрафоваться на -10 баллов.

## Спорные ситуации

Все спортыне ситуации решаются в пользу преподавателей. 

Все найденные лазейки чтобы не делать что-то или упростить будут трактоваться как не применимые и что это не разрешено.

## Типичные ошибки

* Не прийти на РК и предупредить препода об этом.
* Ничего не делать 2 недели и начать суетиться за пару дней до РК, с планом все успеть в последний день. Как правило получается где-то на половину баллов.
* Слушать как сокомандник кормит завтраками и не снимать с него задачи, перераспределяя их по другим членам команды. Такие случаи надо сразу эскалировать в менторов и преподов. Бездельники нам не нужны, лучше мы их отчислим и команда меньшим составом все затащит, чем вы будете полагаться на того кто вас подведет.
* Иметь плохо сданные РК так что не хватает на 3-ку, но ничего не делать до конца семестра и начать суетиться после РК-4. То что где-то баллов вы не добираете вы знаете сразу после РК и решать эту ситацию лучше так же сразу после РК. В конце семестра ситуация как правило заканчивается отчислением.
