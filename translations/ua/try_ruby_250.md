---
lang:   UA
title:  Ще кілька простих відгуків
answer: [3-9]
load:   books = {"Фарбований лис" => :splendid}
ok:     Бачиш, метод length працює з рядками, списками і словниками.
error:
---

Продовжуй, заповни хеш відгуками. А якщо хочеш побачити весь список, просто набери: puts books

Знову ж, можливі оцінки: :splendid, :quite_good, :mediocre, :quite_not_good і :abysmal.

Ці оцінки не є рядками. Коли ти ставиш двокрапку перед простим словом, ти отримуєш __символ (Symbol)__. Символ є дешевшим за рядок (з точки зору комп'ютерної пам'яті). Тож якщо використовуєш слово знову і знову в своїй програмі, використовуй символ. Замість того, щоб мати тисячі копій цього слова в пам'яті, Ruby буде зберігати символ тільки __один раз__.

Що важливіше, символ каже нам, що це не просто якесь слово, а таке, що має значення у нашій програмі.

>Примітка перекладача: в англійській мові є два слова: Symbol і Char, і обидва перекладаються українською як "символ".
>В контексті Ruby Symbol правильно було б перекласти як "ідентифікатор", але використовують слово символ.
>Тому якщо в контексті Ruby ти почуєш "символ", то швидше за все це Symbol, ідентифікатор, який записується як :good, і є оптимізованим для пам'яті рядком.

Введи ще 2 відгуки, використовуй books.length, щоб дізнатися, скільки відгуків в словнику:

    books["Сутінки. Сага."] = :abysmal
    books["Фарбований Лис"] = :mediocre

    puts books

    puts books.length
