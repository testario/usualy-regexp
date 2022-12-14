# Часто используемые регулярки
#### удаление из номера телефона всех нечисловых символов
```
/[^+\d]/g
```
#### проверка на валидность email
```
/^([A-Za-z0-9_\-\.])+\@([A-Za-z0-9_\-\.])+\.([A-Za-z]{2,4})$/
```
#### поразрядный формат числа (100 000 000.00)
```
/\B(?=(\d{3})+(?!\d))/g
```
#### регулярка для проверки даты (учитывается високосный год)
```
/^(?:(?:31(\/|-|\.)(?:0?[13578]|1[02]))\1|(?:(?:29|30)(\/|-|\.)(?:0?[1,3-9]|1[0-2])\2))(?:(?:1[6-9]|[2-9]\d)?\d{2})$|^(?:29(\/|-|\.)0?2\3(?:(?:(?:1[6-9]|[2-9]\d)?(?:0[48]|[2468][048]|[13579][26])|(?:(?:16|[2468][048]|[3579][26])00))))$|^(?:0?[1-9]|1\d|2[0-8])(\/|-|\.)(?:(?:0?[1-9])|(?:1[0-2]))\4(?:(?:1[6-9]|[2-9]\d)?\d{2})$/
```
#### валидация Base64
```
^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$
```
#### удаление повторяющихся слов, идущих друг за другом
```
/(\w+)\s+\1/gi
```
#### проверка номера телефона
```
/^((8|\+7)[\- ]?)?(\(?\d{3}\)?[\- ]?)?[\d\- ]{7,10}$/
```
#### проверка формата расчетного банковского счета
```
/^((\d{5})(\s{1}[-]{1}\s{1})){3}(\d{5})$/
```
