# Гайд по деплою бота на сервер

в данном гайде мы будем использовать [TimeWeb>cloud](https://timeweb.cloud)

## 1 Шаг (Регистрация)
регистрируемся на сайте и используем любой выгодный промокод
## 2 Шаг (Панель управления)
нажимаем на свой аккаунт -> выбираем "Панель управления"
нажимаем создать -> облачный сервер
## 3 Шаг (Создание сервера)
1. в образах выбираем Ubuntu версии 22.04 (или какую вы хотите)
![изображение](https://github.com/user-attachments/assets/7001b9a3-e4e3-4aac-b090-c42705ac5457)


2. регион выбираем ближайщий к вам и лучший

![изображение](https://github.com/user-attachments/assets/0ac68638-37a1-4cab-9534-bd16add09395)

4. конфигурация для легких ботов подойдет Premium NVMe
   
![изображение](https://github.com/user-attachments/assets/1b7509ea-c7a4-446c-8ff0-99149de9fae3)


6. сеть

![изображение](https://github.com/user-attachments/assets/5618db56-e9e7-40b1-920f-c37106e11147)

7. дополнительные услуги пропускаем, либо выбираем что нужно вам

8. авторизация также на ваше усмотрение

9. заказываем сервер

## 4 Шаг (НАстройка сервера)

после того как вы купили ваш сервер у вас откроеться данное окно

![изображение](https://github.com/user-attachments/assets/f3fe40f3-9152-4711-8aff-6d26cfa10370)

1. перед тем как продолжить нам понадобиться [FileZila](https://filezilla-project.org/)

![изображение](https://github.com/user-attachments/assets/496c45ba-87a0-424f-8807-9b15e01ce722)


3. дальше заходим в Windows PowerShell

4. вставляем SSH

![изображение](https://github.com/user-attachments/assets/26624f1f-6694-477c-bd4d-23d6cc993610)

5. отвечаем: yes

6. вводим пароль (root, он чуть ниже SSH)

7. создаем папку

![изображение](https://github.com/user-attachments/assets/9700e1fc-ba28-4b54-b099-8cfb2ea3e668)

8. заходим в директорию bots (cd bots) и в ней создаем deploy_bot

![изображение](https://github.com/user-attachments/assets/ca31f399-bc3c-42e2-984c-039a7dbeb54a)

9. ДОПИШУ ЗАВТРА
