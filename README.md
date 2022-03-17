# qaguru-11-tda-hw-10

Welcome to the qaguru-11-tda-hw-10!  
  
Урок 10 Первая сборка в Jenkins:  
master  
Job -> c11-lifetesting-unit10-hw-jenkins-demoqa  
  
Урок 11 параметризованные сборки:  
branch -> "hw11"  
Job -> https://jenkins.autotests.cloud/job/c11-lifetesting-unit11-hw/  
  
Урок 12 отправка уведомлений:  
branch -> "hw12-notification-telegram-bot"  
Job -> https://jenkins.autotests.cloud/job/c11-lifetesting-unit12-hw/  


---
Параметры сборок для уроков 11 и 12

BRANCH - ветка для запуска тестов, назначение ветки выше в описании

ENVIRONMENT - в данном случае просто пример параметра, который указывает на какой среде выполнялись тесты (подтягивается в нотификашку в телеграм)

TASK - запуск тестов в зависимости от тега
- существующие теги:
  - test - запускает все тесты из репо
  - smoke-test - запускает один тест с минимальным заполнением полей для успешного прохождения теста (сделан для проверки отработки тега в рамках урока 11)
  - success-test - запускает все успешные тесты из repo, сделан чтобы разделить поток нотификашек в телеграм (все отчеты шлются в личный и общий чат, успешные отчеты шлются только в личку, чтобы снизить нагрузку на общий чат)
  
REMOTE_BROWSER
REMOTE_BROWSER_USER (нет значения по-умолчанию)
REMOTE_BROWSER_PASSWORD (нет значения по-умолчанию)
Переменные в рамках 11 урока для запуска удаленного браузера selenoid

COMMENT - любой коммент касательно сборки

BROWSER - браузер, в котором будут проводиться тесты

BROWSER_SIZE - разрешение браузера

First_Name - Имя студента, которая заполнится в карточке студента тесте

Last_Name - Фамилия студента, которая заполнится в карточке студента тесте
