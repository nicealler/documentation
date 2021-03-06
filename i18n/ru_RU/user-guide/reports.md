# Отчеты

Функция отчетов доступна в [Advanced Pack](https://www.espocrm.com/extensions/advanced-pack/).

Существует два типа отчетов: список и сетка.

## Отчеты Списки

Список выводит те записи, которые соответствуют указанным критериям.

Чтобы создать новый отчет о списке, нажмите вкладку «Отчеты», а затем нажмите кнопку «Создать отчет». Выберите необходимый тип объекта, затем нажмите кнопку «Создать» в разделе «Список отчетов».

В поле _Columns_ выберите поля, которые вы хотите отобразить. Ниже вы можете указать параметры отображения для каждого столбца, например: ширину и выравнивание.

Выберите необходимую сортировку в поле _List Order_.

В разделе _Filters_ вы можете указать критерии, которые определят, какие записи будут перечислены в вашем отчете. Вы можете использовать логические операторы «ИЛИ», «И».

_Runtime Filters_ позволяют вам указывать разные фильтры перед запуском отчета.

Вы можете отображать результаты отчета __export__ в формате excel и csv.

## Отчеты по сетке

В отчете по сетке суммируются значения, сгруппированные по указанным полям. Эти отчеты могут отображаться в виде диаграммы.

![Grid reports](https://raw.githubusercontent.com/espocrm/documentation/master/_static/images/user-guide/reports/grid.png)

Чтобы создать новый отчет о сетях, нажмите вкладку «Отчеты», а затем нажмите кнопку «Создать отчет». Выберите необходимый тип объекта, затем нажмите кнопку «Создать» в разделе «Отчет по сетке».

В поле _Group By_ выберите одно или два поля, в которые вы хотите сгруппировать ваши данные отчета. Можно группировать по месяцам, месяцам, дням поля даты. Если вы группируете по двум полям, ваш отчет будет считаться трехмерным.

В поле _Columns_ выберите одну или несколько совокупных функций, таких как COUNT, SUM (суммирование), MIN, MAX, AVG (среднее значение).

Поле _Order by_ определяет, как будут сортироваться данные отчета.

В разделе _Filters_ вы можете указать критерии, определяющие, какие записи будут использоваться в вашем отчете. Вы можете использовать логические операторы «ИЛИ», «И».

_Runtime Filters_ позволяет вам указать разные фильтры перед запуском отчета.

Отчет по сетке позволяет отображать результаты в форме диаграммы. Существуют следующие типы _chart_: Столбцы (Горизонтальные), Столбцы (Вертикальные), Смещения, Линии.

Результаты __export__ grid report можно получить в формате excel и csv.

## Фильтры

#### Фильтр полей

Простой в использовании тип фильтров. Вы также можете выбрать поля целевого объекта, а также связанные с ним объекты.

![Field filter](https://raw.githubusercontent.com/espocrm/documentation/master/_static/images/user-guide/reports/filter-field.png)

### Или в группе

Или означает, что по крайней мере одно условие в группе должно быть выполнено.

![OR group](https://raw.githubusercontent.com/espocrm/documentation/master/_static/images/user-guide/reports/filter-or.png)

### И в группе

И означает, что все условия в группе должны быть выполнены.

### Без группы

Обеспечивает возможность фильтрации записей, не соответствующих заданным критериям. Например: перечисление учетных записей, которые не имеют возможности с закрытым статусом «Закрытый успешный или закрытый неудачный».

![NOT group](https://raw.githubusercontent.com/espocrm/documentation/master/_static/images/user-guide/reports/filter-not.png)

### Комплексное выражение

Для более продвинутого использования. Вы можете применить функцию для определенного столбца базы данных и сравнить ее с результатом выражения [formula](../administration/formula.md).

Примечание. Если вам нужно сравнить только с простым строковым значением, вы должны поместить его в одинарные кавычки `` некоторые строки``.

Примечание. Функции, предназначенные для взаимодействия с записью сущности, здесь не работают, потому что формальная форма не применяется к конкретной записи.

![Complex Expression filter](https://raw.githubusercontent.com/espocrm/documentation/master/_static/images/user-guide/reports/filter-complex.png)

## Отображение на панели управления

Вы можете отображать любой отчет на панели управления. Для этого вам нужно добавить Report dashlet, а затем выбрать нужный отчет в параметрах dashlet.

## Отправка электронной почты

Можно сделать систему для отправки результатов отчета определенным пользователям на регулярной основе в указанное время. Это необходимо для отдельных отчетов.

## Синхронизация с целевыми списками

Возможно, списки целевых списков синхронизированы с результатами отчета списка. Это удобно для массовой электронной почты, когда вы хотите отправлять электронные письма только контактам, которые соответствуют определенным критериям в момент отправки. Эта функция доступна в подробном представлении любого целевого списка на панели «Синхронизировать с отчетами».
