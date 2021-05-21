# Test Case ID NV1 Проверка валидации номера банковской карты
### Приоритет (Priority): High
### Номера карт / Bug Reported - Шаги (Steps to reproduce) - Expected result (OK / FAIL) - Actual result (Pass / Failed)

1. Проверка карт с номерами в 14 цифр / Bug Reported: [Bug Report #2:](https://github.com/BabintsevaS/TestingNValidator/issues/2#issue-881728079)  Валидный номер карты с номером в 14 цифр не принимается
   1. Вводим валидный номер карты Diners Club - Carte Blanche (14 цифр): 30353986170923 - Expected result: OK - Actual result: Failed
   1. Вводим валидный номер карты Diners Club - International (14 цифр): 30320163778794 - Expected result: OK - Actual result: Failed

1. Проверка карт с номерами в 15 цифр / Bug Reported: [Bug Report #3:](https://github.com/BabintsevaS/TestingNValidator/issues/3) Валидный номер карты с номером в 15 цифр не принимается
   1. Вводим валидный номер карты American Express (AMEX) (15 цифр): 374011112738492 - Expected result: OK - Actual result: Failed
   1. Вводим валидный номер карты American Express (AMEX) (15 цифр): 379658132614114 - Expected result: OK - Actual result: Failed

1. Проверка карт с номерами в 16 цифр / Bug Reported: no
   1. Вводим валидный номер карты MasterCard: (16 цифр): 2221009035649524 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты Discover (16 цифр): 6011100254522735 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты Visa Electron: (16 цифр): 4175003468150110 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты JCB: (16 цифр): 3544499054428165 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты InstaPayment (16 цифр): 6399653320913843 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты Diners Club - North America (16 цифр): 5477127640134056 - Expected result:  OK - Actual result: Pass
   1. Вводим валидный номер карты Maestro (16 цифр): 6762160371112845 - Expected result:  OK - Actual result: Pass

1. Проверка карт с номерами в 19 цифр /Bug Reported: [Bug Report #1:](https://github.com/BabintsevaS/TestingNValidator/issues/1#issue-881720304) Валидный номер карты с номером в 19 цифр не принимается
   1. Вводим валидный номер карты VISA (19 цифр): 6011220770465851981 - Expected result: OK - Actual result: Failed
   1. Вводим валидный номер карты Discover (19 цифр): 6011170257641260105 - Expected result: OK - Actual result: Failed
   1. Вводим валидный номер карты JCB (19 цифр): 3531891444165450902 - Expected result: OK - Actual result: Failed

1. Невалидные номера карт / Bug Reported: no
   1. Вводим невалидный номер карты (10 цифр): 2536452578 - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты (17 цифр): 36985452365421587 - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты (20 цифр): 69854752123658974521 - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты: пустое поле - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты: символ пробела - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты: буквенные символы - Expected result: FAIL - Actual result: Pass 
   1. Вводим невалидный номер карты: специальные символы - Expected result: FAIL - Actual result: Pass 