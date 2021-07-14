# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

13.07.2021 - 13.07.2021 было проведено ручное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 ч

В результате тестирования выявлены следующие дефекты: 

[Программа проверки не принимает номера с карт с количеством цифр не равным 16](https://github.com/iva1111/java1.1-Credit-Card/issues/1)

## Описание процесса тестирования

В качестве тестовых данных использовались данные 
[Credit Card Number Generator & Validator](www.freeformatter.com)

VISA:
- 4532171286257918   result is ok
- 4556804016730041   result is ok
- 4532991999079747848    result is fail

MasterCard:
- 5449721748009874   result is ok
- 5330316502269434   result is ok
- 5348423542509934   result is ok

American Express (AMEX):
- 344976366643258    result is fail
- 373824932228804    result is fail
- 349996357798205    result is fail

Discover:
- 6011005543364312   result is ok
- 6011321618364628   result is ok
- 6011035883713860350   result is fail

JCB:
- 3545202437796483    result is ok
- 3533108812189927    result is ok
- 3529078135942652609    result is fail

Diners Club - North America:
- 5436918853308738    result is ok
- 5489002618482819    result is ok
- 5417980932281719    result is ok

Diners Club - Carte Blanche:
- 30197641435159    result is fail
- 30199774777241    result is fail
- 30521176043783    result is fail

Diners Club - International:
- 36098138794658    result is fail
- 36839767161515    result is fail
- 36284350533269    result is fail

Maestro:
- 6762139163438394    result is ok
- 0604683207064448    result is ok
- 5893879490543895    result is ok

Visa Electron:
- 4917845258567546   result is ok
- 4913044255441418   result is ok
- 4844754109556542   result is ok

InstaPayment:
- 6392226297511754   result is ok
- 6382701203642333   result is ok
- 6372289661644977   result is ok



Тестирование производилось в следующем окружении:

- Windows 10 pro, 64 bit
- Java 11.0.11 2021-04-20
