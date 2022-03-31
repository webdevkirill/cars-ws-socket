#Тестовое задание

Написать SPA-приложение для вывода списка автомобилей, которые приходят с сервера. Для запуска сервера использовать команду 
```bash
npm run server
```

Все зависимости указаны в файле package.json.

Сервер поднимается на порту 5001 по адресу http://localhost:5001/ и через WebSocket отправляет раз в 5 секунд информацию об автомобиле, а именно объект 

```javascript
{
    id: string,
    timestamp: Date,
    color: string,
    carClass: string, //класс авто - легковой, грузовой и т.д.
    plate: string, // номерной знак автомобиля
    speed: number
}
```
Более подробно описано в файле `./server/randomCar.js`

Выводить информацию любым образом. Весь визуал на ваше усмотрение, можно (и желательно) подключить фантазию. Использовать эмидзи, выводить номер авто картинкой и т.п.

Нужно добавить фильтры по цвету автомобиля, по скорости (от мин. до макс.) и по классу авто.

Желательно использовать Redux, TS. Приветствуется использование обычных React-flow библиотек (например роутер).

В качестве ответа скинуть ссылку на гит репозиторий, в README добавить команды для запуска приложения.