# os-1-msinstall
### Задание 1. Создание скрипта для автоматизации установки под Windows

Если вы не слышали ничего про выполнение пакетных файлов, прочитайте эту [статью](https://ru.wikipedia.org/wiki/Пакетный_файл) (в пункте "Ссылки" приведены 3 ОЧЕНЬ детальные статьи на тему создания и использования bat-файлов). 

Надо отметить, что в современной версии Windows 10 уже [реализуется PowerShell](https://ru.wikipedia.org/wiki/PowerShell), где возможно выполнять команды, поддерживаемые в терминале ОС семейства GNU/Linux.



В первом задании предлагается познакомиться с автоматизированной установкой программного обеспечения в ОС Windows, разобраться с типами установщиков и понять как автоматизировать установку программ с разными типами установщиков. Начинаем с установщика MSI. 

Посмотрите, пожалуйста, [видео](https://youtu.be/zAhxiUQbQGQ):

<iframe width="560" height="315" src="https://www.youtube.com/embed/zAhxiUQbQGQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Повторите шаги, выполняемые в видео, установив на свой компьютер (при наличии системы ОС Windows или на тестовый компьютер, согласовав с преподавателем время и день) разберитесь как устанавливать ПО с параметрами в списке ниже:

Напишите скрипт для установки дистрибутивов следующего ПО:

- архиватор **7-zip** (каталог для установки - по умолчанию);
  - автоматический режим - только указатель хода выполнения,
  - без перезагрузки,
  - вести журнал установки с отображением все сообщений об ошибках в файл 7zip-log.txt,
  - каталог для установки указать явно "C:\Program Files\7-Zip",
- графический редактор **Paint.Net**:
  - полностью автоматическая установка (в том числе и согласие с лицензией),
  - на рабочий стол вывести ярлык для запуска приложения,
  - каталог для установки — "C:\Program Files\Graphics\Paint",
- векторный графический редактор **Inkscape**:
  - установка с сокращенным интерфейсом,
  - без перезапуска,
  - вести журнал установки с отображением всех сообщений об устранимых ошибках в файл inkscape-log.txt,
  - каталог для установки указать явно "C:\Program Files\Graphics\Inkscape",
- офисный редактор **LibreOffice** (последней версии на сайте и русскоязычное языковое расширение для него);
  - автоматический режим - только указатель хода выполнения,
  - без перезагрузки после установки LibreOffice, но с перезагрузкой после установки языкового расширения,
  - вести журнал установки с отображением все сообщений об ошибках в файл libreoffice-install-log.txt,
  - каталог для установки - по умолчанию,
- текстовый редактор **Notepad++**:
  - полностью автоматическая установка,
  - установка в директорию по умолчанию,



**Справочная информация**

1. [Типы инсталляторов](http://www.oszone.net/2766)

2. Ветка на форум с примерами скриптов для автоматизации установки и удаления ПО https://www.cyberforum.ru/cmd-bat/thread1475233.html

3. [Использование пакетных и командных файлов](http://www.oszone.net/2245) для решения различных задач.

   

**Установка ПО для запуска программ на Java**

Прочитайте статью про автоматическую установку Java Runtime Environment и напишите скрипт, позволяющий установить JRE 8 с использованием конфигурационного файла, содержащего следующие параметры: 

- автономный режим установки (без задания вопросов пользователю);
- создание лог-файла с результатами установки (имя лог-файла в текущей директории: jre-log.txt);
- каталог для установки java: "C:\Java\JRE";
- отключить отправку веб-аналитики на сервера Oracle;
- разрешить запуск веб-приложений Java в браузере

Приложите к скрипту и файлу конфигурации лог-файл, получившийся в результате установки (jre-log.txt).

**Справочная информация**

1. https://www.java.com/ru/download/help/silent_install.xml
2. https://docs.oracle.com/javase/8/docs/technotes/guides/install/config.html#installing_with_config_file



В отчете о выполнении задания представить скрипты или общий скрипт по установке указанных выше программ, отчет можно (но не обязательно) дополнить скринкастом с комментариями.

Отчет представить с помощью разметки Markdown в собственном репозитории на GitHub (созданным с использованием GitHub Classroom).