# Data Mining Tool System
Проект **Data Mining Tool System** - Инструментальная система интеллектуального анализа данных (ИСИАД) представляет собой программный проект, позволяющий проводить исследования эффективности различных методов интеллектуального анализа данных и применять их для решения поставленных пользователем задач.

ВНИМАНИЕ: Для успешной компиляции проекта необходимо наличие установленной Microsoft Visual Studio версии не ниже 2015. 
 
 Проект выполняется студентами ННГУ им. Лобачевского в рамках выпускной работы.
## Описание струкруры репозитория

Данный репозиторий имеет следующую структуру из папок:

- ***project-files*** - содержит исходный код проекта.
- ***reports*** - выпускные работы и презентации к ним.
- ***tech-doc*** - техническая **утвержденная** документация проекта: диаграммы классов, описание API, UML-диаграммы и т.п.
- ***working-doc*** - рабочая документация проекта: требования к реализации определенной функциональности, документирование интеграционных процессов и т.д.

###Структура папок

####project-files
Данная папка содержит директории ***dms*** и ***lib***. 

Папка ***dms*** содержит исходный код проектов, составляющих систему ИСИАД. Там же находятся файлы решения и проектов ИСИАД, построенные в IDE **Visual Studio 2013**. В данной папке содержатся следующие проекты:

- bin - содержит бинарные файлы проектов данного решения и библиотек, используемых в нем
- dms-app - проект приложения системы, написанный на C#  с использованием WPF.
- dms-solvers - проект-прослойка между библиотеками решателей и dms-app. Написан на C++/CLI
- neurolib - библиотека нейронных сетей. Написана на C/C++
- neuro-test-managed - тестовый проект для проверки работы нейронных сетей через dms-solvers. Написан на C#
- neuro-test-native - тестовый проект для проверки работы нейронных сетей. Написан на C.
- mkl - бинарники и заголовочные файлы библиотеки Intel MKL, необходимы для работы нейронных сетей.

Папка ***lib*** содержит бинарные файлы всех библиотек, подключаемых к проектам ИСИАД.

- extended-wpf-toolkit - библиотека, содержащая дополнительные элементы управления WPF. Подключается к dms-app.
- sqlite - библиотека для работы с БД

####reports
В данной папке хранятся отчеты и презентации к выпускным и курсовым работам. Отчеты разных людей хранятся в разных папках с названиями вида **фамилия-имя**.

####tech-doc
Актуальная техническая документация под каждую часть проекта хранится в подпапке с соответствующим названием. Техническая документация, относящаяся к системе вцелом, находится в подпапке **common**.

####working-doc
Текущая документация, определяющая и координирующая ведущиеся работы:

- meetings - планы и результаты собраний
- class-diagram - Диаграмма классов системы, построена в **Visual Paradigm 13.0**
- entity-diagram - Диаграмма "сущность-связь" БД системы, построена в **Visual Paradigm 13.0**
- user-scenarios.docx - Документ, описывающий доступный функционал системы и графический интерфейс пользователя
