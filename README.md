# gb_crm_architecture

## Вводные данные:

Имеется система CRM для телекоммуникационной компании с количеством
операторов в 100 человек.

### CRM состоит из:

- Клиентов (физические и юридические лица)
- Заказов (заказы на услуги, предоставляемые компанией клиенту)
- Обращений (обращения в техническую поддержку)
- Менеджера задач (Kanban-доска для отработки обращений, содержит доски,
задачи, витрину с динамическими фильтрами)

### WorkFlow:

- Пользователь авторизуется в CRM
o Профиль пользователя;
o Уведомления пользователя.

- Пользователю доступны клиенты
o Возможность просматривать список клиентов;
o Возможность поиска по имени клиента;
o Возможность редактировать клиента;
o Возможность создавать клиента.

- Пользователю доступны заказы
o Возможность просматривать список заказов по клиенту;
o Возможность просматривать список заказов;
o Возможность поиска заказа;
o Возможность создавать заказ на клиента.

- Пользователю доступны обращения
o Возможность просматривать обращения;
o Возможность создавать обращение на клиента;
o Возможность закрывать обращение.

- Пользователю доступен менеджер задач
o Пользователю создается доска;
o При создании обращения на доске создается задача;
o У задачи имеется бизнес-процесс;
o По завершению задачи, она закрывается, автоматически закрывается
обращение, нотифицируется (менеджеру, клиенту).

- Имеется интеграция во внешние системы(входящая/исходящая)
Менеджер задач содержит витрину, на которой отображается информация по
задачам. Применяются динамические фильтры.
Время отклика не более 1 секунды.

Система должна быть отказоустойчивой (выбрать способ) и высоконагруженной
(500 rps);

### Решаемые задачи:

1. Разработать доменную модель (любая нотация);
2. Выработать единую архитектуру (монолит, SOA, MSA), с описанием, почему
выбран именно такой подход;
3. Подготовить оптимальное интеграционное решение;
4. Выбрать способ обеспечения отказоустойчивости и работы под нагрузкой;
5. Реализовать блок-схему\диаграмму архитектурного решения, возможно по
этапам Day 0-Daу 2;
6. Выбрать Языки и Стек технологий c альтернативным решением (основная
технология + альтернативная технология) с таблицей сравнительной оценки
предпочтительной (из лекции 5, модуля 4, в приложении), дать оценку для
1,2-х главных технологий.
7. Оценить техническую инфраструктуру, вычислители, ОЗУ, долговременное
хранилище, сеть, на период 5 лет эксплуатации.
8. Дополнительно: оценить общую трудоёмкость решения (должности в
разработке и человеко/месяцы трудозатрат)

### Отчётные документы:
1. Документы должны содержать следующие диаграммы: Use Case, ERD, DFD,
Sequence Diagram (общая и несколько детальных), Class Diagram, Component
Diagram, Deploy Diagram, Интеграционную диаграмму, Архитектуру БД;
2. Подготовить документацию API (Swagger);
3. Результат представить в виде 2-х документов:
● Текстовый документ формата A4 c диаграммами, таблицами и
комментариями.
● Презентация по ключевым диаграммам и идеям.

Компоненты Клиент и Заказы являются legacy с более старым стеком.
Попробовать внедрить legacy в новую архитектуру
