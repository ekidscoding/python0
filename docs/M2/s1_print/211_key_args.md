---
title: Ключові аргументи
---

# Функція `print()` - ключові аргументи
Python пропонує ще один механізм передачі аргументів, який допоможе, якщо ви хочете переконати функцію `print()` дещо змінити її поведінку.

Наразі ми не будемо пояснювати цю ідею детально. Ми зробимо це коли говоритимемо про функції. Зараз просто покажемо як це працює. Можете вільно користуватись цим у всіх ваших програмах.

Механізм називають **"ключові аргументи"**. Імʼя походить від того факту, що значення аргументу взяте **НЕ** від його порядкового номеру (позиції), а від спеціального слова (keyword), що використовують, щоб відрізняти аргументи.

Функція `print()` має 2 ключових аргументи, які можна використати у власних цілях. Перший з них має імʼя `end`.

В наступному блоці ви бачите найпростіший приклад використання ключового аргументу.

``` { .yaml .copy }
print("Мене звати", "Python.", end=" ")
print("Monty Python.")
```

Щоб користуватись ключовими аргументами,необхідно знати деякі правила:

1. ключовий аргумент складається з трьох частин:
    - ключового слова, що відрізняє аргумент (ключове слово `end` в нашому випадку);
    - знак присвоїти (`=`);
    - і значення, що присвоюється аргументові;
2. будь-які ключові аргументи мають вказуватись **після** останнього позиційного аргументу (це важливо)

В нашому прикладі ми скористались ключовим аргументом `end`, і встановили його як текст, що містить один пробіл.

Запустимо код, щоб побачити результат.

Консоль має відобразити наступний текст:

`Мене звати Python. Monty Python`.

Як можна бачити, ключове слово `end` визначає символи, які надсилає функція `print()` в консоль зразу після того, як досягне кінця останнього позиційного аргументу.

За замовчуванням, якщо не вказати інакше, ключовий аргумент `end` неявним чином встановлюється за нас: `end="\n"`.
