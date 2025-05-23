University: [ITMO University](https://itmo.ru/ru/) 

Faculty: [FTMI](https://ftmi.itmo.ru) 

Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) 

Year: 2024/2025 

Group: U4125 

Author: Surzhikov Artyom Viktorovich

Lab: Lab2

Date of create: 22.04.2025 

Date of finished: 22.04.2025

Итак, что мы сделали тут? Мы задеплоили на мощностях Google контейнер, который был уже добавлен в библиотеку. С настройками указаннымии в документации. Указанный контейнер поднялся по умолчанию на 8080 порту по адресу https://hello-sa-demo-307056602443.us-central1.run.app/

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab2/Screenshot%20at%20Apr%2022%2021-19-13.png?raw=true)

Как видно выше задеплойенный контейнер с заранее подготовленным содержимым готов к использованию

После этого я запустиил пингии с моей машины командой ping `https://hello-sa-demo-307056602443.us-central1.run.app/` 

Это привело к тому что я начал генерировать запросы к URL-у на котором поднялся контейнер. 

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab2/Screenshot%20at%20Apr%2022%2021-20-42.png?raw=true)

После этого, я зашел в редактировать в настройки и поднял новую ревизию на новом порту `8090` это привело к тому что появился новый контейнер с тем же содержимым

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab2/Screenshot%20at%20Apr%2022%2021-20-11.png?raw=true)

А продолжающиеся пингии создали небольшую нагрузку

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab2/Screenshot%20at%20Apr%2022%2021-21-27.png?raw=true)

Таким образом появилась возможность распределять трафик между разными контейнерами поднятыми на разных портах

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab2/Screenshot%20at%20Apr%2022%2021-31-59.png?raw=true)

 

