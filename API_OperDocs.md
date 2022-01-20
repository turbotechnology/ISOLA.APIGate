# API создания операционных документов

## Общая информация


## Функция GetHistory
      begD  = GetFieldDefD(лПараметры, 'begDate', Today);
      endD  = GetFieldDefD(лПараметры, 'endDate', Today + 1);
      AgrID = GetFieldDefI(лПараметры, 'AgreementID');
      HType = GetFieldDefI(лПараметры, 'Type'); 1-ДС 2-ЦБ не задано - все


## Функция PermissionToCreate
Проверяет возможности подать поручение

Параметры:
  - AgreementID         - ID договора
  - OperID              - ID создаваемой операции

Возвращает 1, если для договора AgreementID доступна возможность подачи поручения на своершение операции с типом OperID
 
## Функция PermissionToOpen
  -- Проверка возможности открыть поручение
  -- Возвращает
  --    1 - документ доступен на правку
  --    2 - только чтение
  -- Параметры:
  --   TaskID          - ID документа
  --   Class           - имя класса записи. По умолчанию Управление.Данные.Процесс
  --   AgreementID     - ID договора

## Функция NewCashCarryInTask

## Функция NewCashWithdrawTask

## Функция NewCashTransTask

## Функция NewSecCarryInTask

## Функция NewSecWithdrawTask

## Функция NewSecTransTask
