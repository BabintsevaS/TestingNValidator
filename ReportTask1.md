# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

08.05.2021 - 09.05.2021 было проведено функциональное тестирование (Functional testing) приложения Credit Card Number Validator.

На тестирование затрачено: 2 ч.

В результате тестирования выявлены следующие дефекты:
* [Bug Report #1:](https://github.com/BabintsevaS/TestingNValidator/issues/1#issue-881720304) Валидный номер карты с номером в 19 цифр не принимается
* [Bug Report #2:](https://github.com/BabintsevaS/TestingNValidator/issues/2#issue-881728079)  Валидный номер карты с номером в 14 цифр не принимается
* [Bug Report #3:](https://github.com/BabintsevaS/TestingNValidator/issues/3) Валидный номер карты с номером в 15 цифр не принимается

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Test Case ID NV1](https://github.com/BabintsevaS/TestingNValidator/blob/master/testcase1.md)  Проверка валидации номера банковской карты

В качестве тестовых данных использовались данные с сервиса генерации валидных номеров карт [freeformatter.com](https://freeformatter.com/credit-card-number-generator-validator.html):
1. Проверка карт с номерами в 14 цифр 
   1. номер карты Diners Club - Carte Blanche (14 цифр): 30353986170923 - Expected result: OK 
   1. номер карты Diners Club - International (14 цифр): 30320163778794 - Expected result: OK 

1. Проверка карт с номерами в 15 цифр 
   1. номер карты American Express (AMEX) (15 цифр): 374011112738492 - Expected result: OK 
   1. номер карты American Express (AMEX) (15 цифр): 379658132614114 - Expected result: OK 

1. Проверка карт с номерами в 16 цифр 
   1. номер карты MasterCard: (16 цифр): 2221009035649524 - Expected result:  OK 
   1. номер карты Discover (16 цифр): 6011100254522735 - Expected result:  OK 
   1. номер карты Visa Electron: (16 цифр): 4175003468150110 - Expected result:  OK 
   1. номер карты JCB: (16 цифр): 3544499054428165 - Expected result:  OK 
   1. номер карты InstaPayment (16 цифр): 6399653320913843 - Expected result:  OK 
   1. номер карты Diners Club - North America (16 цифр): 5477127640134056 - Expected result:  OK 
   1. номер карты Maestro (16 цифр): 6762160371112845 - Expected result:  OK 

1. Проверка карт с номерами в 19 цифр 
   1. номер карты VISA (19 цифр): 6011220770465851981 - Expected result: OK 
   1. номер карты Discover (19 цифр): 6011170257641260105 - Expected result: OK 
   1. номер карты JCB (19 цифр): 3531891444165450902 - Expected result: OK 

1. Невалидные номера карт
    1. номер карты (10 цифр): 2536452578 - Expected result: FAIL 
    1. номер карты (17 цифр): 36985452365421587 - Expected result: FAIL 
    1. номер карты (20 цифр): 69854752123658974521 - Expected result: FAIL
    1. номер карты: пустое поле - Expected result: FAIL 
    1. номер карты: символ пробела - Expected result: FAIL 
    1. номер карты: буквенные символы - Expected result: FAIL 
    1. номер карты: специальные символы - Expected result: FAIL

Тестирование производилось в следующем окружении:
* Windows 10 Home 64bit
* Java version 16.0.1
