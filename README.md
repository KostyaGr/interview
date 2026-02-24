
# Interview



Создать компонент <TreeView> для отображения иерархической структуры данных (например, файловая система или каталог магазина). 



Компонент должен поддерживать динамическое открытие-закрытие узлов дерева и поиск по содержимому с использованием фильтрации.



```typescript

const Node = {

 id: string,

 name: string,

 children?: Array<TreeNode>,

}

```



```javascript

const fetchBranchOne = () => new Promise( (resolve, reject) => {

 setTimeout( () => {

 resolve([{

 "id": "catalog",

 "name": "Каталог",

 "children": [{

 "id": "electronics",

 "name": "Электроника",

 "children": [{

 "id": "smartphones",

 "name": "Смартфоны",

 "children": [{

 "id": "iphone",

 "name": "iPhone"

 }, {

 "id": "android",

 "name": "Android"

 }]

 }, {

 "id": "computers",

 "name": "Компьютеры",

 "children": [{

 "id": "laptops",

 "name": "Ноутбуки"

 }, {

 "id": "desktops",

 "name": "Стационарные ПК"

 }]

 }, {

 "id": "accessories",

 "name": "Аксессуары",

 "children": [{

 "id": "headphones",

 "name": "Наушники"

 }, {

 "id": "chargers",

 "name": "Зарядные устройства"

 }]

 }]

 }, {

 "id": "clothing",

 "name": "Одежда",

 "children": [{

 "id": "men",

 "name": "Мужская одежда",

 "children": [{

 "id": "shirts",

 "name": "Рубашки"

 }, {

 "id": "pants",

 "name": "Брюки"

 }]

 }, {

 "id": "women",

 "name": "Женская одежда",

 "children": [{

 "id": "dresses",

 "name": "Платья"

 }, {

 "id": "skirts",

 "name": "Юбки"

 }]

 }, {

 "id": "kids",

 "name": "Детская одежда",

 "children": [{

 "id": "boys",

 "name": "Для мальчиков"

 }, {

 "id": "girls",

 "name": "Для девочек"

 }]

 }]

 }, {

 "id": "home_goods",

 "name": "Товары для дома",

 "children": [{

 "id": "furnitures",

 "name": "Мебель"

 }, {

 "id": "decorations",

 "name": "Украшения интерьера"

 }, {

 "id": "kitchenware",

 "name": "Посуда"

 }]

 }]

 }])

 }

 , Math.floor(Math.random() * (5000 - 1500 + 1)) + 1500)

}

)

```



```javascript

const fetchBranchTwo = () => new Promise( (resolve, reject) => {

 setTimeout( () => {

 resolve([{

 "id": "root",

 "name": "Корневая папка",

 "children": [{

 "id": "src",

 "name": "Источники",

 "children": [{

 "id": "components",

 "name": "Компоненты",

 "children": [{

 "id": "header",

 "name": "Хедер"

 }, {

 "id": "footer",

 "name": "Футер"

 }, {

 "id": "main",

 "name": "Главная"

 }]

 }, {

 "id": "pages",

 "name": "Страницы",

 "children": [{

 "id": "home",

 "name": "Домашняя страница"

 }, {

 "id": "about",

 "name": "О нас"

 }, {

 "id": "contact",

 "name": "Контакты"

 }]

 }, {

 "id": "styles",

 "name": "Стили",

 "children": [{

 "id": "global.css",

 "name": "Глобальные стили"

 }, {

 "id": "theme.css",

 "name": "Темные цвета"

 }]

 }]

 }, {

 "id": "assets",

 "name": "Активы",

 "children": [{

 "id": "icons",

 "name": "Иконки"

 }, {

 "id": "images",

 "name": "Изображения"

 }, {

 "id": "fonts",

 "name": "Шрифты"

 }]

 }, {

 "id": "config",

 "name": "Конфигурация",

 "children": [{

 "id": "env.js",

 "name": "Переменные окружения"

 }, {

 "id": "webpack.config.js",

 "name": "Конфиг Webpack"

 }]

 }]

 }])

 }

 , Math.floor(Math.random() * (5000 - 1500 + 1)) + 1500)

}

)

```

