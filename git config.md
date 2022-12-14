[< к содержанию](./readme.md)

# GIT config

В состав **Git** входит утилита *git config*, которая позволяет просматривать и настраивать параметры, контролирующие все аспекты работы **Git**, а также его внешний вид. Эти параметры могут быть сохранены в трёх местах:
* Файл ***[path]/etc/gitconfig*** содержит значения, общие для всех пользователей системы и для всех их репозиториев. Если при запуске ***git config*** указать параметр --***system***, то параметры будут читаться и сохраняться именно в этот файл. Так как этот файл является системным, то вам потребуются права суперпользователя для внесения изменений в него.

* Файл ***~/.gitconfig*** или ***~/.config/git/config*** хранит настройки конкретного пользователя. Этот файл используется при указании параметра --***global*** и применяется ко всем репозиториям, с которыми вы работаете в текущей системе.

* Файл ***config*** в каталоге **Git**  репозитория, который вы используете в данный момент, хранит настройки конкретного репозитория. Вы можете заставить **Git** читать и писать в этот файл с помощью параметра --***local***, но на самом деле это значение по умолчанию. Неудивительно, что вам нужно находиться где-то в репозитории **Git**, чтобы эта опция работала правильно.