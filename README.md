# Sport part of the scholarship backend project #

### Описание функционала сервиса ###

Сервис принимает данные от пользователя, связанные с его спортивными достижениями в формате json и вносит в базу данных заявок. Информация обрабатывается в соответсвие с пунктами из Приложения5 и вносится в соответствующие базы данных. Связь между базами будет осуществляться через присвоение уникального id каждому пользователю во внутренней архитектуре сервиса. После этого заявка становится в статус "неподтвержденной" (скорее всего для этого будет создана бд с полями: id, фио, статус заявки) до проверки и выставления баллов за все достижения ответственными лицами. После прохождения всех проверок и выставления баллов заявка принимает статсу "подтверждена", по id со всех бд стаскиваются данные для генерации нужного пакета документов.

### Используемые технологии 

* Django REST 
* PostgreSQL
