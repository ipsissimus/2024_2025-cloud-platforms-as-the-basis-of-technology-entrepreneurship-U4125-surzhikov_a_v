University: [ITMO University](https://itmo.ru/ru/) 

Faculty: [FTMI](https://ftmi.itmo.ru) 

Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) 

Year: 2024/2025 

Group: U4125 

Author: Surzhikov Artyom Viktorovich

Lab: Lab1 

Date of create: 21.04.2025 

Date of finished: 22.04.2025



Для начала мы создали Storage Admin. После чего создали виртуальную машину с типом E2, которая стоила $3.44

После того как была создана ВМ-ка, я подключился к ней и выполнил команду *gcloud auth login* что было моей ошибкой, так как это перезаписало все права, которые я назначал этой машиине в панели управления.

В результате выполненные команды исполнялись от имени этого пользователя. Поэтому при выполнении команды по копированию 3 файлов из бакета я практически до самого конца получал успех

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab1/IMAGE%202025-04-22%2015:27:27.jpg?raw=true)

Выполняемые мной команды всегда исполнялись и я видел эти 3 файла в своей файловой системе

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab1/IMAGE%202025-04-22%2015:27:23.jpg?raw=true)

После того как я пересоздал новую машиину, на которой не было прописано моих прав корневого аккаунта и добавил их заново своей виртуалке, при попытке выполнить ту же команду на копирование файлов, я получал запрет, который говорит что с правами *Compute Viewer* я доступа к бакету не имел 

![](https://github.com/ipsissimus/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-surzhikov_a_v/blob/main/lab1/IMAGE%202025-04-22%2015:27:35.jpg?raw=true)

