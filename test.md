
## **Знакомство с контролем версий**

**Контроль версий (контроль исходного кода)** - практика, которая позволяет отслеживать изменения исходного кода и управлять ими.

**Контроль версий необходим, чтобы:**
* хранить разные версии проекта;
* возвращаться к разным версиям проекта.

*Примеры: версии сайтов (по датам) и документов.*

Хранение версий сводится к созданию копий информации на компьютере или сервере. Функцию возврата реализуют за счёт восстановления предыдущих версий.

Таким образом, **система контроля** - это реализованная возможность замены информации с использованием сохраненных версий.

**Git** - самая популярная система контроля версий.
Программа **Git** берёт на себя контроль версий проекта и позволяет переключаться между ними. **Git** хранит не файлы целиком, а отличия между ними. Это позволяет
экономить память. 

### **Команды Git:**

+ __*git --version*__ - проверка текущей установленной версии программы;
+ __*git init*__ - инициализация: указываем папку, в которой git начнет отслеживать изменения ( создание репозитория в папке на локальной машине ). В папке создается скрытая папка __.git__;
+ __*git status*__ - показывает текущее состояние гита, есть ли изменения, которые нужно закоммитить (сохранить);
+ __*git add*__ - отслеживать добавленные файлы ( добавляет содержимое рабочего каталога в индекс (staging area) для последующего коммита ). Эта команда дается после добавления файлов;
+ __*git commit*__ + комментарий - зафиксировать или сохранить.

По умолчанию *__git commit__* использует лишь этот индекс, так что можно использовать **_git add_**
для сборки слепка нашего следующего коммита. Команда **_git commit_** берёт все данные, добавленные в индекс с помощью _**git add**_, и сохраняет их слепок во нутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок;

+ __*git log*__ - список действий и сохранений; 
+ __*git checkout*__ - переключение между версиями. Для работы нужно указать не только интересующий нас коммит, но и вернуться в тот, где работаем, при помощи команды
**_git checkout master_** ;
+ __*git diff*__ - показывает разницу между текущим файлом
и сохранённым. Перед переключением версии файла в Git используем команду __*git log*__, чтобы увидеть количество сохранений;
+ __*git branch*__ - создание новой ветки.
*__git branch -d__* - удалить ветку;
+ __*git merge*__ - слияние любой ветки с текущей;
+ __*git ignore*__ - исключение ненужных файлов из загрузки;
+ __*git log --graph*__ - отображение коммитов в виде дерева.
+ __*git log --graph*__ - отображение коммитов в виде дерева;
+ __*git clone*__ - копирует внешний репозиторий, она не только загружает все изменения, но и пытается слить все ветки на локальном компьютере и в удаленном репозитории;
+ __*git pull*__ - скачивает все из текущего репозитория и автоматически делает merge с нашей версией;
+ __*git push*__ - оправляет свою версию репозитория во внешний репозиторий. При первом её использовании нужна авторизация;
+ __*cd*__ - change directory - переход в необходимую папку.

### **Работа с удаленными репозиториями (работаем с github.com)**

#### __Как настроить совместную работу__

1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. *GitHub при создании нового репозитория подскажет, как это можно сделать:
    * git remote add origin [ссылка на удаленный репозиторий];
    * git branch -m main; 
    * git push -u origin main.
4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно, вам нужно будет авторизоваться на удалённом репозитории
5. Провести изменения “с другого компьютера”
6. Выкачать (pull) актуальное состояние из удалённого репозитория

#### **Команда Pull request**

+ команда для предложения изменений;
+ запрос на вливание изменений в репозиторий.

В больших компаниях один ответственный за проект создает аккаунт. Другие пользователи дают команду pull request. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет изменения командой push в свой аккаунт на GitHub и даёт команду pull request.

#### *Как сделать pull request*

+ Делаем _fork_ (ответвление) репозитория;
+ Делаем git clone СВОЕЙ версии репозитория;
+ Создаем новую ветку и в НЕЕ вносим свои изменения;
+ Фиксируем изменения (делаем коммиты);
+ Отправляем свою версию в свой GitHub;
+ На сайте GitHub нажимаем кнопку pull request


### **Синтаксис языка Markdown**

- **Жирный текст** обозначается ( ** или __ ) с двух сторон текста;
- *Курсивный текст* обозначается ( * или _ ) с двух сторон текста;
- ~~Зачеркнутый текст~~ обозначается ( ~~ ) с двух сторон текста;
- Выделение заголовка обозначается ( # ) в начале строки;
- Нумерованные списки обозначаются цифрами:    
    1. Элемент №1 
    2. Элемент №2
    3. Элемент №3
- Ненумерованные списки обозначают ( *, - , + ) в начале строки;
- Вложенные списки- выполняем отступы

### **Работа с изображением**

![Орущий кот :)](cat1.jpg)

### **Добавляем цитаты**

Список цитат:   

>«Никогда не ошибается тот, кто ничего не делает». Теодор Рузвельт
>>«Дай человеку власть, и ты узнаешь, кто он». Наполеон Бонапарт
>>>«Чем умнее человек, тем легче он признает себя дураком». Альберт Эйнштейн
