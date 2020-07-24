[< к содержанию](./readme.md)

## Основные операции

***git config***

Команда настройки параметров для Git на вашем компьютере.

Например, первое, что вам следует сделать после установки Git — указать ваше имя и адрес электронной почты. Это важно, потому что каждый коммит в Git содержит эту информацию, и она включена в коммиты, передаваемые вами, и не может быть далее изменена:
git config --global user.name "Your Name"
git config --global user.email "your_email@whatever.com"

***git init***

Эта команда создаёт в текущей директории новую поддиректорию с именем .git, содержащую все необходимые файлы репозитория — структуру Git-репозитория.

По сути, эта команда создает пустой репозиторий на вашем компьютере.

***git commit***

При выполнении команды git commit изменения всех файлов, внесённые в индекс, переносятся в репозиторий. При создании коммита (точки фиксации изменений) требуется указать сообщение.

Параметр -m позволяет написать сообщение из командной строки.

Обычно в сообщении пишется задача, которая решается этим обновлением, например «инициализация», «добавление счетов» или «исправление ошибки создания счёта». А правила «что написано в коммите» устанавливаются внутри команды разработчиков.

Однако общепризнанная практика состоит в том, что сообщения коммитов пишутся на английском языке «init», «add Invoices» или «fix bug of create Invoice» или на родном языке проекта и содержат достаточную информацию о точке фиксации изменений.

Пример:
git commit -m «init»

***git clone***

Эта команда служит для создания копии репозитория.

Клонировать можно как локальный (находящийся на вашем компьютере), так и удалённый (находящийся в сети) репозиторий.

Пример:
git clone https://github.com/avsudnichnikov/example