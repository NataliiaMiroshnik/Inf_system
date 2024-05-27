У наведеному прикладі коду використовувався довгий ланцюжок викликів bank.get_customer().get_account().get_balance(). Це створює тісні залежності між класами та ускладнює підтримку і розширення коду.

Прийняті рішення:
1. Інкапсуляція ланцюжка викликів
    Був доданий метод get_balance до класу Bank, який інкапсулює ланцюжок викликів та надає доступ до балансу напряму. Таким чином, можна отримати баланс без необхідності знати внутрішню структуру класів.

2. Спрощення інтерфейсу
    Метод get_balance забезпечує простий та зрозумілий інтерфейс для отримання балансу, зменшуючи кількість коду і роблячи код більш читабельним.

3. Зменшення залежностей
    Тепер класи Customer та Account не мають публічних методів для отримання внутрішніх даних. Це сприяє зниженню залежностей між класами та полегшує підтримку коду.