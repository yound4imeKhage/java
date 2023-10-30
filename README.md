# java
Задача 1: Вывести сумму чисел от 1 до N.

function sumNumbersToN(N) {
    let sum = 0;
    for (let i = 1; i <= N; i++) {
        sum += i;
    }
    return sum;
}

Задача 2: Проверка на четность.

function isEven(number) {
    return number % 2 === 0;
}

Задача 3: Реверс строки.

function reverseString(str) {
    return str.split('').reverse().join('');
}

Задача 4: Поиск максимального числа в массиве.

function findMaxNumber(arr) {
    return Math.max(...arr);
}

Задача 5: Подсчет количества гласных в строке.

function countVowels(str) {
    const vowels = 'AEIOUaeiou';
    let count = 0;
    for (let char of str) {
        if (vowels.includes(char)) {
            count++;
        }
    }
    return count;
}

Задача 6: Проверка на палиндром.

function isPalindrome(str) {
    str = str.toLowerCase().replace(/[^a-zA-Z0-9]/g, '');
    const reversed = str.split('').reverse().join('');
    return str === reversed;
}

Задача 7: Генерация случайного числа в диапазоне.

function getRandomNumber(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}
Задача 8: Поиск дубликатов в массиве.

function findUniqueElements(arr) {
    return Array.from(new Set(arr));
}

Задача 9: Разделение строки на слова.

function splitStringIntoWords(str) {
    return str.split(' ');
}

Задача 10: Проверка на простое число.

function isPrime(number) {
    if (number <= 1) return false;
    if (number <= 3) return true;
    if (number % 2 === 0 || number % 3 === 0) return false;
    for (let i = 5; i * i <= number; i += 6) {
        if (number % i === 0 || number % (i + 2) === 0) return false;
    }
    return true;
}

Задача 11: Подсчет суммы цифр числа.

function sumOfDigits(number) {
    let sum = 0;
    while (number > 0) {
        sum += number % 10;
        number = Math.floor(number / 10);
    }
    return sum;
}

Задача 12: Поиск наибольшего общего делителя (НОД).

function findGCD(a, b) {
    while (b !== 0) {
        let temp = b;
        b = a % b;
        a = temp;
    }
    return a;
}

Задача 13: Генерация массива чисел от M до N.

function generateRangeArray(M, N) {
    const result = [];
    for (let i = M; i <= N; i++) {
        result.push(i);
    }
    return result;
}

Задача 14: Поиск индекса элемента в массиве.

function findElementIndex(arr, element) {
    return arr.indexOf(element);
}

Задача 15: Объединение двух массивов.

function mergeArrays(arr1, arr2) {
    return arr1.concat(arr2);
}

Задача 16: Проверка на анаграмму.

function areAnagrams(str1, str2) {
    return str1.split('').sort().join('') === str2.split('').sort().join('');
}

Задача 17: Возведение числа в степень.

function power(base, exponent) {
    return Math.pow(base, exponent);
}

Задача 18: Факториал числа.

function factorial(number) {
    if (number === 0 || number === 1) {
        return 1;
    }
    return number * factorial(number - 1);
}

Задача 19: Переворот массива.

function reverseArray(arr) {
    return arr.slice().reverse();
}

Задача 20: Вычисление среднего значения массива.

function calculateAverage(arr) {
    const sum = arr.reduce((acc, curr) => acc + curr, 0);
    return sum / arr.length;
}
