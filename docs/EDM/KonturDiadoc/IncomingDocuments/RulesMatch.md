# Правила сопоставления документов

В подключаемом модуле прописаны правила сопоставления электронных входящих документов с документами 1С. Исходя из этих правил выбирается вид при создании на основании входящего электронного документа нашего документа 1С

[![1][1]][1]

Ниже приведена информация по соответствиям: 

| Вид электронного документа | Тип документа 1С |
| ------- | ------- |
| Накладная | Поступление товаров услуг |
| Акт | Поступление товаров услуг |
| Счет фактура / Корректировочный счет фактура | Счет фактура полученный |
| Корректировочная накладная | Корректировка поступления |

Где вид электронного документа соответствует следующим типам документа и функциям:

| Вид электронного документа | Тип документа | Функция документа |
| ------- | ------- | ------- |
| Счет фактура | UniversalTransferDocument | Invoice / СЧФ / КСЧФ |
|  | UniversalTransferDocumentRevision | Invoice / СЧФ / КСЧФ |
|  | Invoice |  |
|  | InvoiceRevision |  |
| Корректировочный счет фактура | UniversalCorrectionDocument | Invoice / СЧФ / КСЧФ |
|  | UniversalCorrectionDocumentRevision | Invoice / СЧФ / КСЧФ |
|  | InvoiceCorrection |  |
|  | InvoiceCorrection |  |
| Накладная / Акт | UniversalTransferDocument | Basic / ДОП / ДИС |
|  | UniversalTransferDocumentRevision | Basic / ДОП / ДИС |
| Накладная | XmlTorg12 |  |
|  | Torg12 |  |
| Акт | XmlAcceptanceCertificate |  |
|  | AcceptanceCertificate |  |
| Корректировочная накладная | UniversalCorrectionDocument | Basic / ДОП / ДИС |
|  | UniversalCorrectionDocumentRevision | Basic / ДОП / ДИС |

Аналогичные соответствия прописаны в типовом модуле УТ.

[1]: RulesMatch.assets/1.png