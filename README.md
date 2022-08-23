# Инструкция по работе с Git
Скачать Git можно по [этой ссылке](https://git-scm.com/downloads).

Инструкции по установке для разных платформ [здесь](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-Git).

## Первые шаги с Git:
1. `git --version` - проверить установленную версию программы git (проверить - установлен ли git вообще)
2. `git config --global user.name "Your Name"` - задать имя пользователя Git
3. `git config --global user.email your@email.com` - задать адрес электронной почты пользователя Git

## Полезные команды Git:
- `git init` - инициализация репозитория в текущей папке
- `git status` - показывает текущее состояние и наличие несохранённых изменений
- `git add filename.txt` - добавить файл в индекс для отслеживания изменений
- `git commit -m "Commit Message"` - зафиксировать изменения/”закоммитить”
    - `git commit -а` - флаг `-a` автоматически добавляет в коммит ранее добавленные файлы через `git add `
- `git log` - показать журнал изменений/коммитов
    - `git log --oneline` - показать журнал коммитов с однострочном виде с кратким хэшем
    - `git log -p` - показать журнал коммитов с подробностями о внесённых изменениях
- `git checkout [hash]` - переключить состояние репозитория к определённому коммиту
    - `git checkout master` - возврат к актуальному состоянию (последнему коммиту)
- `git diff` - показать разницу между текущим файлом и сохранённым
- `git branch` - показывает список веток