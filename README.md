# Gulppack. Версия с Pug + SCSS
Gulppack - сборка для автоматизации задач в повседневной front-end разработке. Компилируйте SCSS и Pug, сжимайте файлы, оптимизируйте картинки, пишите на ES6. При  каждом сохранении файла в редакторе кода браузер автоматически перезагружает страницу. Не волнуйтесь о том, что вам придётся выполнять рутинную работу.

## Что включает в себя сборка?
* [browser-sync](https://browsersync.io/docs/gulp) - живая перезагрузка веб-страницы при внесении изменений в файлы вашего проекта. Одна из опций — tunnel, которая выдаёт вам ссылку, чтобы любой желающий смог посмотреть вашу работу (в обход хостинга);
* [gulp-autoprefixer](https://www.npmjs.com/package/gulp-autoprefixer) — автоматически расставляет вендорные префиксы в CSS в соответствии с сервисом [Can I Use](https://caniuse.com/);
* [gulp-babel](https://www.npmjs.com/package/gulp-babel) - использование ES6 с [Babel](https://babeljs.io/);
* [gulp-uglify](https://www.npmjs.com/package/gulp-uglify) — минификация JS-файлов;
* [gulp-pug](https://www.npmjs.com/package/gulp-pug) — компиляция Pug в HTML;
* [gulp-concat](https://www.npmjs.com/package/gulp-concat) - объединение файлов;
* [gulp-sass](https://www.npmjs.com/package/gulp-sass) — компиляция SCSS в CSS;
* [gulp-clean-css](https://www.npmjs.com/package/gulp-clean-css) — минификация CSS-файлов;
* [gulp-sourcemaps](https://www.npmjs.com/package/gulp-sourcemaps) - карта стилей;
* [gulp-rename](https://www.npmjs.com/package/gulp-rename) — переименование файлов, добавление суффиксов и префиксов (например, добавление суффикса .min к минифицированным файлам);
* [gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin) — сжатие изображений PNG, JPG, GIF и SVG;
* [imagemin-pngquant](https://www.npmjs.com/package/imagemin-pngquant) — дополнение к gulp-imagemin для работы с PNG-изображениями;
* [imagemin-jpeg-recompress](https://www.npmjs.com/package/imagemin-jpeg-recompress) — дополнение к gulp-imagemin для работы с JPG-изображениями;
* [gulp-favicons](https://github.com/evilebottnawi/favicons) — генератор фавиконок для вашего проекта;
* [gulp-iconfont](https://www.npmjs.com/package/gulp-iconfont) — генератор иконочного шрифта из SVG-изображений;
* [gulp-iconfont-css](https://www.npmjs.com/package/gulp-iconfont-css) — генератор стилей для иконочного шрифта;
* [gulp-svg-sprites](https://www.npmjs.com/package/gulp-svg-sprites) — создание SVG-спрайтов;
* [gulp-replace](https://www.npmjs.com/package/gulp-replace) - замена строк;
* [gulp-newer](https://www.npmjs.com/package/gulp-newer) — дополнительный плагин к ```gulp-imagemin```, позволяет сжимать только новые изображения;
* [gulp-plumber](https://www.npmjs.com/package/gulp-plumber) — оповещения в командной строке (например, ошибки в Sass/SCSS);
* [gulp-debug](https://www.npmjs.com/package/gulp-debug) — отладка в терминале;
* [gulp-watch](https://www.npmjs.com/package/gulp-watch) — отслеживание изменений в ваших файлах проекта;
* [gulp-clean](https://www.npmjs.com/package/gulp-clean) — удаление файлов и папок.

## Как пользоваться?

Установите [Yarn](https://yarnpkg.com/en/docs/install).

> Yarn - это современная альтернатива npm. Yarn работает с тем же файлом ```package.json``` и так же скачивает необходимые модули в папку ```node_modules```, но делает это намного быстрее.

Далее, используя ```cmd``` в Windows или Терминал Linux/macOS, проделайте следующие шаги:

* скачайте сборку: ```git clone https://github.com/andreyalexeich/gulppack-pug.git```;
* установите ```gulp``` глобально: ```yarn global add gulp-cli```;
* перейдите в скачанную папку со сборкой: ```cd gulppack-pug```;
* введите команду, которая скачает необходимые компоненты для корректной работы нашей сборки, указанные в файле ```package.json```: ```yarn```;
* введите последнюю команду: ```gulp```.

![](https://i.imgur.com/iOYGCoG.png)

Если вы всё сделали правильно, у вас должен открыться браузер с локальным сервером и работающим browser-sync. Теперь если вы внесёте изменения в файлы ```.pug```, ```.scss```, ```.js```, браузер сам перезагрузит веб-страницу, а Gulp заново соберёт ваш проект в папке ```dest```.

## Bower?
Вместо [Bower](https://bower.io/) используйте yarn. Например, вам нужен [jQuery](https://jquery.com/) (уже используется в сборке в качестве примера), введите команду: ```yarn add jquery```, затем соберите: ```gulp vendor``` и запустите: ```gulp```. Вам остаётся подключить данную библиотеку в ваш ```.pug```.

***

# Gulppack. Pug + SCSS version

Gulppack is a very useful gulp build for your front-end projects. Compile SCSS and Pug, compress the files, optimize the pictures, write ES6. It reloads your browser automatically every time you save a file in a code editor. Don't care about tedious things, leave it to us!

## What includes:
* [browser-sync](https://browsersync.io/docs/gulp) - live reloading your web page. Browsersync makes your browser testing workflow faster by synchronising URLs, interactions and code changes across multiple devices;
* [gulp-autoprefixer](https://www.npmjs.com/package/gulp-autoprefixer) - parsing CSS and add vendor prefixes to rules by [Can I Use](https://caniuse.com/);
* [gulp-babel](https://www.npmjs.com/package/gulp-babel) - use next generation JavaScript with [Babel](https://babeljs.io/);
* [gulp-uglify](https://www.npmjs.com/package/gulp-uglify) - minifing JS files;
* [gulp-concat](https://www.npmjs.com/package/gulp-concat) - concatenates files;
* [gulp-pug](https://www.npmjs.com/package/gulp-pug) — compiling Pug to HTML;
* [gulp-sass](https://www.npmjs.com/package/gulp-sass) - compiling SCSS to CSS;
* [gulp-clean-css](https://www.npmjs.com/package/gulp-clean-css) - minifing CSS files;
* [gulp-sourcemaps](https://www.npmjs.com/package/gulp-sourcemaps) - generating the sourcemaps;
* [gulp-rename](https://www.npmjs.com/package/gulp-rename) - renaming files, adding prefix, suffix;
* [gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin) - minify PNG, JPEG, GIF and SVG images;
* [imagemin-pngquant](https://www.npmjs.com/package/imagemin-pngquant) - pngquant imagemin plugin;
* [imagemin-jpeg-recompress](https://www.npmjs.com/package/imagemin-jpeg-recompress) - jpeg-recompress imagemin plugin;
* [gulp-favicons](https://github.com/evilebottnawi/favicons) - favicons generator for your projects;
* [gulp-iconfont](https://www.npmjs.com/package/gulp-iconfont) — generate iconic fonts from your SVG;
* [gulp-iconfont-css](https://www.npmjs.com/package/gulp-iconfont-css) — generate styles for your iconic fonts;
* [gulp-svg-sprites](https://www.npmjs.com/package/gulp-svg-sprites) — create SVG sprites;
* [gulp-replace](https://www.npmjs.com/package/gulp-replace) - a string replace plugin for gulp;
* [gulp-newer](https://www.npmjs.com/package/gulp-newer) - piping the source files to newer before imagemin ensures that only those images that have changed are minified;
* [gulp-plumber](https://www.npmjs.com/package/gulp-plumber) - notifications in your terminal (SCSS/Sass errors for example);
* [gulp-debug](https://www.npmjs.com/package/gulp-debug) - debug Vinyl file streams to see what files are run through your Gulp pipeline;
* [gulp-watch](https://www.npmjs.com/package/gulp-watch) - file watcher;
* [gulp-clean](https://www.npmjs.com/package/gulp-clean) — removes files and folders.

## How to use:
* Install [Yarn](https://yarnpkg.com/en/docs/install).

> Yarn is a modern alternative to npm. Yarn works with the same ```package file.json``` and just downloads the required modules into the folder ```node_modules```, but does it much faster.

Then using ```cmd``` in Windows or Terminal in Linux/macOS, please do the following:

* clone the repository: ```git clone https://github.com/andreyalexeich/gulppack-pug.git```;
* install ```gulp``` globally: ```yarn global add gulp-cli```;
* go to the folder: ```cd gulppack-pug```;
* enter the command that downloads the required components: ```yarn```;
* run Gulp: ```gulp```.

![](https://i.imgur.com/iOYGCoG.png)

Your web browser will open with local server and running browser-sync. Now if you make changes to the
files ```.pug```, ```.scss``` or ```.js```, your web browser will reload the web page itself, and Gulp
will re-build your project in the ```dest``` folder.

## Bower?
Use yarn instead of [Bower](https://bower.io/). For example, you are need in [jQuery](https://jquery.com/) (already used in this project as an example), then using ```cmd``` in Windows or Terminal in Linux/macOS install it: ```yarn add jquery```, build it: ```gulp vendor``` and run: ```gulp```. All you have to do is connect this library to your ```.pug```.
