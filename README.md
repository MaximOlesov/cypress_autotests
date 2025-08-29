<h2>UI Автотесты на фреймворке Cypress</h2>

> **Статус проекта:**
> Публичный проект: https://login.qa.studio/
> 
> 🟢 Поддерживается (активный) 

## Описание проекта и задачи
Автоматизировать часть проверок регресса с помощью Cypress

## Тест-кейсы, которые автоматизировали
* Авторизация с верным паролем и верным логином
* Авторизация c верным логином и неверным паролем
* Авторизация c неверным логином и верным паролем
* Проверка работы валиадации на наличие @ в логине
* Проверка флоу восстановления пароля
* Проверка строчные буквы

## Детали реализации

1. baseUrl вынесен в переменные конфига
![image](https://raw.githubusercontent.com/MaximOlesov/cypress_autotests/refs/heads/main/cypress/screenshots/baseUrl.png)

2. Применение хуков beforeEach и afterEach
![image](https://raw.githubusercontent.com/MaximOlesov/cypress_autotests/refs/heads/main/cypress/screenshots/hooks.png)

3. Переменные данные для авторизации вынесены в отдельный файл
![image](https://raw.githubusercontent.com/MaximOlesov/cypress_autotests/refs/heads/main/cypress/screenshots/user_data.png)

4. Каждая страница описана в формате объекта с локаторами
![image](https://raw.githubusercontent.com/MaximOlesov/cypress_autotests/refs/heads/main/cypress/screenshots/locators.png)

## Локальный запуск через Cypress UI
1. Скачать проект и открыть в терминале.
2. Перейти в директорию проекта.
3. В терминале в папке с проектом запустить npm `install --save-dev cypress@12.7.0`
4. В терминале в папке с проектом запустить npm `npm i`
5. В терминале в папке с проектом запустить npm `npx cypress open`
6. Выбрать в Cypress UI E2E тестирование и браузер Google Chrome
7. Выбрать спеку my_autotest

Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://raw.githubusercontent.com/MaximOlesov/cypress_autotests/refs/heads/main/cypress/screenshots/my_autotest.cy.js/my_autotest.png)

## Локальный запуск тестов из терминала
1. Скачать проект
2. Перейти в терминале в директорию проекта
2. Выполнить команду:
```
npx cypress run --spec cypress/e2e/my_autotest.cy.js --browser chrome
```


**👤 Автор:**

Максим Олесов ([@Mxwave](https://t.me/Mxwave))

<p align="left">
  <img src="https://img.shields.io/badge/Made%20by-Maxim%20Olesov-blue?style=for-the-badge&logo=github" alt="Made by Maxim Olesov" />
</p>
