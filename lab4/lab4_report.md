University: [ITMO University](https://itmo.ru/ru/) 

Faculty: [FTMI](https://ftmi.itmo.ru) 

Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) 

Year: 2024/2025 

Group: U4125 

Author: Surzhikov Artyom Viktorovich

Lab: Lab4

Date of create: 22.04.2025 

Date of finished: 28.04.2025



Это схема реально существующего механизма по распознгаванию титульных листов ВПР работ в школах Санкт-Петербурга

Весь флоу представляет из себя такую цепочку действий

![image_2025-04-28_17-21-35](/Users/iwanbranwell/Downloads/image_2025-04-28_17-21-35.png)

Через существующий АПИ метод происходит запрос передающий в АПИ запросе файл, сконвертированный в base64. После чего вызывается модель mnist которая извлекает необходимые блоки и сопоставляет их с координатами, после чего сверяет их с существующими формами написания числовых значений. После этого происходит распознавание таблицы с баллами, а сформированный ответ в виде json отправляется обратно пользователю

![diagram-export-28.04.2025-17_19_28](/Users/iwanbranwell/Documents/ИТМО/Cloud-platforms/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/lab4/diagram-export-28.04.2025-17_19_28.png)
