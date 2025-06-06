# Проверка количества дней отсрочки платежа

В разделе **"Заказы"** в **"Настройках исполнения заказов"** в **"Проверках документов"** устанавливаем проверку - **"Количество дней отсрочки платежа"** для документов **Заказ клиента**.

[![1][1]][1]

[![2][2]][2]

[![3][3]][3]

[![4][4]][4]

Дата задолженности возьмется из регистра "Дебиторская задолженность" или взиморасчетов с клиентами, ведущимися в этой системе (если в соглашении на вкладке "Взаиморасчеты" стоит галочка "Использовать взаиморасчеты для расчета задолженности")  

Переходим к соглашениям с контрагентами и устанавливаем для соглашения "Сладкая жизнь. Соглашение об условии продаж" на вкладке *"Ценовые условия"* максимальное количество дней задолженности - 5.

[![5][5]][5]

В регистре **"Дебиторская задолженность"** фиксируем для соглашения "Сладкая жизнь. Соглашение об условии продаж" дату задолженности (дата последней оплаты) - 01.05.2020.

[![6][6]][6]

Создаем [заказ клиента](../../CustomerOrder.md) с параметрами:

- Дата - 07.05.2020
- Организация - Молочный мир
- Контрагент - ООО "Сладкая жизнь плюс"
- Соглашение об условиях продаж - Сладкая жизнь. Соглашение об условии продаж
- Точка доставки - Сладкая жизнь. Комсомольское шоссе, 4
- Дата отгрузки - 07.05.2020
- Дата доставки - 07.05.2020

Товары:

- Сыр Адыгейский, количество - 10

Нажимаем кнопку **"Провести"**, установится статус заказа - **Проверки не успешны**.

Проверка по количеству дней отсрочки платежа не пройдет, потому что по соглашению "Сладкая жизнь. Соглашение об условии продаж" на дату заказа превышено ожидание по оплате. Об этом будет написано в сообщении при нажатии на гиперссылку *"Успешно 11 из 12"* (12 - количество включенных проверок, 11 - количество пройденных проверок).

[![7][7]][7]

[1]: CheckingTheNumberOfDaysOfDeferredPayment.assets/1.png
[2]: CheckingTheNumberOfDaysOfDeferredPayment.assets/2.png
[3]: CheckingTheNumberOfDaysOfDeferredPayment.assets/3.png
[4]: CheckingTheNumberOfDaysOfDeferredPayment.assets/4.png
[5]: CheckingTheNumberOfDaysOfDeferredPayment.assets/5.png
[6]: CheckingTheNumberOfDaysOfDeferredPayment.assets/6.png
[7]: CheckingTheNumberOfDaysOfDeferredPayment.assets/7.png