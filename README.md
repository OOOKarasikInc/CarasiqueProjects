# CarasiqueProjects
## Описание идеи
1. Сайт по поиску учебной команды 2-n человек удаленно/локально для работы над каким-нибудь проектом. Идею проекта инициализировать может любой человек, но участвовать в другом проекте можно только после ухода из команды/роспуска команды.
   Результат проекта можно выложить в качестве портфолио.
   Участие в проектах бесплатное, на добровольных началах.
   По задумке данный стартап должен помочь начинающим специалистам прокачать так называемые "хард" и "софт" скиллы. Но это может развиться и в полноценную рабочую среду.
   У каждого проекта есть 5-10 тегов, которые одним словом могут описать как сам проект, так и участников. Например, <бекенд>, <дота2>, <блюз>, <политика> и так далее.
   Каждый потенциальный участник может указать в личном кабинете эти теги: так "тимлиды" могут найти вас и позвать к себе в команду.
2. Также проект рассматривается как некоторая социальная сеть по интересам, вполне себе можно завести новые знакомства.

## Текущий способ запуска 
1. Скопируйте проект ```git clone https://github.com/OOOKarasikInc/CarasiqueProjects.git```
2. В терминале проекта напишите: ```composer install```
3. Скопируйте файл ```.env.example``` в каталог проекта. Переименуйте его в ```.env```. В файл ```.env``` впишите следующие строки (либо измените значения):
```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1  
    DB_PORT=3306
    DB_DATABASE=teamwork.gg
    DB_USERNAME=root
    DB_PASSWORD=
```
4. Введите ```npm install```
5. Введите ```npm run build``` для отображения CSS-стилей
6. Введите последовательно ```php artisan key:generate``` и ```php artisan config:cache```
7. В терминале проекта напишите команду: ```php artisan migrate --seed```
8. Следом напишите команду ```php artisan serve```
9. Откройте сайт по появившемуся адресу

### Сниппет:
![Сниппет](https://i.imgur.com/N6nzqAU.png)

Есть предложения по идеям/изменениям (в том числе README, способа инициализации веб-приложения) - предлагайте.

### Уточнения по среде запуска

1. Для просмотра всех роутов: ```php artisan route:list``` 

2. Все необходимые зависимости для CSS и JS находятся в ```package.json```.

3. Версия PHP - **8.3**

4. Версия Laravel - **10.48.10**

5. Версия Ubuntu - **22.04.4 LTS**
