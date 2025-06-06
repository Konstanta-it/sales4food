# Приемка

Кнопка **"Приемка по заказам"** используется при перемещении для приема на склад получатель.

После открытия формы обработки **"Меню учетных точек"** заполняем поля:

- Дата
- Смена
- Учетная точка
- Сканируем штрихкод сотрудника, если были установлены Индивидуальные права доступа

На форме обработки появятся кнопки выбранной учетной точки, выбираем кнопку **"Приемка по заказам"**.

[![1][1]][1]

Выбираем **"Заказ на перемещение"**, по которому будет осуществляться приемка.

[![2][2]][2]

Далее сканируем штрихкод короба поступившей на склад продукции, номенклатура появится на форме.

[![3][3]][3]

Для завершения работы по приемке нажимаем кнопку **"Завершить"**.

В результате будет создан документ **"Распоряжение на приемку"**. 

[![4][4]][4]

Для отражения расхождений между перемещением и приемкой используется документ **"Акт расхождений после перемещения"** (в подсистеме "Заказы")  
Акт создается на основании перемещения товаров (или из него по кнопке "Оформить расхождения")

На вкладке "Основное" указываются : 
- Номер и дата (заполняются автоматически)
- Основание (Перемещение товаров)
- Заказ на перемещение
- Организация
- Подразделение
- Склад отправитель
- Склад получатель
- Задание на доставку

![5]

На вкладке "Товары" указываются расхождения между приемкой и отгрузкой  
Цена заполняется на дату документа по виду цен себестоимости (из константы)

![6]

[1]: Acceptance.assets/1.png
[2]: Acceptance.assets/2.png
[3]: Acceptance.assets/3.png
[4]: Acceptance.assets/4.png
[5]: Acceptance.assets/5.png
[6]: Acceptance.assets/6.png

