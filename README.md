# Лабораторная работа 3

1. Первым делом клонируем нашу основную виртуальную машину и создаем две сети NAT c разными адресами. Первая имеет адрес ```10.0.2.0```, а вторая – ```10.0.3.0```.

   <img width="1460" alt="image" src="https://github.com/user-attachments/assets/71ec2226-5f66-4aed-8ed5-b287390f824d">
   
2. В настройках сети виртуальных машин выбираем пункт ```Сеть NAT``` и подключаем каждую машину к созданным нами ранее сетям. Первая виртаульная машина должна быть подключена к двум разным сетям одновременно, чтобы иметь доступ и ко второй, и к третьей. Вторую и третью машину подключаем только к одной сети.

   <img width="943" alt="image" src="https://github.com/user-attachments/assets/41426e39-1118-45e1-82a5-86f481177113">

   <img width="941" alt="image" src="https://github.com/user-attachments/assets/21e836bf-75f4-4a3f-8f34-9c163497ec1e">

   <img width="942" alt="image" src="https://github.com/user-attachments/assets/5b349216-2252-4915-98af-b6e54008ef3c">

   <img width="940" alt="image" src="https://github.com/user-attachments/assets/70b71e97-1bad-45bc-8fbf-a1f948e66af3">
   
4. Запускаем виртуальные машины. Вводим команду ```ifconfig```, чтобы узнать ip-адреса.

   ![telegram-cloud-document-2-5247074039859535757](https://github.com/user-attachments/assets/8b6c5c8c-829e-47b0-8aba-322d9e84dec4)

   ![telegram-cloud-document-2-5247074039859535759](https://github.com/user-attachments/assets/1c6ee6d2-e647-44b1-ae84-f8197158f8ea)

   ![telegram-cloud-document-2-5247074039859535760](https://github.com/user-attachments/assets/ad5534cb-bd81-449f-91b8-f923448919d7)

   Как можно увидеть, первая машина имеет два адреса, ```10.0.2.4``` и ```10.0.3.5```. Вторая имеет адрес ```10.0.2.15```, а третья – ```10.0.3.4```.
   

6. Проверяем доступ в Интернет на всех машинах с помощью команды ```ping 8.8.8.8```.

   ![telegram-cloud-document-2-5247074039859535764](https://github.com/user-attachments/assets/ad67f9bc-9338-4ad7-b160-c5c28b464852)

   ![telegram-cloud-document-2-5247074039859535766](https://github.com/user-attachments/assets/f27187ac-82ce-44a6-a23c-20d17ef4a1cd)

   ![telegram-cloud-document-2-5247074039859535769](https://github.com/user-attachments/assets/b3e80802-50e4-43cd-a4d3-0327876758c3)

   Все машины имеют доступ в Интернет.


7. Проверяем, существует ли связь между машинами с помощью команды ```ping <ip-adress>```.

   ![telegram-cloud-document-2-5247074039859535790](https://github.com/user-attachments/assets/fd1ee9ff-668d-4d7d-a6e2-d202e03fbf8d)

   На скриншоте видно, что моя основная виртуальная машина имеет связь и со 2, и с 3 машиной. Так же как и 2, и 3 машины имеет связь с 1. А вот связи между 2 и 3 машиной нет – они находятся в разных подсетях. 





   




