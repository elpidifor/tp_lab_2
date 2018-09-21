# tp_lab_2

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [ ] 1. Ознакомиться со ссылками учебного материала
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial

```bash
$ export GITHUB_USERNAME=<имя_пользователя> // Создание переменной с именем пользователя на GitHub
$ export GIST_TOKEN=<сохраненный_токен> // Создание перменной, которая хранит токен
$ alias edit=vim // Открытие текстового редактора
```

```ShellSession
$ mkdir -p ${GITHUB_USERNAME}/workspace // Создание директория workspace
$ cd ${GITHUB_USERNAME}/workspace // Переход в директорию
$ pwd // Путь к данной папке (/Users/elpidifor/elpidifor/workspace)
$ cd .. // возврат назад на одну директорию
$ pwd // (/Users/elpidifor/elpidifor)
```

```ShellSession
$ mkdir -p workspace/tasks/ // Создание подпапок в workspace
$ mkdir -p workspace/projects/
$ mkdir -p workspace/reports/
$ cd workspace // Переход в workspace
```

```ShellSession
$ npm install -g gistup /* Установка gistup */
( npm install -g gistup
```

```ShellSession
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}" // Cоздает скрытую папку, в которую записывается токен
}
EOF
```

## Report

```ShellSession
$ export LAB_NUMBER=02 // Перемнная с номером лабораторной
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER} // Клонирование репозитория
$ mkdir reports/lab${LAB_NUMBER} // Новая папка
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md
$ gistup -m "lab${LAB_NUMBER}" # enter: yes↵
```
