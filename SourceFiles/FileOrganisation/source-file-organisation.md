# Исходные файлы

### Организация файлов

Все модули, используемые в проектах среды программирования Delphi, должны соответствовать следующему порядку организации элементов:

1. Копирайт, идентификационный комментарий;
2. Название модуля;
3. Директивы компилятора;
4. Раздел интерфейса;
5. Раздел реализации;
6. Признак конца модуля `end.`.

Данные элементы должны быть разделены как минимум одной пустой строкой.

Порядок расположения остальных элементов остается на усмотрение разработчика.

```Pascal
{*******************************************************}
{                                                       }
{       Borland Delphi Visual Component Library         }
{                                                       }
{       Copyright (c) 1995,98 Inprise Corporation       }
{                                                       }
{*******************************************************}

unit Buttons;

{$S-,W-,R-}
{$C PRELOAD}

interface

uses 
  Windows, Messages, Classes, 
  Controls, Forms, Graphics, 
  StdCtrls, ExtCtrls, CommCtrl;
```

В исходном коде продуктов компании Embarcadero используются следующие идентификационные комментарии:

```Pascal
//---------------------------------------------------------------------------

// This software is Copyright (c) 2017 Embarcadero Technologies, Inc.
// You may only use this software if you are an authorized licensee
// of Delphi, C++Builder or RAD Studio (Embarcadero Products).
// This software is considered a Redistributable as defined under
// the software license agreement that comes with the Embarcadero Products
// and is subject to that software license agreement.

//---------------------------------------------------------------------------
```

```Pascal
{*******************************************************}
{                                                       }
{           CodeGear Delphi Runtime Library             }
{                                                       }
{ Copyright(c) 1995-2017 Embarcadero Technologies, Inc. }
{              All rights reserved                      }
{                                                       }
{   Copyright and license exceptions noted in source    }
{                                                       }
{*******************************************************}
```

Не имеет значения, располагается ли раздел описаний типов перед списком констант, порядок их представления может изменяться по усмотрению разработчика.

Раздел реализации требуется начинать с ключевого слова `implementation`. За ним должен следовать список подключений. Далее могут находиться любые подключения или директивы компилятора языка:

```Pascal
implementation

uses 
  Consts, SysUtils, ActnList, 
  ImgList;

{$R BUTTONS.RES}
```

При оформлении программных модулей важна не только их внутренняя организация, но и соответствие содержимого модулей следующему правилу: длина строки кода программы не должна превышать 80 символов.

