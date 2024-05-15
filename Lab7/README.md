Після рефакторингу:

Поля product_id, name, category, price були змінені на приватні, за допомогою зміни префіксу подвійних знаків підкреслення (__).
Додано публічні методи для доступу до цих полів: get_product_id(), get_name(), get_category(), get_price(). 
Додано публічні методи для зміни цих полів: set_name(name), set_category(category), set_price(price).

У методі print_product_details замінено прямий доступ до полів об'єктів Product на виклик відповідних методів доступу.