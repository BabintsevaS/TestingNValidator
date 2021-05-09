# Test Case ID NV1 Проверка валидации номера банковской карты
###Приоритет (Priority): High
###Шаги (Steps to reproduce) - Expected result (OK / FAIL) - Actual result (Pass / Failed) - Comments - Bug Reported:
1. Вводим валидный номер карты: 4088405745243541 - ожидаемый результат:  OK - Pass - no - no
1. Вводим валидный номер карты: 6011220770465851981 - ожидаемый результат: OK - Failed - no - Bug Report ID NVB01
1. Вводим валидный номер карты: 30320163778794 - ожидаемый результат: OK - Failed - no - Bug Report ID NVB02
1. Вводим невалидный номер карты: пустое поле - ожидаемый результат: FAIL - Pass - no - no
1. Вводим невалидный номер карты: символ пробела - ожидаемый результат: FAIL - Pass - no - no
1. Вводим невалидный номер карты: буквенные символы - ожидаемый результат: FAIL - Pass - no - no
1. Вводим невалидный номер карты: специальные символы - ожидаемый результат: FAIL - Pass - no - no