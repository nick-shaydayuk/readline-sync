# Readline-sync practice

## Preparations
0. We believe you've reached 26-th lesson on hexlet - make sure you have.
1. Clone this repository
2. Open your terminal and enter THIS directory.
3. Run __npm init__ command and click enter several times.
4. You'll see some new files added to current working directory. So let us explore those: 
    1. "package.json - это файл, который используется в проектах на Node.js для описания зависимостей, скриптов и других метаданных проекта. Он содержит информацию о названии проекта, версии, авторе, лицензии, зависимостях и скриптах, которые можно запустить в проекте. Этот файл используется для управления зависимостями и сборки проекта, а также для обмена информацией о проекте между разработчиками."
    2. "package-lock.json - это файл, который создается автоматически при установке зависимостей в проекте на Node.js. Он содержит информацию о точных версиях всех установленных пакетов и их зависимостей. Это позволяет гарантировать, что проект будет работать стабильно на любой машине, где он будет установлен, так как все зависимости будут точно такими же, как и на машине разработчика. Этот файл должен быть добавлен в систему контроля версий, чтобы все участники проекта имели доступ к одинаковым версиям зависимостей."
5. Install the __readline-sync__ library via npm (node package manager). If you ran out of ideas how to do it, google this: "npm install something"
6. Create a new __index.js__ 
7. Insert following code into __index.js__:
    `const readlineSync = require('readline-sync');

    // Запрос имени пользователя
    const userName = readlineSync.question('Введите ваше имя: ');

    console.log(Привет, ${userName}! Добро пожаловать в мир Node.js и readline-sync.);`

8. For the next step, run your code in terminal aka CLI aka command line interface. Remember that "node fileName.js" command? You'll need this.
9. The result has to look like terminal asks your name, then you type it and then terminal greets you.
10. Alright mate, if you're finished, call teacher to check this out

## Some rules
So, for the following tasks the result is:

0. Don't forget to create a new file for each task
1. A function
2. The function does "return" something
3. At the end of the task you have to log to the console a call oh the function you just wrote
4. Always remember, that funcion gets its arguments from command line (terminal) and not from a standart variable 

### Задача №1: Калькулятор налога на доходы

Напишите функцию incomeTaxCalculator(income), которая принимает на вход сумму дохода и возвращает сумму налога на доходы. Пусть ставка налога составляет 15%.

### Задача №2: Конвертер температуры

Создайте функцию celsiusToFahrenheit(celsius), которая принимает температуру в градусах Цельсия и возвращает ее эквивалент в градусах Фаренгейта. Формула: (C * 9/5) + 32.

### Задача №3: Расчет скидки в магазине

Напишите функцию calculateDiscount(price, discountPercentage), которая принимает цену товара и процент скидки, а затем возвращает сумму с учетом скидки.

### Задача №4: Расчет периметра и площади прямоугольника

Создайте функцию calculateRectangleProperties(width, height), которая принимает ширину и высоту прямоугольника, а затем возвращает объект с его периметром и площадью.

### Задача №5: Расчет расстояния между двумя точками в 2D

Создайте функцию calculateDistance(x1, y1, x2, y2), которая принимает координаты двух точек в 2D пространстве и возвращает расстояние между ними.

### Задача №6: Расчет времени пути

Создайте функцию calculateTime(distance, speed), которая принимает расстояние и скорость (в км/ч), а затем возвращает время в пути в формате ХХч. ХХм. 

### Задача №7: Подсчет количества слов в строке

Напишите функцию countWords(sentence), которая принимает строку и возвращает количество слов в ней.

### Задача №8: Калькулятор расходов и доходов

Напишите функцию calculateBalance(incomes, expenses), которая принимает на вход две строки, содержащие перечьни доходов и расходов, а затем возвращает баланс (разницу между общим доходом и общими расходами).

### Задача №9: Расчет средней оценки

Создайте функцию calculateAverageGrade(grades), которая принимает строку со списком оценок и возвращает среднюю оценку. Оценки могут быть представлены числами от 1 до 10.

 
### Задача №10: Генератор случайных уравнений

Напишите функцию generateRandomEquation(), которая генерирует случайное уравнение вида ax + b = c, где a, b и c - случайные числа.

### Задача №11: Калькулятор бонусов сотрудника

Создайте функцию calculateEmployeeBonus(salary, performanceRating), которая принимает зарплату сотрудника и его рейтинг производительности, а затем возвращает бонус. Если рейтинг выше 8, бонус составляет 20% от зарплаты, в противном случае - 10%.

### Задача №12: Реверс строки с исключением слов

Напишите функцию reverseStringWithException(str, exception), которая принимает строку и слово-исключение, а затем возвращает строку с перевернутыми словами, за исключением слова-исключения. Например, для Hello World и исключения World результат должен быть World olleH.