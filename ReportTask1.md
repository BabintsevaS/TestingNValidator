# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

08.05.2021 - 09.05.2021 было проведено функциональное тестирование (Functional testing) приложения Credit Card Number Validator.

На тестирование затрачено: 2 ч.

В результате тестирования выявлены следующие дефекты:
* Bug Report ID NVB01: https://github.com/BabintsevaS/TestingNValidator/issues/1#issue-881720304
* Bug Report ID NVB02: https://github.com/BabintsevaS/TestingNValidator/issues/2#issue-881728079

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Test Case ID NV1 Проверка валидации номера банковской карты

В качестве тестовых данных использовались данные с сервиса генерации валидных номеров карт freeformatter.com:
* номер карты: 4088405745243541, ожидаемый результат:  OK
* номер карты: 6011220770465851981, ожидаемый результат: OK
* номер карты: 30320163778794, ожидаемый результат: OK
* номер карты: пустое поле, ожидаемый результат: FAIL
* номер карты: символ пробела, ожидаемый результат: FAIL
* номер карты: буквенные символы, ожидаемый результат: FAIL
* номер карты: специальные символы, ожидаемый результат: FAIL

Тестирование производилось в следующем окружении:
* Windows 10 Home 64bit
* Java 16