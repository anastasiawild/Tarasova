# Инструкция по языку MarkDown

## Стилизация текста 

Обычный текст набираем как есть.

Новая строка .

**Полужирный текст**

*Курсив*

Цитирование в языке markDown
> Первый уровень цитирования 
>> Второй уровень цитирования

##  Списки
### Ненумерованные списки
* Лист
* Лист

 ### Нумерованный список
 1. Лист
 2. Лист

 ## WEB ссылки
 Текст [пример ссылки](http.example.com "Всплывающая подсказка")

Добавим как добавлять картинки в Markdown

Это картинка
![Картинка](картинка.jfif)

## Это репозиторий для обучения pull request
Первые шаги
Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория https://git@github.com:gulden-geekbrains/version_control.git
Выполняем команду клонирования из своей fork-копии
git clone git@github.com:*YOURE_GITHUB*/version_control.git
Создаем новую ветку и вносим необходимые изменения в файл
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"
Делаем push
git push --set-upstream origin updatereadme
Переходим на свою страницу репозитория. Выбираем ветку updatereadme и жмем кнопку Compare & pull request
Заметки
Что бы сделать push от другого пользователя необходимо выполнить команду

GIT_SSH_COMMAND='ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes' git push git@github.com:gulden-geekbrains/version_control.git
вместо user-private-key подставьте свой ключ

Можно прописать настройки для подсоединения по ssh

git config remote.origin.url git@github.com:gitusername/reponame
git config core.sshCommand "ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes"
Как подружить git с github под Windows 10
Вот видео инструкция https://youtu.be/E8cIjbJMEpE