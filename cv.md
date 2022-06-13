### ALENA METENEVA

#### Contacts:
* **Discord:** nekirilova#1158
* **Telegram:** @nekirilova
* **email:** alenameteneva@gmail.com

#### About myself:
I am a junior QA, former accountant, mother of three childeren and I hope a future frontend developer. I spent 7 years taking care of my daughters, so ***I am highly motivated*** to become more than just a mother. I am very excited of working as QA, but I also found myself interested in HTML&CSS and JS.

#### Skills:
* HTML&CSS
* SQL
* JavaScript
* C#
* Postman, Charles Proxy
* DevTools
* REST API
* SWAGGER

#### Code example:
```
const puppeteer = require('puppeteer');

async function testYaRu(){
    console.log('Запуск браузера');
    const browser = await puppeteer.launch();
    
    console.log('Создание новой вкладки в браузере');
  const page = await browser.newPage();
    
    console.log('Переход на страницу ya.ru');
    await page.goto('https://ya.ru/');
    

    console.log('Ввод текста "Автоматизация тестирования" в поисковую строку');
    const searchField = await page.$('#text');
    await searchField.type('Автоматизация тестирования');
   
    console.log('Клик в кнопку "Найти"');
    const searchButton = await page.$('.button[type=submit]');
    await searchButton.click();
   
    
    console.log('Ожидание элемента с результатом');
    await page.waitForNavigation();
                               
    console.log('Получение строки с результатом');
    const result = await page.$('.serp-item');
    console.log('Проверка условия тест-кейса');
    if (!result) {
        console.log('Успех. Результаты найдены');
    }
    else {
        console.log('Ошибка');
    };

    console.log('Закрытие браузера');
    await browser.close();
   
}

testYaRu();
```

#### Experience:
I used to work as accountant in a bank.  And after 7 years of maternity leave I began working as a junior QA. 

#### Languages:
* Russian
* English (Upper-Intermediate, FCE)
* Chezh (C1)
* Dutch (A2)
* Italian (A2)
* A bit of chinese (HSK3)