# Геометрические фигуры

Источник: видео "Геометрические фигуры на HTML и CSS // Треугольник стрелка круг трапеция и другие" 
https://vk.com/im/convo/19460369?entrypoint=list_all&z=video-125918837_456239144%2Fcb0fe0d085da504841

1. создаем создаем файлы index.html, style.css (в папке css) в папке проекта.

2. в файле index.html готовим шаблон

```html
<!-- Сообщаем браузеру, как стоит обрабатывать эту страницу -->
<!DOCTYPE html>
<!-- Оболочка документа, указываем язык содержимого -->
<html lang="ru">
<!-- Заголовок страницы, контейнер для других важных данных (не отображается) -->
<head>
    <!-- Заголовок страницы в браузере -->
    <title></title>
    <!-- Подключаем CSS -->
    <link rel="stylesheet" href="css/style.css">
    <!-- Кодировка страницы -->
    <meta charset="utf-8">
    <!-- Адаптив -->
    <meta name="viewport" content="width=device-width">
</head>
<!-- Отображаемое тело страницы -->
<body>
<!-- Оболочка для демонстрации -->
<div class="wrapper">
    <!-- Контент -->
   
</div>
</body>
</html>
```

3. в файле style.css вставляем шаблон

```css
/* Обнуление */
*,*:before,*:after{
    padding: 0;
    margin: 0;
    border: 0;
    box-sizing: border-box;
}
/* Стили для демонстрации */
html,body{
    height: 100%;
}
.wrapper{

}
/* Основные стили */
```

4. в файле index.html в head указываем название проекта

```html
<title>Геометрические фигуры</title>
```

5. в файле index.html в body указываем div с геометрическими фигурами

```html
<div class="block">
   <div class="block_item">
      <div class="square"></div>
   </div>
   <div class="block_item">
      <div class="rectangle"></div>
   </div>
   <div class="block_item">
      <div class="circle"></div>
   </div>
   <div class="block_item">
      <div class="oval"></div>
   </div>
   <div class="block_item">
      <div class="triangle-up"></div>
   </div>
   <div class="block_item">
      <div class="triangle-down"></div>
   </div>
   <div class="block_item">
      <div class="triangle-left"></div>
   </div>
   <div class="block_item">
      <div class="triangle-right"></div>
   </div>
   <div class="block_item">
      <div class="parallelogram"></div>
   </div>
   <div class="block_item">
      <div class="trapezoid"></div>
   </div>
</div>
```

6. в файле style.css добавляем в стили для демонстрации

```css
.block{
   padding: 50px;
   max-width: 1170px;
   margin: 0 auto;
}
.block_item{
   margin: 0 0 30px 0;
}
```

7. в файле style.css добавляем классы из html

```css
.square{}
.rectangle{}
.circle{}
.oval{}
.triangle-up{}
.triangle-down{}
.triangle-left{}
.triangle-right{}
.parallelogram{}
.trapezoid{}
```

8. в файле style.css расписываем стили фигур

```css
.square{ /* Квадрат */
   width: 150px;
   height: 150px;
   background-color: green;
}
.rectangle{ /* Прямоугольник */
   width: 300px;
   height: 150px;
   background-color: green;
}
.circle{ /* Круг - квадрат с закругленными краями */
   width: 150px;
   height: 150px;
   background-color: green;
   border-radius: 50%;
}
.oval{ /* Овал - прямоугольник с закругленными краями */
   width: 300px;
   height: 150px;
   background-color: green;
   border-radius: 50%;
}
.triangle-up{
   width: 0;
   height: 0;
   border-left: 50px solid transparent; /* transparent - прозрачный цвет */
   border-right: 50px solid transparent;
   border-bottom: 100px solid green;
}
.triangle-down{
   width: 0;
   height: 0;
   border-left: 50px solid transparent; /* transparent - прозрачный цвет */
   border-right: 50px solid transparent;
   border-top: 100px solid green;
}
.triangle-left{
   width: 0;
   height: 0;
   border-top: 50px solid transparent; /* transparent - прозрачный цвет */
   border-bottom: 50px solid transparent;
   border-right: 100px solid green;
}
.triangle-right{
   width: 0;
   height: 0;
   border-top: 50px solid transparent; /* transparent - прозрачный цвет */
   border-bottom: 50px solid transparent;
   border-left: 100px solid green;
}
.parallelogram{
   width: 200px;
   height: 100px;
   background-color: green;
   transform: skew(15deg);
}
.trapezoid{
   width: 200px;
   border-bottom: 100px solid green;
   border-left: 30px solid transparent;
   border-right: 30px solid transparent;
}
```

9. в файле style.css если хотим менять цвет фигуры при наведении курсора - hover

```css
.square{ /* Квадрат */
   width: 150px;
   height: 150px;
   background-color: green;
}
.square:hover{
   background-color: red;
}
```

# Итог

1. в файле index.html

```html
<!-- Сообщаем браузеру, как стоит обрабатывать эту страницу -->
<!DOCTYPE html>
<!-- Оболочка документа, указываем язык содержимого -->
<html lang="ru">
<!-- Заголовок страницы, контейнер для других важных данных (не отображается) -->
<head>
   <!-- Заголовок страницы в браузере -->
   <title>Геометрические фигуры</title>
   <!-- Подключаем CSS -->
   <link rel="stylesheet" href="css/style.css">
   <!-- Кодировка страницы -->
   <meta charset="utf-8">
   <!-- Адаптив -->
   <meta name="viewport" content="width=device-width">
</head>
<!-- Отображаемое тело страницы -->
<body>
<!-- Оболочка для демонстрации -->
<div class="wrapper">
   <!-- Контент -->
   <div class="block">
      <div class="block_item">
         <div class="square"></div>
      </div>
      <div class="block_item">
         <div class="rectangle"></div>
      </div>
      <div class="block_item">
         <div class="circle"></div>
      </div>
      <div class="block_item">
         <div class="oval"></div>
      </div>
      <div class="block_item">
         <div class="triangle-up"></div>
      </div>
      <div class="block_item">
         <div class="triangle-down"></div>
      </div>
      <div class="block_item">
         <div class="triangle-left"></div>
      </div>
      <div class="block_item">
         <div class="triangle-right"></div>
      </div>
      <div class="block_item">
         <div class="parallelogram"></div>
      </div>
      <div class="block_item">
         <div class="trapezoid"></div>
      </div>
   </div>
</div>
</body>
</html>
```

2. в файле style.css 

```css
/* Обнуление */
*,*:before,*:after{
   padding: 0;
   margin: 0;
   border: 0;
   box-sizing: border-box;
}
/* Стили для демонстрации */
html,body{
   height: 100%;
}
.wrapper{

}
.block{
   padding: 50px;
   max-width: 1170px;
   margin: 0 auto;
}
.block_item{
   margin: 0 0 30px 0;
}

/* Основные стили */

.square{ /* Квадрат */
   width: 150px;
   height: 150px;
   background-color: green;
}
.square:hover{
   background-color: red;
}

.rectangle{ /* Прямоугольник */
   width: 300px;
   height: 150px;
   background-color: green;
}
.circle{ /* Круг - квадрат с закругленными краями */
   width: 150px;
   height: 150px;
   background-color: green;
   border-radius: 50%;
}
.oval{ /* Овал - прямоугольник с закругленными краями */
   width: 300px;
   height: 150px;
   background-color: green;
   border-radius: 50%;
}
.triangle-up{
   width: 0;
   height: 0;
   border-left: 50px solid transparent; /* transparent - прозрачный цвет */
   border-right: 50px solid transparent;
   border-bottom: 100px solid green;
}
.triangle-down{
   width: 0;
   height: 0;
   border-left: 50px solid transparent; /* transparent - прозрачный цвет */
   border-right: 50px solid transparent;
   border-top: 100px solid green;
}
.triangle-left{
   width: 0;
   height: 0;
   border-top: 50px solid transparent; /* transparent - прозрачный цвет */
   border-bottom: 50px solid transparent;
   border-right: 100px solid green;
}
.triangle-right{
   width: 0;
   height: 0;
   border-top: 50px solid transparent; /* transparent - прозрачный цвет */
   border-bottom: 50px solid transparent;
   border-left: 100px solid green;
}
.parallelogram{
   width: 200px;
   height: 100px;
   background-color: green;
   transform: skew(15deg);
}
.trapezoid{
   width: 200px;
   border-bottom: 100px solid green;
   border-left: 30px solid transparent;
   border-right: 30px solid transparent;
}
```