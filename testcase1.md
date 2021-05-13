# Test Case ID NV1 Проверка валидации номера банковской карты
### Приоритет (Priority): High
### Шаги (Steps to reproduce) - Expected result (OK / FAIL) - Actual result (Pass / Failed) - Comments - Bug Reported:
1. Вводим валидный номер карты (16 цифр): 4088405745243541 - Expected result:  OK - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим валидный номер карты (19 цифр): 6011220770465851981 - Expected result: OK - Actual result: Failed - Comments: no - Bug Reported: [Bug Report #1](https://github.com/BabintsevaS/TestingNValidator/issues/1#issue-881720304)
1. Вводим валидный номер карты (14 цифр): 30320163778794 - Expected result: OK - Actual result: Failed - Comments: no - Bug Reported: [Bug Report #2](https://github.com/BabintsevaS/TestingNValidator/issues/2#issue-881728079)
1. Вводим валидный номер карты (15 цифр): 374011112738492 - Expected result: OK - Actual result: Failed - Comments: no - Bug Reported: [Bug Report #3](https://github.com/BabintsevaS/TestingNValidator/issues/3)
1. Вводим невалидный номер карты (10 цифр): 2536452578 - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты (17 цифр): 36985452365421587 - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты (20 цифр): 69854752123658974521 - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты: пустое поле - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты: символ пробела - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты: буквенные символы - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no
1. Вводим невалидный номер карты: специальные символы - Expected result: FAIL - Actual result: Pass - Comments: no - Bug Reported: no