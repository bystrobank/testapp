testapp
=======

Программа демонстрирует взаимосвязь используемых нами технологий
разработки web-приложений - php xml xsd xslt.

Схема обработки запросов следующая:
(xml запрос) -> (php приложение: проверка входных данных на соответсвие
схеме xsd, обработка) -> (xml ответ) -> (xslt преобразование: форма в
браузере) -> (xml запрос) ->....

Ваше задание:
- установить тестовую базу (скрипты в tools/sql/) 
- установить программу на web-сервер (для тестирования откройте в
браузере testapp/web/documentList.php) - данный отчет представляет собой
простой фильтр документов по дате создания 
- разобраться с технологией обработки запросов на основе данной программы
- модифицировать программу, добавив в отчет поля ключевые слова (поле
keywords), удален (да/нет) (поле deleted) 
- модифицировать программу, добавив в форму фильтр по полю наименование
(содержит) 
- модифицировать программу, добавив в форму поле "формат отчета" (html/pdf),
при выборе pdf должен формироваться pdf-файл, содержащий таблицу документов
аналогичного html-версии содержания. Пример формирования PDF из XML:
http://tech.google-it.info/tgi/web/howto_xml_pdf.xhtml

Установленное приложение в openshift
http://php-bystrobank.rhcloud.com/testapp/web/documentList.php
