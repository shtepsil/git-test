## Команды для Windows
ls или dir - покажет все файлы в текущей диретории
c:, d:, ... - сразу перейти на нужный диск

## Команды Git
- git init - инициализация репозитория (создание скрытой директории .git со всем её содержимым)
- git pull - загружает файлы с облака git и показывает какие файлы были изменены
- git checkout -- index.html - если файлв не в стэйдже, то возвращает состояние файла из последнего коммита (т.е. откатывает как бы)
- git checkout -- . - все файлы
- git reset file.txt - вынимает файл из стэйджа(т.е. после команды git add - файлы попадают в стэйдж)
- git reset . - все файлы отменяет(вынимает из стэйджа)
- git reset --soft HEAD^1 - возврат к коммиту указанному числом на конце. Есть варианты отмены (--soft| --hard) - и вроде как третий вариант есть, надо будет снова глянуть лекцию yandex по Git'у.

### Команды с ветками
- git branch - показывает все ветки. Звёздочка показывает в какой ветке мы находимся.
- git branch -v показывает последний коммит, который был сделан в этой ветке.
- git branch имя ветки - создаёт новую ветку
- git checkout имя ветки - переход на указанную ветку
- git checkout -b имя ветки - создаёт ветку и сразу же в неё переходит
- git checkout хэш коммита - переход к указанному коммиту (можно переходить назад на коммит, и оттуда уже создавать новые ветки)
- git branch -D имя ветки - удаление ветки



## Git config
- git config --global user.name "Sergey Brazhnikov"
- git config --global user.email akvarius_84@mail.ru
> Проверка config'a
> > git config --list

## …or create a new repository on the command line
- echo "# git-test" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin https://github.com/shtepsil/git-test.git
- git push -u origin main

## …or push an existing repository from the command line
- git remote add origin https://github.com/shtepsil/git-test.git
- git branch -M main
- git push -u origin main

## Алиасы
