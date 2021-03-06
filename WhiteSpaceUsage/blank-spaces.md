# Пробелы и межстрочные расстояния

### Пробелы

Delphi - очень "чистый" язык программирования, код на котором читается без труда, особенно, если он написан грамотно. Для оформления кода не требуется много пробелов, ведь лишние "разрывы" рассеивают внимание при его изучении.

Необходимо помнить, что пробелы НЕ должны использоваться:

1. Между названием функции или процедуры и открывающей скобкой;
2. Перед или после оператора `.`;
3. Перед унарным оператором и его операндом;
4. Между оператором приведения к типу и приводимым выражением;
5. После открывающей круглой скобки и перед закрывающей круглой скобкой;
6. После открывающей квадратной скобки и перед закрывающей квадратной скобкой;
7. Перед символом "точка с запятой".

Примеры:

```Pascal
// ПРАВИЛЬНО:

  function TMyClass.MyFunc(var AValue: Integer);
  MyPointer := @MyRecord;
  MyClass := TMyClass(MyPointer);
  MyInteger := MyIntegerArray[5];
```

```Pascal
// НЕПРАВИЛЬНО:

  function TMyClass.MyFunc( var AValue: Integer ) ;
  MyPointer := @ MyRecord;
  MyClass := TMyClass ( MyPointer ) ;
  MyInteger := MyIntegerArray [ 5 ] ;
```



