# Сценарии распределения затрат

Справочник **"Сценарий распределения затрат"** используется для хранения настроек [распределения затрат](CostAllocation.md).

Справочник расположен в разделе **"Деньги"** в подсистеме **"Закрытие месяца"**

Для сценария распределения затрат указываются:

- Наименование - используется для представления объекта в системе
- [Организация](../CommonInformation/Organization.md)
- [Направление деятельности](DirectionOfActivity.md)
- Пояснение - произвольный комментарий

[![5][5]][5]

На вкладке **"Затраты"** устанавливается либо признак **"Остаток на конец месяца"**, тогда затраты в документе [**"Распределение затрат"**](CostAllocation.md) будут заполняться на конец месяца, либо заполняется поле **"Остаток затрат на дату"** - элемент справочника **Варианты начала периода**, который отвечает за дату на которую расчитываются затраты

В табличной части вкладки **"Затраты"** могут быть заполнены отборы:

- [Подразделение](../CommonInformation/Department.md) - отвечает за то по каким подразделениям будут выбираться затраты
- [Статья затрат](ItemsOfExpenditure.md) - отвечает за отбор затрат по указанным статьям
- Аналитика затрат - отвечает за отбор затрат по указанным аналитикам
- Отбор - позволяет установить дополнительные отборы
- Сортировка - позволяет задать порядок затрат

На вкладке **"База"** заполняются:

- Затраты распределять:
    - На продажи 
    - На продажи и перемещение (Показатель в этом случае может быть только Количество или Вес, База - Рассчитываемая)

- Показатель:

    - Количество - затраты будут распределяться пропорционально количеству отгружаемого товара
    - Сумма - затраты будут распределяться пропорционально сумме за отгружаемый товар
    - Вес - затраты будут распределяться пропорционально весам отгружаемого товара
    - Себестоимость - затраты будут распределяться пропорционально себестоимости отгружаемого товара
    - Валовая прибыль - затраты будут распределяться пропорционально валовой прибыли от отгружаемого товара

- Признак **"База на каждую строку затрат"** - устанавливается для того, чтобы для каждой строки затрат определялась своя база

- Фиксированная или Рассчитываемая

    Если база **Фиксированная**, то таблица вручную заполняется данными:

    - [Подразделение](../CommonInformation/Department.md)
    - [Контрагент](../CommonInformation/Contractor.md)
    - [Заказ клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder.md)
    - Аналитика
    - Количество
    - Сумма
    - Вес
    
    Если база **Рассчитываемая**, то либо устанавливается признак **База распределения на месяц документа**, тогда база определяется за весь месяц в который создано [распределение затрат](CostAllocation.md), либо устанавливается период расчета базы

[![4][4]][4]

В табличной части устанавливаются отборы по которым определяется база (например, если распределяются затраты на доставку нам сторонней транспортной компанией, то базу нужно расчитывать по Перевозчику):

- Торговый представитель - менеджер [точки доставки](../CommonInformation/DeliveryPoint.md)
- Менеджер направления - менеджер группы партнеров для планирования
- Менеджер клиента - менеджер [контрагента](../CommonInformation/Contractor.md)
- [Товарная категория](../CommonInformation/РroductCategory.md)
- Маркетинговое мероприятие
- [Перевозчик](../CommonInformation/Contractor.md)
- Транспортное средство
- Водитель
- [Задание на доставку](../CRM/CustomerService/FormationOfShipments/PlanningOfShipments/DistributionOfShipmentsByCar.md)
- [Холдинг](../CommonInformation/Holding.md)
- [Контрагент](../CommonInformation/Contractor.md)
- [Заказ клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder.md)
- [Подразделение](../CommonInformation/Department.md)
- Отбор - позволяет установить дополнительные отборы
- Сортировка - позволяет задать порядок базы

[1]: CostAllocationScenario.assets/1.png
[4]: CostAllocationScenario.assets/4.png
[5]: CostAllocationScenario.assets/5.png