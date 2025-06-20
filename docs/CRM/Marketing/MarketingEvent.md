# Маркетинговое мероприятие

Маркетинг и продажи - Маркетинговое мероприятие

При создании маркетингового мероприятия указываются:

- Номер (заполняется автоматически)  
- Дата  
- Наименование (может быть сформировано автоматически)  
- Акционные цены (дата начала, дата окончания) - когда акция проводится у нашей организации  
- Влияние акции (дата начала, дата окончания) - период, в течение которого на наших клиентов повлияла акция    
- Проведение у клиента (дата начала, дата окончания)  
Периоды можно заполнить по периоду акционных цен, по проведению у клиента по кнопке "Заполнить периоды"  
- Организация  
- Вид акции:  

    - Отгрузка конечному клиенту  
    - Отгрузка посреднику (объемные показатели рассчитываюся по документу "Вторичные отгрузки товаров")  
- Группа планирования отгрузки  
- Статус:  

    - Планируется  
    - Утверждена  
    - Отменена  
    - Завершена  

- [Профиль акции](MarketingEventProfiles.md)  
- Стратегия влияния на отгрузки:  
    - С приростами  
    - Полнообъемная  
- Тип акции  
- Фактор продаж  

![9]

На закладке **"Номенклатура"** добавляется весь ассортимент, участвующий в акции.

[![3][3]][3]

На закладке **"Контрагенты"** указываются контрагенты, для которых будет действовать данная акция, можно ввести уточнения по точкам доставки.

[![4][4]][4]

На закладке **"Показатели"** происходит планирование показателей маркетингового мероприятия для указанных раннее номенклатур и контрагентов

1. Объемные показатели

    Объемные показатели продаж без акции – это средние продажи, очищенные от акционных приростов  
    Нажав на кнопку **"Заполнить объем" - "Без акции"**, нужно указать количество недель от даты документа, за которые необходимо проанализировать отгрузки. За этот период будут вычислены отгрузки без учета акционных отгрузок

    `Объем продаж без акции = (Объем продаж за период расчета от даты документа - Акционные отгрузки за период расчета от даты документа) * Коэффициент корректировки`

    `Коэффициент корректировки = (Дата окончания акционных цен - Дата начала акционных цен) \ Количество дней периода расчета`

    Основываясь на объеме продаж без акции указывается коэффициент роста    

    На основании объема продаж без акции и коэффициента роста будут рассчитаны прирост и итоговый объем продаж:

    `Прирост = Объем продаж без акции * Коэффициент роста - Объем продаж без акции`

    `Итого = Объем продаж без акции * Коэффициент роста`

2. Ценовые показатели

    Нажатием на кнопку **"Заполнить цены"** - **"Все"** будут автоматически заполнены три вида цен: базовая, отпускная, себестоимость. Отпускная цена определяется по условиям соглашения с клиентом, базовая и себестоимость берутся из соответствующих констант  
    Опираясь на эти цены, необходимо заполнить акционную цену. Можно указать процент скидки и акционная цена будет рассчитана автоматически (или наоборот)  

3.  Затраты

    В группировке **"Затраты"** можно указать затраты на логистику на единицу продукции   
    Также здесь могут быть распределены дополнительные затраты. Для этого в табличной части "Дополнительные затраты" указываются : статья затрат, сумма (дополнительных затрат), вариант распределения (пропорционально марже или выручке), ассортимент (весь ассортимент или его часть)  
    После того, как все статьи указаны, нужно нажать кнопку **"Распределить дополнительные затраты"**  

    Формула распределения дополнительных затрат пропорционально марже :  
    `Сумма дополнительных затрат * Маржинальные показатели с акцией по строке / Сумма маржинальных показателей с акцией`

    Формула распределения дополнительных затрат пропорционально выручке :  
    `Сумма дополнительных затрат * Итоговые объемные показатели по строке * Акционная цена по строке / Сумма (Итоговые объемные показатели по строке * Акционная цена по строке) по всем строкам`

4. Маржинальные показатели

    Маржинальные показатели рассчитываются автоматически при вводе значений.

    `МП без акции = (Отпускная цена - Себестоимость) * Объем продаж без акции`

    `МП с акцией = (Акционная цена - Себестоимость) * Объем продаж итого`

    `Прирост = МП с акцией - МП без акции`

    `Прирост, % = МП с акцией/МП без акции * 100 - 100`

5. Детальные показатели

    В табличной части "Детальные показатели" расположены детальные записи, в которых указаны данные с расчетом по каждому контрагенту по каждой строке

![5]

На закладке **"Влияние"** по кнопке "Обновить по рассчитанным показателям" заполняются итоговые регулярные продажи и прирост по акции по товарным категориям, можно указать каннибализм

[![6][6]][6]

На закладке **"Дополнительно"** указываются способ создания, ответственный, комментарий

После ввода всех показателей и расчета маржинальности, необходимо провести данную акцию и установить ей статус **"Утверждена "**. Только после этого акция будет считаться действующей

На основании маркетинговых мероприятий создаются документы "Скидка (наценка)". Для этого нужно нажать "Создать на основании" - "Скидки (наценки)"  

[![7][7]][7]

На форме создания скидок для каждого контрагента подбираются соглашения, по которым будут скидки. Можно выбрать тип скидки (процентом на номенклатуру / фиксированная цена), в правой части выведена ифнормация по акционной цене

[![8][8]][8]  

Автоматически, после проведение документа "Маркетинговое мероприятие", создается документ ["Акционные отгрузки"](PromShipments.md)

[2]: MarketingEvent.assets/MainPage.png
[3]: MarketingEvent.assets/Nom.png
[4]: MarketingEvent.assets/Contra.png
[5]: MarketingEvent.assets/10.png
[6]: MarketingEvent.assets/Influence.png
[7]: MarketingEvent.assets/7.png
[8]: MarketingEvent.assets/8.png
[9]: MarketingEvent.assets/9.png