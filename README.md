# **🗲XML🗲**

*Задание 1. Создать внешний репозиторий c названием XML.*

`Решение`⮯

1. Перейти по ссылке
2. Нажать "New"
3. Ввести "XML" в поле "Repository name"
4. Выбрать "Public" и "Add a README file"
5. Нажать "Create repository"
---

*Задание 2. Клонировать репозиторий XML на локальный компьютер.*

`Решение`⮯

1. Нажать "Code"
2. Выбрать "SSH"
3. Нажать "Скопировать ссылку на репозиторий"
4. В GitBash зайти в папку (в которой будет размещен репозиторий)
5. Клонировать репозиторий на локальный компьютер:

```bash
git clone "git@github.com:VitasQA/XML.git"
```

6. Войти в папку "Xml":

```bash
cd Xml
```
---

*Задание 3. Внутри локального "XML" создать файл “new.xml.*

`Решение`⮯

1. Создать файл:

```bash
touch new.xml
```

2. Посмотреть состояние файлов в рабочем каталоге и индексе:

```bash
git status
``` 
---

*Задание 4. Добавить файл под гит.*

`Решение`⮯

1. Добавить содержимое рабочего каталога в индекс для последующего коммита:

```bash
git add new.xml
```
2. Посмотреть состояние файлов в рабочем каталоге и индексе:

```bash
git status
``` 
---

*Задание 5. Закоммитить файл.*

`Решение`⮯

1. Сделать снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов:

```bash
git commit -m "add new.xml"
``` 
---

*Задание 6. Отправить файл на внешний GitHub репозиторий.*

`Решение`⮯

1. Выгрузить содержимое локального репозитория в удаленный:

```bash
git push
```
---

*Задание 7. Отредактировать содержание файла “new.xml - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.*

`Решение`⮯

1. Открыть текстовый редактор Vim:

```bash
vim new.xml
```

2. Нажать " i "
3. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<aboutMe>
 <fullName>Kruglik Vitaliy Iv</fullname>
 <age>32</age>
 <pets>I don`t have any pets</pets>
 <future_salary>1500</future_salary>
<aboutMe>
```

4. Нажать "Esc"
5. Нажать ":wq"
---

*Задание 8. Отправить изменения на внешний репозиторий.*

`Решение`⮯

```bash
git add new.xml

git commit -m "modified file"

git push
```
---

*Задание 9. Создать файл preferences.xml.*

`Решение`⮯

```bash
cat > preferences.xml
```
---

*Задание 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм,сериал, еда, время года, страна которую хотели бы посетить) в формате XML.*

`Решение`⮯

1. Ввести информацию:
   
```xml
<?xml version="1.0" encoding="UTF-8"?>
<myPreferences>
 <movie>Avatar</movie>
 <series>Friends</series>
 <food>Meat</food>
 <season>Spring</season>
 <country>USA</country>
</myPreferences>
```

2. Нажать "Enter"
3. Нажать "Ctrl + D"
---

*Задание 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML.*

`Решение`⮯

1. Ввести:

```bash
cat > skills.xml
```

2. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<skills>
 <one>Mobile testing</one>
 <two>Postman</two>
 <three>Software testing theory</three>
 <four>Client-server arhitecture</four>
 <five>API testing</five>
 <six>Android Studio</six>
 <seven>Dev Tools of web browsers Google Chrome</seven>
</skills>
```

3. Нажать "Enter"
4. Нажать "Ctrl + D"
---

*Задание 12. Отправить сразу 2 файла на внешний репозиторий.*

`Решение`⮯

```bash
git add .

git commit -m "add preferences.xml and skills.xml"

git push
```
---

*Задание 13. На веб интерфейсе создать файл bug_report.xml.*

`Решение`⮯

1. Зайти в репозиторий "XML"
2. Нажать кнопку "Add file"
3. Нажать кнопку "Create new file"
4. В поле "Name your file" ввести "bug_report.xml"
---

*Задание 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit new file"
---

*Задание 15. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.*

`Решение`⮯

1. Открыть файл "bug_report.xml"
2. Нажать кнопку "Редактировать" 
3. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<BugReport>
   <summary>The login page crashes when attempting to enter a username with a special character> 
   <descriprion>WS dosen't provide information if response containes more than 89characters.</descriprion>
   <actualResult>information gets</actualResult>
   <expectedResult>information doesen't get</expectedResult>
   <requirementId>requirement</requirementId>
   <reproducedOn>Win 11</reproducedOn>
   <reproducibility>always</reproducibility>
   <workaround>no</workaround>
   <stepsTOreproduce>
        <one>1. Navigate to the login page</one>
        <two>2. Enter a username with a special character (e.g. !@#$%)>
        <three>3. Request method: POST</three>
        <four>4. Click on the 'Login' button>
        <five>5. Observe the page crashing>
   </stepsTOreproduce>
   <severity>minor</severity>
   <priority>low</priority>
</bugReport>
```
---

*Задание 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit changes"
---

*Задание 17. Синхронизировать внешний и локальный репозиторий XML.*

`Решение`⮯

```bash
git pull
```
