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
* Проверка работы валиадации на наличие @ в логине
* Проверка флоу восстановления пароля

## Детали реализации

1. baseUrl вынесен в переменные конфига
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_16-52-00.png)

2. Применение хуков beforeEach и afterEach
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_16-54-41.png)

3. Переменные данные для авторизации вынесены в отдельный файл
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_16-55-49.png)

4. Каждая страница описана в формате объекта с локаторами
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_17-02-44.png)

## Локальный запуск тестов (из терминала)
1. Скачать проект
2. Перейти в терминале в директорию проекта
2. Выполнить команду:
```
npx cypress run --spec cypress/e2e/lesson_locators.cy.js --browser chrome
```
Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_17-02-44.png)


## Локальный запуск через Cypress UI
1. Скачать проект и открыть в терминале.
2. Перейти в директорию проекта.
3. В терминале в папке с проектом запустить npm `install --save-dev cypress@12.7.0`
4. В терминале в папке с проектом запустить npm `npm i`
5. В терминале в папке с проектом запустить npm `npx cypress open`
6. Выбрать в Cypress UI E2E тестирование и браузер Google Chrome
7. Выбрать спеку lesson_locators

Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://github.com/prettybetty023-debug/cypress_autotests/blob/main/2026-08-11_17-05-25.png)


## Автор

Елизавета Познышева ([@msdvibe](https://t.me/msdvibe))
