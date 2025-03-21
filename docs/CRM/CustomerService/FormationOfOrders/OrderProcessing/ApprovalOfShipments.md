# Утверждение отгрузок

Для планирования отгрузок товаров в разрезе групп планирования отгрузок по клиентам используется АРМ **"Утверждение отгрузок"**. При планировании отгрузок учитываются заявки на производство, остатки, история заказов, текущие заказы на дату отгрузки. 

Для возможности работы с АРМом **"Утверждение отгрузок"** необходимо установить флаг **"Двухэтапное подтверждение заказов"**.

[![22][22]][22]

[![23][23]][23]

Если же флаг не будет поставлен, то в системе будет доступен альтернативный АРМ реализующий функции АРМов [**"Утверждение отгрузок"**](ApprovalOfShipments.md) и [**"Подтверждение заказов"**](OrderConfirmation.md) на вкладке **"Подтверждение заказов"** АРМа **"Формирование плана отгрузки"**. АРМ расположен в разделе **"Склад и доставка"** в подсистеме **"Складская логистика"**.

[![24][24]][24]

АРМ **"Утверждение отгрузок"** расположен в разделе **"Заказы"** в подсистеме **"Обработка заказов клиентов"**.

[![1][1]][1]

Для пользователей, которые занимаются Утверждением отгрузок в системе создан поставляемый профиль доступа *"Утверждение отгрузок"*.

[![2][2]][2]

Утверждение отгрузок происходит по **"Настройкам утверждения отгрузок"**, которые заполняются в разделе **"Заказы"** в подсистеме **"Сервис"** - **Настройки исполнения заказов"**.

[![3][3]][3]

[![4][4]][4]

В **"Настройках утверждения отгрузок"** заполняются:

- Наименование
- Дата отгрузки - элемент справочника **"Варианты начала периода"**, заполняется для определения по дате отгрузки заказов с которыми работаем
- Дата работы - элемент справочника **"Варианты начала периода"**, заполняется для получения остатков
- Дата заявки - элемент справочника **"Варианты начала периода"**, заполняется для определения по дате задания заявок на производство
- Округлять по кратности - при установке признака во время редактирования количество будет округляться к наибольшему ближайшему кратному, кратность устанавливается в регистре "Кратность номенклатуры" или в самой номенклатуре
- Склады отгрузки - перечень складов с которыми работаем
- Этап заявки для чтения - в АРМе будет отображаться количество в заявках из установленного этапа
- Этап заказа клиента для чтения - в АРМе будет отображаться количество в заказах клиента из установленного этапа
- Этап внутреннего заказа для чтения - в АРМе будет отображаться количество во внутренних заказах из установленного этапа
- Этап заказа на перемещение для чтения - в АРМе будет отображаться количество в заказах на перемещение из установленного этапа
- Сценарий заявки - заявки отбираются по указанному сценарию
- Товарные категории - список товарных категорий для определения номенклатур по которым производится корректировка

Остатки в АРМе **"Утверждение отгрузок"** рассчитываются из свободных остатков на складе или из прогнозных остатков производства на дату работы

В АРМе **"Утверждение отгрузок"** есть следующие функции:

1. В контекстном меню, которое вызывается нажатием правой кнопки мыши при выборе заказа в таблице:

    - Обнулить колонку - обнуляется колонка, отвечающая за подтвержденное количество в выбранной группе
    - Обнулить строку - по выбранной номенклатуре будут обнулены все ячейки, отвечающие за подтвержденное количество во всех группах
    - Заказано -> Подтверждено - переносит количество из колонки "Заказано" в колонку "Подтверждено" для выбранной группы

2. В командной панели

    - Сохранить - сохраняет подтвержденное количество по всем группам  
    - Заказано -> Подтверждено - переносит количество из колонки "Заказано" в колонку "Подтверждено" для всех групп
    - Включить/Выключить компактный режим - скрывает/отображает колонки кратность, единицы измерения, заказано для групп планирования отгрузок
    - Скрыть детальный расчет - скрывает колонки расчета остатка, общего количества по группам планирования отгрузок, заявок на производство

[![20][20]][20]

Вносим подтвержденное количество товаров и нажимаем кнопку **"Сохранить"** - тем самым утверждаем количество отгружаемых товаров по группе планирования отгрузок, эти данные в дальнейшем используются при подтверждении заказов. Сохранять можно, только если в настройках указан **один** склад отгрузки

[![21][21]][21]

Отгрузки будут утверждены

[1]: ApprovalOfShipments.assets/1.png
[2]: ApprovalOfShipments.assets/2.png
[3]: ApprovalOfShipments.assets/3.png
[4]: ApprovalOfShipments.assets/4.png
[5]: ApprovalOfShipments.assets/5.png
[6]: ApprovalOfShipments.assets/6.png
[7]: ApprovalOfShipments.assets/7.png
[8]: ApprovalOfShipments.assets/8.png
[9]: ApprovalOfShipments.assets/9.png
[10]: ApprovalOfShipments.assets/10.png
[11]: ApprovalOfShipments.assets/11.png
[12]: ApprovalOfShipments.assets/12.png
[13]: ApprovalOfShipments.assets/13.png
[14]: ApprovalOfShipments.assets/14.png
[15]: ApprovalOfShipments.assets/15.png
[16]: ApprovalOfShipments.assets/16.png
[17]: ApprovalOfShipments.assets/17.png
[18]: ApprovalOfShipments.assets/18.png
[19]: ApprovalOfShipments.assets/19.png
[20]: ApprovalOfShipments.assets/20.png
[21]: ApprovalOfShipments.assets/21.png
[22]: ApprovalOfShipments.assets/22.png
[23]: ApprovalOfShipments.assets/23.png
[24]: ApprovalOfShipments.assets/24.png