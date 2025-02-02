# Гайд по деплою бота на сервер

В этом гайде мы будем использовать TimeWeb Cloud timeweb.cloud (https://timeweb.cloud/).

## Шаг 1 Регистрация

1. Регистрируемся на сайте и используем любой выгодный промокод.

## Шаг 2 Панель управления

1. Нажимаем на свой аккаунт.
2. Выбираем "Панель управления".
3. Нажимаем "Создать" и выбираем "Облачный сервер".

## Шаг 3 Создание сервера

### Выбор образа

Выбираем образ Ubuntu версии 22.04 или другую подходящую для вас.

![изображение](https://github.com/user-attachments/assets/7001b9a3-e4e3-4aac-b090-c42705ac5457)

### Выбор региона

Выбираем регион, ближайший к вам и наиболее подходящий.

![изображение](https://github.com/user-attachments/assets/0ac68638-37a1-4cab-9534-bd16add09395)

### Конфигурация

Для легких ботов подойдет конфигурация Premium NVMe.

![изображение](https://github.com/user-attachments/assets/1b7509ea-c7a4-446c-8ff0-99149de9fae3)

### Сеть

![изображение](https://github.com/user-attachments/assets/5618db56-e9e7-40b1-920f-c37106e11147)

### Дополнительные услуги

Пропускаем или выбираем необходимые вам услуги.

### Авторизация

Авторизация на ваше усмотрение.

### Заказ сервера

Заказываем сервер.

## Шаг 4 Настройка сервера

После того как вы купили сервер, у вас откроется следующее окно:

![изображение](https://github.com/user-attachments/assets/f3fe40f3-9152-4711-8aff-6d26cfa10370)

### Установка FileZilla

Перед тем как продолжить, скачайте и установите FileZilla filezilla-project.org (https://filezilla-project.org/).

![изображение](https://github.com/user-attachments/assets/496c45ba-87a0-424f-8807-9b15e01ce722)

### Подключение через PowerShell

1. Откройте Windows PowerShell.
2. Вставьте SSH-команду, предоставленную в окне управления сервером.

![изображение](https://github.com/user-attachments/assets/26624f1f-6694-477c-bd4d-23d6cc993610)

3. Ответьте "yes" на запрос.
4. Введите пароль (root, он указан ниже SSH).

### Создание папки

1. Создайте папку bots.

![изображение](https://github.com/user-attachments/assets/9700e1fc-ba28-4b54-b099-8cfb2ea3e668)

### Переход в директорию

1. Перейдите в директорию bots:

cd bots


2. Создайте папку deploy_bot.

![Создание директории deploybot](https://github.com/user-attachments/assets/ca31f399-bc3c-42e2-984c-039a7dbeb54a)

3. Перейдите в директорию deploy_bot и создайте виртуальное окружение.

![Создание виртуального окружения](https://github.com/user-attachments/assets/3dbe237a-d740-4d40-a4b3-06307337b0b8)

4. Выполняем команду для активации venv.

![Активация venv](https://github.com/user-attachments/assets/a7f8cf45-4c73-4760-bbf0-a9a08db71f3c)

5. Устанавливаем зависимости, необходимые для вашего проекта.

![Установка зависимостей](https://github.com/user-attachments/assets/f065e790-5daf-464e-93c3-6c1f0d77ed01)

## Шаг 5 Заливаем файлы на сервер

1. Открываем **FileZilla**.

2. Вводим данные для подключения к серверу (Хост, имя пользователя, пароль, порт (22)).

![Подключение через FileZilla](https://github.com/user-attachments/assets/c7f96b2e-6921-461f-863a-a8418f3bc84e)

3. Жмем на "Быстрое соединение".

4. Переходим в **bots -> deploy_bot.

![изображение](https://github.com/user-attachments/assets/4dad92f5-e0c5-48dc-b51b-415f8d077b7e)

5. Копируем ваши файлы и вставляем в окно.
![изображение](https://github.com/user-attachments/assets/cef000fb-5d9b-489b-8568-b134a767c92f)

## Шаг 6 Запуск сервера (бота)

1. Возвращаемся в консоль.

2. Переходим в корень и пишем команду:

screen -S deploy_bot

![изображение](https://github.com/user-attachments/assets/a78c507d-3e20-4f67-95ed-6a8a4fa479e6)

3. Заходим в директорию бота.

4. Активируем venv.

5. Запускаем бота.

![изображение](https://github.com/user-attachments/assets/735fcb56-2f93-420c-a5eb-f0a5059bebf5)

Теперь ваш бот работает на сервере! Если возникнут вопросы, не стесняйтесь их задавать.

