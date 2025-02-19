# Совместная работа над файлами в репозитории

Пока ты работал над файлом локально, в удалённом репозитории появилась его новая версия.

Чтобы отправить свои изменения, следуй шагам ниже.

1. **Сохрани изменения** в локальном файле (**Ctrl+S**),

2. **Закоммить свои правки:**
   ```bash
   git add <имя_файла>
   git commit -m "Пояснения к коммиту"
   ```

3. **Скачай обновления с удалённого репозитория:**
   ```bash
   git fetch origin
   ```

4. **Обнови свою локальную ветку (например, test):**
   ```bash
   git pull origin test
   ```
   Если файлы из удалённой ветки отличаются от локальных, Git сообщит о конфликтах:
     * открой нужный файл в редакторе кода локально,
     * разреши конфликты в разделе контроля версий,
     * сохрани файл. 

   Затем снова выполни:
     ```bash
     git add <имя_файла>
     ```

6. **Запуши свои изменения:**
   ```bash
   git push origin test
   ```

Теперь твои с коллегами изменения объединены.
```
