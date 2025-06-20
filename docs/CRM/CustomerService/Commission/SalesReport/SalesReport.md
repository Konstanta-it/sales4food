# Отчет комиссионера о продажах

В документе **«Отчет комиссионера о продажах»** отражаются проданные комиссионером товары, возвращенные комиссионеру товары от конечных покупателей и рассчитывается комиссионное вознаграждение    
Документ изменяет количество товаров, находящихся у комиссионера : уменьшает из вкладки «Товары», увеличивает из вкладки «Возвращенные товары»

На вкладке «Основное» указываются :  
- Номер и дата документа (заполняются автоматически)  
- Входящий номер документа  
- Период, за который был прислан отчет  
- Организация (видно, если организаций несколько)  
- Подразделение  
- Комиссионер  
- [Соглашение](../Settings/Settings.md)  
- Виды цен продажи и передачи (заполняются автоматически из соглашения)  
- Налогообложение (налогообложение при продажах из соглашения)  
- Табличная часть с расчетом дат задолженностей  
- Флаг «Выписывать счет-фактуры сводно» (при включении настройки счет-фактуры, полученные от покупателей в один день, будут создаваться в одном документе Счет-фактура)   
- Счет-фактура реализация. По кнопке «Оформить» будут создаваться документы Счет-фактура (выданный) для конечных покупателей. По гиперссылке откроется форма со списком созданных счетов-фактур  
- Счет-фактура возвраты. По кнопке «Оформить» будут создаваться документы Счет-фактура корректировочный (выданный) для конечных покупателей, оформивших возврат товаров. По гиперссылке откроется форма со списком созданных счетов-фактур  
- Счет фактура    

При изменении табличных частей с товарами и повторном нажатии кнопки «Оформить» неактуальные счета-фактуры пометятся на удалении, а новые создадутся

[![1]][1]

На вкладке «Товары» указываются проданные комиссионером за период товары   
По кнопке «Заполнить» табличная часть заполнится всеми товарами, которые есть у комиссионера на данный момент  

При включении флага «Есть счет-фактура» становятся доступными для редактирования ячейки : Номер, Дата, Покупатель (выбирается из справочника Контрагенты) соответствующей строки. После оформления счет-фактур гиперссылка на пих появляется в ячейке «Счет-фактура»  

[![2]][2]

На вкладке «Возвращенные товары» указываются возвращенные комиссионеру от покупателей товары за период  

При включении флага «Есть счет-фактура» становятся доступными для редактирования ячейки : Номер, Дата, Покупатель (выбирается из справочника Контрагенты), Счет-фактура (выбирается из списка документов Счет-фактура (выданный)) соответствующей строки. После оформления счет-фактур гиперссылка на них появляется в ячейке «Корр. Счет-фактура»  

[![3]][3]

На вкладке «Комиссионное вознаграждение» указываются :  
- Способ расчета вознаграждения (заполняется из соглашения)  
- Итоговая сумма к учету (разность проданных и возвращенных товаров)  
- Процент комиссии / сумма вознаграждения (видно, если рассчитывается способ вознаграждения, заполняется из соглашения)  
- Флаг «Удерживать вознаграждение» (видно, если рассчитывается способ вознаграждения, заполняется из соглашения)  

[![4]][4]

[1]: 1.png  
[2]: 2.png 
[3]: 3.png 
[4]: 4.png 