## Что это?

Это стили для [Typst](https://typst.app/) для Белорусского Государственного Технологического Университета.

Это не официальный репозиторий, тут могут быть ошибки и несостыковочки.

В конце файла `gost-belstu.typ` есть инструкции для агентов, о том как лучше оформлять записку.

## Как установить?

### Шрифты

По ГОСТу вам нужны будут шрифты `Times New Roman` и `Courier New`.

### Пакет

Файл `gost-belstu.typ` можно просто скопировать куда угодно – у него нет зависимостей.

Скачать последнюю версию можно так:
```sh
wget https://raw.githubusercontent.com/qobrito/gost-belstu/refs/heads/main/gost-belstu.typ -O gost-belstu.typ
```

## Как использовать?

Чтобы применить стили, подключите эту библиотеку и передайте всё содержимое документа функции `styles` (`#show: it => gost.styles(it)`), вот:
```typ
#import "gost-belstu.typ" as gost

#show: it => gost.styles(it);
// для отладки можно использовать:
// #show: gost.styles-debug
```
