Перший рефакторинг:

    Опис проблеми:
        Вхідний код містить клас BasicCalculator, який реалізує лише базові операції додавання та віднімання. Завдання полягало в розширенні функціональності калькулятора шляхом додавання методів множення та ділення, використовуючи підхід зі створенням підкласу.

    Рішення:
        Для розширення функціональності був створений підклас AdvancedCalculator, який наслідує клас BasicCalculator та додає методи для множення і ділення.


Другий рефакторинг:

    Опис проблеми:
        Клас LibraryBook надає базові функції перевірки наявності книги в бібліотеці та її повернення, але відсутні методи для перевірки стану книги та отримання інформації про книгу.

    Рішення:
        Для додавання цієї функціональності був створений клас LibraryBookDetails, який використовує делегування для роботи з об'єктом LibraryBook та надає методи check_condition і get_info.