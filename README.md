# vkflex-php

Нативное расширение на C для PHP для склонения имен. Использует vkext/flex из [KittenPHP](https://github.com/vk-com/kphp-kdb). Это тот же движок склонений, который используется **ВКонтакте**.

Включена поддержка русского и украинского.


### Установка
```
$ phpize
$ ./configure
$ make
# make install
```

### Использование

`vkflex($name, $case, $sex, $lang, $type)`

- `$name` - имя или фамилия в кодировке cp1251;
- `$case` - падеж: `Gen`, `Dat`, `Acc`, `Ins` или `Abl`;
- `$sex` - `0` - мужской, `1` - женский;
- `$lang` - `0` - русский, `1` - украинский;
- `$type` - `0` - имя, `1` - фамилия.

Возвращает строку в кодировке cp1251.

См. пример в `test.php`.
