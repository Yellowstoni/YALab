## Задание первое
 1. Определите первый HTTPS-запрос, отправленный к домену ylab.io. </br> В ответе укажите стартовую строку данного запроса.

 2. У вкладки “О компании” (https://drive.google.com/file/d/1fSPgT9usn6gEBGcQcnKaBlcWuJkBI-88/view?usp=sharing) </br> определите цвет используемого шрифта. В ответе укажите его в формате r,g,b.

Ответ:   

 1.1  
 Я очень много времени потратила на размышление казалось бы простого задания, и пришла к выводу,   
 что https запрос не имеет стартовой строки. Https запрос представляет из себя соединение   
 клиент-сервер с верификации сертифката SSL. Т.е. клиент с сервером   
 обмениваются специальными сообщениями по TLS/SSL протоколу "тройным рукоможатием",  
 и после, сайт и браузер генерируют уникальный ключ шифрования данных.     

 Далее, мы уже можем по методу GET совершить HTTP запрос на документ html   
 из которого подтянуться стили, и другие файлы необходимые для рендеринга DOM сайта.  
А выглядеть первый HTTP запрос будет так:   
`GET https://ylab.io/ HTTP/1.1`   
`Host: ylab.io`

 2.1 `rgb(10, 184, 182)` 

## Задание второе 
 Определить для API https://api.nasa.gov/planetary/apod следующие данные:

 1. Минимально возможное валидное значение параметра date. </br> Ответ в формате YYYY-MM-DD.

 2. Укажите количество записей, возвращаемых в ответе на запрос к указанному API, </br> за период, начало которого - это ответ из пункта 1 данной задачи, а конец - 16 июня 1996 года.

 1.1 `1995-06-16 - минимальное возможное валидное значение`   
 2.1 `Колличество = 364` 

>[!NOTE] 
> Путем пользовательской ошибки `400` был определен диапозон значений
<div>
  <img align='center' src='img.png' width='650x'>
</div>

>[!NOTE] 
> Через скрипт было подсчитано кол-во записей
<div>
  <img align='center' src='img_1.png' width='550'>
</div>



## Задание третье 

Вопрос: К какому виду идентификаторов ресурсов в сети относится https://www.yandex.ru/search/?text=test

Ответ: `URI — имя и адрес ресурса в сети, включает в себя URL и URN;`

## Задание четвертое 
Вопрос: Верно ли утверждение, что структура HTTP-запроса равна структуре HTTP-ответа?

Ответ: `Верно, структура запроса/ответа похожа, но различие кроется в стартовой строке, где в запросе вводится метод и URI, а в ответе — код состояния и пояснение.` 


## Задание пятое 
Вопрос:
Должен ли http-ответ содержать заголовок Host?

Ответ: `Нет. Заголовок host относится к http-запросу как обязательный c версии http 1.1 `

