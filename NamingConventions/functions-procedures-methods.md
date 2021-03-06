# Соглашения о наименовании

### Функции, процедуры, методы

Именование функций, процедур и методов классов производится согласно стилю InfixCaps. Первые буквы слов, присутствующих в названии функции или процедуры, должны быть заглавными, как и буквы любой включенной в идентификатор аббревиатуры. Все остальные буквы представляются в нижнем регистре. Подчеркивания в именах процедур и функций не используются.

Имя процедуры или функции должно быть глаголом в повелительном наклонении. Допускаются фразовые глаголы и содержащие глаголы выражения. Имя должно быть сформулировано так, чтобы давать представление о назначении функции или процедуры, возвращаемом значении \(для функции\) и, по возможности, алгоритме ее работы.

Примеры наименований:

```Pascal
// ПРАВИЛЬНО:

  ShowStatus
  DrawCircle
  AddLayoutComponent

// НЕПРАВИЛЬНО:

  MouseButton  // Не содержит глагол, не описывает функцию
  drawCircle   // Начинается со строчной буквы
  add_layout_component    // Содержит подчеркивания

  ServerRunning    // Содержит глагол, но не в повелительном наклонении
// Назначение данной конструкции неясно. 
// Согласно названию, ее содержимое может использоваться
// как для запуска сервера, так и для проверки его работы.
// Один из корректных вариантов: IsServerRunning
```

Вышеупомянутые правила актуальны и для методов.

Метод, использующийся для получения значения или установки какого-либо свойства класса должен называться `GetProperty` или `SetProperty` соответственно, где `Property` - имя свойства, с которым ведется работа. Например:

```Pascal
GetHeight, SetHeight
```

Метод, использующийся для проверки классового свойства типа Boolean, должен называться `IsXxx`, где `Xxx` - имя тестируемого свойства. Например:

```Pascal
IsResizable, IsVisible
```



