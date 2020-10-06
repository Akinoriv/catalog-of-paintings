# Каталог
Верстка выполнена по методологии БЭМ, на Vue.Cli с использованием средства автоматизации webpack.

Конфигурация корректно работает на 12 версии Node.js.

Использовался только чистый css на scss.

Кнопка “купить” реализовывает следующий функционал:<br>
    По ее нажатию отправляется ajax запрос методом get по адресу https://jsonplaceholder.typicode.com/posts/1;<br>
    На время выполнения запроса вместо надписи “купить” появлятся лоадер;<br>
    После удачного запроса внешний вид кнопки менятет состояние: “в корзине”.<br>
   
После перезагрузки страницы состояния товаров сохраняется. Для запросов к серверу использовался axios. Реалезована поддержка IE11;

![catalog](https://user-images.githubusercontent.com/49586977/95232456-31eaca80-080d-11eb-850f-6986b5dc71c2.gif)

![vue](https://user-images.githubusercontent.com/49586977/95232502-416a1380-080d-11eb-9b09-b8836dbf6c20.gif)

Верстка по макету: https://www.figma.com/file/p5xYvZV5Vy9cZvWzkL7uk5/Redsoft-test?node-id=0%3A1 выполнена в PixelPerfect
