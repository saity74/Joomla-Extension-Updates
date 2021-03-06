# Репозиторий обновлений расширений
Чтобы Joomla предложила обновить измененное расширение нужно сделать следующее.

(*В примере будет использоваться компонент каталога com_catalogue*)

## Изменить версию в xml файле расширения
В файле com_catalogue.xml
`<version>2.0.0</version>`
меняем на
`<version>2.0.1</version>`

(**Версия обязательно должна быть выше предыдущей**)

## Поменять версию в файле, лежащем в этом репозитории
В файле com_catalogue_update.xml
`<version>2.0.0</version>`
меняем на
`<version>2.0.1</version>`

## Обновиться
Можно подождать, пока Joomla сама проверить обновления, 
но по умолчанию время кеширования результатов проверки обновлений равно 6 часам.

Если ждать нет времени, то идем в `Менеджер расширений: Обновление` и жмем `Найти обновления`. 
Если и после этого обновления не появились, то нужно проверить 2 вещи в `Настройках` менеджера обновлений:
* `Кэширование обновлений (в часах)` - ставим в `0`
* `Минимальная стабильность` - ставим в `Для разработчиков`

*Конечно, на продакшене не стоить ставить стабильность `Для разработчиков`,
но в данный момент мы активно работаем над компонентом каталога, так что ничего страшного*

**Готово, вы восхитительны!**
