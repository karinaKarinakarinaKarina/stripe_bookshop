# stripe_bookshop
Запуск:
git clone https://github.com/karinaKarinakarinaKarina/stripe_bookshop
распаковать архив
cd test_r
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

При потере данных: 
python manage.py loaddata fixtures/discounts.json > main.Discount 
python manage.py loaddata fixtures/taxes.json > main.Tax
python manage.py loaddata fixtures/items.json > main.Item
python manage.py loaddata fixtures/orders.json > main.Order

Для администрирования сайта, просмотра всех моделей:
python manage.py createsuperuser


Главная страница: http://localhost:8000/
/ - Главная страница со всеми товарами 
admin/ - Админка
item/<item_id> - Просмотр страницы товара
buy/<item_id> - Покупка товара с выводом SessionId
orders/ - Просмотр всех заказов 
order/<order_id> - Оплата заказа с выводом SessionId

<img width="1842" height="890" alt="image" src="https://github.com/user-attachments/assets/9df2d125-f620-4cd7-a685-1a97dd2c8866" />

<img width="1868" height="893" alt="image" src="https://github.com/user-attachments/assets/c007d934-7d5e-45d2-9c3e-7b8e90f4cdcb" />

<img width="1844" height="890" alt="image" src="https://github.com/user-attachments/assets/e6c58e15-f3a7-499a-8b22-c30f7140d3a6" />


