# Стартовый шаблон для проекта

Данный шаблон сверстан по HTML5 и оптимизирован под Google PageSpeed, и содержит все что могло ускорить верстку и облегчить выполнение однообразных операций возникающий при старте любого проекта.  


Шаблон состоит из: 

* папка `app` :  содержит исходный код проекта;
* папка `dist`:  содержит готовый проект с html файлом, шрифтами, рисунками оптимизированные для Google PageSpeed, и минифицированные css и js файлы;
* папка `bower_components`: содержит скачанные bower пакеты;
* файл `.bowerrc`: содержит путь в паку, куда bower скачивает пакеты. Если нет этого файла, то по умалчанию скачивает в папку bower_components;
* файл `.gitignore`: содержит список директории и файлов, которых git должен игнорировать;
* файл `README.md`: содержит инструкцию для проекта;
* файл `bower.json`: файл манифест, где хранятся информации о нашем bower пакете и о их зависимостях; 
* файл `gulpfile.js`: содержит gulp таски
* файл `package.json`: файл манифест, где хранятся информации о нашем проекте и о их зависимостях; 


## Как использовать шаблон

1. [Скачайте](https://github.com/nurbol-sarsenbayev/start-template-gulp/archive/master.zip) start-template-gulp с GitHub;
2. Установите модули Node.js выполнив команду **npm i** в терминале;
3. Установите пакеты Bower командой **bower i** в терминале;
4. Запустите Bower-Installer командой **bower-installer**, чтобы копировать только нужные файлы с папкой bower_components в папку app/libs; 
5. Если хотите установить другие пакеты или библиотеки, тогда 
    * выполняете в терминале комманду **bower i --save название_пакета**;
    * проверяете все ли нужные файлы пакета написаны в файле bower.json скаченного пакета в свойстве **main**;
    * если нет, тогда в файле bower.json нашего проекта в свойстве sources создаем новое свойство с названием пакета, а его значением будет массив путей нужных файлов пакета; 
    * после запускаем команду **bower-installer**;
    * импортируем css файлов пакета в файле libs.sсss;
    * добавляем пути к js файлам пакета в таск libs-js в файле gulpfile.js;
    * если пакет использует шрифты или изображения, то надо их переместить в папку fonts или img, и поменять пути к этим шрифтам и изображениям в файле libs.sсss. Там будет переопределятся css значение библиотек. 


## Таски Gulp

* gulp

## Bower

**Bower** — клиентский пакетный менеджер, который упрощает установку сторонных библиотек с их зависимостями.  

Если не установлен Bower на вашем компьютере глобально, то установите выполнив в терминале комманду:
```npm
    npm install -g bower
```

Если не установлен Bower-Installer на вашем компьютере глобально, то установите выполнив в терминале комманду:
```npm
    npm install -g bower-installer
```
