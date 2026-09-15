# Saga - Хореография "Оформление заказа"

|    | **Этап**                                                   | **Тип события** | **Название**                       |
|:--:|:-----------------------------------------------------------|:----------------|:-----------------------------------|
| 1  | Получение списка товаров                                   | domain          | ShoppingCartListSucceeded          |
| 2  | Способ доставки выбран успешно                             | domain          | DeliveryMethodSucceeded            |
| 3  | Произошла ошибка при выборе способа доставки               | failed          | DeliveryMethodFailed               |
| 4  | Выбор способа оплаты - успех                               | domain          | PaymentMethodSucceeded             |
| 5  | Выбор способа оплаты - ошибка                              | failed          | PaymentMethodFailed                |
| 6  | Успешное резервирование товаров                            | domain          | ReservationSucceeded               |
| 7  | Ошибка резервирования                                      | failed          | ReservationFailed                  |
| 8  | Время резервирования истекло                               | timeout         | ReservationTimeout                 |
| 9  | Payment URL получен покупателем                            | domain          | PaymentUrlReceived                 |
| 10 | Платежная система не вернула Payment URL - вернула ошибку  | failed          | PaymentUrlFailed                   |
| 11 | Успешный запрос с реквизитами                              | domain          | PaymentDataRequestSucceeded        |
| 12 | Ошибка в запросе с реквизитами                             | failed          | PaymentDataRequestFailed           |
| 13 | Оплата прошла успешно                                      | domain          | PaymentSucceeded                   |
| 14 | Ошибка оплаты                                              | failed          | PaymentFailed                      |
| 15 | Возврат средств                                            | compensation    | RefundSecceeded                    |
| 16 | Успешная заявка на доставку                                | domain          | DeliveryRequestSucceeded           |
| 17 | Ошибка - заявка на доставку                                | failed          | DeliveryRequestFailed              |
| 18 | Успешное Оповещение продавца об оплате                     | domain          | NotificationSellerPaymentSucceeded |
| 19 | Ошибка Оповещения продавца об оплате                       | failed          | NotificationSellerPaymentFailed    |
