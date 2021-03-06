Использование GitHub
====================

Аккаунт и репозитории на github.com
-----------------------------------

В первую очередь необходимо установить и настроить клиент git, указанный в [списке требуемого ПО](software.md).


Затем надо зарегистрироваться на https://github.com/. После чего можно будет создавать свои репозитории или присоединиться к работе над проектами коллег, сделав fork другого репозитория. В ходе данного курса все необходимые репозитории для вашего кода будут создаваться автоматически при помощи GitHub Classrooms, но при желании или необходимости вы можете создавать их и самостоятельно.

Теперь пошагово разберем как получить задание, выполнить его и отправить на проверку.


Выполнение домашних заданий
---------------------------

Домашние задания выполняются на платформе GitHub Classrooms, которая обеспечивает автоматическое создание репозиториев для ваших решений. 

### Получение задания

Для получения задания необходимо пройти по [ссылке для получения задания](README.md#Ссылки-для-получения-домашних-заданий) и нажать кнопку "Accept this assignment".

![Получение ДЗ](img/10homework.png?raw=true "Получение ДЗ")

При необходимости войдите в аккаунт GitHub.

![Вход в GitHub](img/1register_in_GitHub_for_Classrooms.png?raw=true "Вход в Github")

После этого система создаст для вас новый репозиторий и выдаст его адрес.

![Задание получено](img/2successful_registration.png?raw=true "Задание получено")

Перейдя по ссылке, вы окажетесь на сайте GitHub, и перед вами будет заготовка репозитория. В этом репозитории вы найдете описание задания, все необходимые информационные ресурсы и ссылки. 

Чтобы приступить к выполнению, вам будет необходимо склонировать этот репозиторий на свой жесткий диск используя git-клиент.
Если вы установили GitHub Desktop, то для этого достаточно нажать кнопку Code и выбрать Open in desktop (если не произошел автоматический запуск программы, то перезапустите браузер):

![Клонирование репозитория](img/3open_in_desktop.png?raw=true "Клонирование репозитория")

После клонирования вы сможете открыть репозиторий в проводнике Windows нажав на ссылку "Show in Explorer":

![Просмотр в проводнике](img/4open_repos_in_explorer.png?raw=true "Просмотр в проводнике")

После этого переходим к выполнению задания.

### Выполнение задания

Для выполнения задания необходимо создать проект в среде разработки (visual studio, mono develop, etc) внутри только что склонированного репозитория (можно прямо в его корне). Этот пункт обязателен, если вы создадите проект в другом месте, то не сможете отправить его на проверку.


> :warning: Важно: при отправлении кода на проверку (коммит) необходимо добавить все файлы проекта и решения (sln и csproj), а не только файл с программой (cs)!

После создания проекта нужно решить свой вариант задания в соответствии с вашим порядковым номером в списке группы.

### Сохранение изменений

После того как вы создали проект, и написали какой-то код, вы можете зафиксировать свои изменения, для того, чтобы иметь возможность вернуться к предыдущей версии кода, если вдруг у вас что-то пошло не так. Для этого сущетствует распределённая система управления версиями - Git. Это может здорово облегчить вам жизнь особенно к концу семестра, когда программы станут сложнее. Подробнее о том как это делать, и куда нажимать вы можете прочитать в этой статье:  https://ux.pub/git-dlya-novichkov-i-dizajnerov-interfejsov/.

### Если что-то не получается

Если при решении задания вы уже сломали себе (и своему соседу) голову, то не стесняйтесь задавать вопросы мне. В разделе Контакты указаны... мои контакты, если не отвечаю сразу, значит немного занят, но обязательно отвечу когда будет время. Для того, чтобы мне было проще вам помочь, заранее выложите все ваши текущие наработки на GitHub, даже если ничего не компилируется и не работает.

### Отправка решения на проверку

После того, как вы решили ваш вариант задания, и уверены, что все решено правильно (или не уверены, но дедлайн уже пришел), то изменения нужно выложить на GitHub и отправить на проверку.

Для этого необходимо в клиенте Git открыть репозиторий задания и закоммитить все изменения. Окно коммита должно выглядеть следующим образом (в списке файлов у вас могут быть другие файлы, больше или меньше):

![Создание коммита](img/5task_completed.png?raw=true "Создание коммита")

В поле Summary (1) нужно ввести текст сообщения, например, "Задание выполнено". А в поле Description можно оставить пустым, или указать какие известные недостатки есть на текущий момент. После чего нажимаем кнопку Commit to master (2) и создается новый **локальный** коммит. Затем отправляем все изменения на GitHub нажатием кнопки "Fetch origin" (3).

### Автоматическая проверка

  Чтобы просмотреть результат проверки нужно перейти в список всех коммитов нажав на ссылку подсвеченную жёлтым:

![Переход к списку коммитов](img/6automatic_check.png?raw=true "Переход к списку коммитов")

Сразу после отправки ваших изменений, на сервере будет запущена автоматическая проверка, которая может занимать до 5 минут.Результат проверки отображается иконкой напротив каждого коммита в списке коммитов на сайте GitHub.

![Список коммитов](img/9commits.png?raw=true "Список коммитов")

В этом списке вы увидите все коммиты которые совершали. Первым в списке будет последний совершенный коммит. По результатам проверки после текста сообщения будет стоять либо зеленая галочка, либо красный крест. Вам нужно добиться того, чтобы там была зеленая галочка.

![Хороший годный коммит](img/7check_true.png?raw=true "Хороший коммит")

Если же, там по какой-то причине будет не зеленая галочка, а красный крест, значит что-то пошло не так. Скорее всего, вы создали проект не в нужной папке, или не добавили его в коммит. Если не получится разобраться самостоятельно, то обратитесь за помощью ко мне.

Вы можете более подробно просмотреть свои ошибки нажав на красный крест. Эта информация очень помогает понять, что же всё-таки было сделано не так.

