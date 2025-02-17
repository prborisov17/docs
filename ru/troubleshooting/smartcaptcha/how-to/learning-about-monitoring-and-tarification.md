# Как получить информацию о количестве использованных проверок за определённый период



## Описание задачи {#case-description}

Возникла необходимость получить информацию о количестве использованных проверок за определённый период.

## Решение {#case-resolution}

Примерное количество проверок можно найти в разделе **Мониторинг** и выбрать нужный период с помощью временного фильтра.


Описание графиков мониторинга:

* `Checkbox captcha shows` — количество показов стандартной кнопки `Я не робот`;
* `Checkbox captcha results` — количество ответов;
* `Advanced challenge shows` — количество показов проверочного задания;
* `Advanced challenge results` — количество ответов во всплывающем окне;
* `Validate results` — количество валидаций, общее количество ответов.

Тарификация производится только за `Validate results`. Подробнее о правилах тарификации пишем в [документации](../../../smartcaptcha/pricing.md).

Точное количество запросов узнать через мониторинг не получится, но можно посмотреть его в детализации биллинга, если включить разбивку по продуктам. В биллинге показаны все обращения к SmartCaptcha, без разделения на успешные и неуспешные. 

Выгрузить детализацию биллинга в CSV можно при помощи кнопки `Экспорт детализации` в правом верхнем углу — в полученном файле будут данные по запросам SmartCaptcha за каждый день с точностью до единиц.