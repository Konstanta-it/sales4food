# Проверка дебиторской задолженности

В разделе **"Заказы"** в **"Настройках исполнения заказов"** в **"Проверках документов"** устанавливаем проверку - **"Дебиторская задолженность"** для документов **Заказ клиента**

В соглашении с покупателем на вкладке "Ценовые условия" указывается максимальная дебиторская задолженность (Запрещать отгрузку при задолженности более ...)

[![5][5]][5]

Задолженность без учета суммы текущего заказа - дебиторская задолженность из регистра "Дебиторская задолженность" или взиморасчеты с клиентами, ведущиеся в этой системе (если в соглашении на вкладке "Взаиморасчеты" стоит галочка "Использовать взаиморасчеты для расчета задолженности"), если по заказу уже создана реализация 

Задолженность по другим заказам - сумма по всем неоплаченным заказам (у которых нет реализации) по данному соглашению, если на вкладке "Ценовые условия" стоит галочка "Учитывать неоплаченные заказы"    

Общая сумма задолженности - сумма задолженностей без учета суммы текущего заказа, задолженности по другим заказам и сумме текущего заказа (если на вкладке "Ценовые условия" стоит галочка "Учитывать неоплаченные заказы"). Именно она сравнивается с максимальной дебиторской задолженностью

[![6][6]][6]

[5]: CheckingAccountsReceivable.assets/5.png
[6]: CheckingAccountsReceivable.assets/6.png