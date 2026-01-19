# Information-System-Design — учебный проект бизнес/системного аналитика (BSA00–BSA11)

## Оглавление
- [1. Краткое описание проекта](#1-краткое-описание-проекта)
- [2. Цель проекта и бизнес-контекст](#2-цель-проекта-и-бизнес-контекст)
- [3. Стек и инструменты](#3-стек-и-инструменты)
- [4. Структура репозитория](#4-структура-репозитория)
  - [4.1. BSA00_Decomposition](#41-bsa00_decomposition)
  - [4.2. BSA01_Stakeholders](#42-bsa01_stakeholders)
  - [4.3. BSA02_Requirements](#43-bsa02_requirements)
  - [4.4. BSA03_HowToRequirements](#44-bsa03_howtorequirements)
  - [4.5. BSA04_Domains](#45-bsa04_domains)
  - [4.6. BSA05_Diagrams](#46-bsa05_diagrams)
  - [4.7. BSA06_BPMN](#47-bsa06_bpmn)
  - [4.8. BSA07_UserStory](#48-bsa07_userstory)
  - [4.9. BSA08_UseCase](#49-bsa08_usecase)
  - [4.10. BSA09_Objects-and-Roles](#410-bsa09_objects-and-roles)
  - [4.11. BSA10_FunctionalRequirements](#411-bsa10_functionalrequirements)
  - [4.12. BSA11_UserInterfaces](#412-bsa11_userinterfaces)
- [5. Артефакты бизнес-системного анализа](#5-артефакты-бизнес-системного-анализа)
- [6. Какие навыки бизнес-системного аналитика демонстрирует проект](#6-какие-навыки-бизнес-системного-аналитика-демонстрирует-проект)

---

## 1. Краткое описание проекта
Репозиторий содержит артефакты учебного проекта по анализу и проектированию информационной системы для двух предметных областей:
- **HAIR** — система онлайн-записи и обслуживания клиентов сети барбершопов (слоты услуг, мастера, клиенты, уведомления, скидки).
- **SHOP** — система обработки и доставки заказов (оператор/диспетчер/курьер, контроль статусов заказа).

В рамках курса выполнены ключевые артефакты системного/бизнес-анализа: декомпозиция, стейкхолдеры, требования as-is/to-be, модели данных, диаграммы процессов/состояний, BPMN, User Stories, Use Cases, объектная модель, UI-спецификация.

## 2. Цель проекта и бизнес-контекст
**Цель:** продемонстрировать полный цикл работ аналитика — от исследования предметной области и формализации требований до проектирования процессов, данных и интерфейсов.

**Бизнес-контекст HAIR:** автоматизация записи и управления слотами услуг, снижение ручных операций и ошибок.  
**Бизнес-контекст SHOP:** упорядочивание обработки заказов и доставки, прозрачное управление статусами и ролями.

## 3. Стек и инструменты
- Моделирование: **BPMN**, **UML**, **DFD**, **Swimlane**, **State diagram / State table**
- Данные: **ERD/логическая модель**, **Data Dictionary**, **CRUD matrix**
- Требования: **as-is/to-be**, **User Stories**, **Use Cases**
- UI: сценарии ролей, перечень экранов, **wireframes**, контроли/валидации
- Форматы: **PDF / SVG / PNG / JPG**

> В этом репозитории отсутствуют отдельные артефакты **SQL** и **Swagger/OpenAPI (YAML/JSON)**.

---

## 4. Структура репозитория

### 4.1. BSA00_Decomposition
**Фокус:** вход в предметную область, источники, глоссарии, декомпозиция.

- [`BSA00_Decomposition/HAIR/ex01__HAIR__infosources.pdf`](BSA00_Decomposition/HAIR/ex01__HAIR__infosources.pdf)  
  В рамках задания определены и зафиксированы источники информации по домену **HAIR** (какие артефакты/люди/документы используются для сбора требований).  
  Навыки: discovery, работа с источниками, формирование базы для elicitation.

- [`BSA00_Decomposition/HAIR/ex02__HAIR__glossary.pdf`](BSA00_Decomposition/HAIR/ex02__HAIR__glossary.pdf)  
  В рамках задания сформирован глоссарий терминов домена **HAIR**.  
  Навыки: терминологическое выравнивание, устранение неоднозначностей.

- [`BSA00_Decomposition/SHOP/ex01__SHOP__infosources.pdf`](BSA00_Decomposition/SHOP/ex01__SHOP__infosources.pdf)  
  В рамках задания определены источники информации по домену **SHOP**.  
  Навыки: discovery, подготовка к сбору требований.

- [`BSA00_Decomposition/SHOP/ex02__SHOP__glossary.pdf`](BSA00_Decomposition/SHOP/ex02__SHOP__glossary.pdf)  
  В рамках задания сформирован глоссарий терминов домена **SHOP**.  
  Навыки: управление терминологией.

- [`BSA00_Decomposition/ex03_decomposition.pdf`](BSA00_Decomposition/ex03_decomposition.pdf)  
  В рамках задания выполнена декомпозиция системы/проблемной области (структурирование на части/подсистемы/функции).  
  Навыки: системное мышление, разбиение сложности.

- [`BSA00_Decomposition/ex04_types.pdf`](BSA00_Decomposition/ex04_types.pdf)  
  В рамках задания описаны типы декомпозиции и их применение.  
  Навыки: методология анализа, выбор подхода к декомпозиции.

- [`BSA00_Decomposition/ex05_types.pdf`](BSA00_Decomposition/ex05_types.pdf)  
  В рамках задания продолжена работа с типами декомпозиции (закрепление на примере).  
  Навыки: практическое применение методологии.

- [`BSA00_Decomposition/ex06_rules.pdf`](BSA00_Decomposition/ex06_rules.pdf)  
  В рамках задания зафиксированы правила корректной декомпозиции и критерии качества разбиения.  
  Навыки: контроль качества аналитических артефактов.

---

### 4.2. BSA01_Stakeholders
**Фокус:** стейкхолдеры, окружение системы, потребности.

- [`BSA01_Stakeholders/ex00__SHOP__stakeholders.pdf`](BSA01_Stakeholders/ex00__SHOP__stakeholders.pdf)  
  В рамках задания составлен перечень стейкхолдеров системы **SHOP** с их ролями/интересами.  
  Навыки: stakeholder analysis, идентификация влияния.

- [`BSA01_Stakeholders/ex01__SHOP__onion.svg`](BSA01_Stakeholders/ex01__SHOP__onion.svg)  
  В файле построена **onion diagram** для **SHOP** (слои окружения: ядро/взаимодействующие/внешние).  
  Навыки: определение границ системы, контекстное моделирование.

- [`BSA01_Stakeholders/ex02__HAIR__needs.pdf`](BSA01_Stakeholders/ex02__HAIR_needs.pdf)  
  В рамках задания выявлены потребности/боли стейкхолдеров домена **HAIR**.  
  Навыки: elicitation, формулировка проблем и ожиданий.

- [`BSA01_Stakeholders/ex02__SHOP__needs.pdf`](BSA01_Stakeholders/ex02__SHOP_needs.pdf)  
  В рамках задания выявлены потребности/боли стейкхолдеров домена **SHOP**.  
  Навыки: elicitation, приоритизация потребностей.

- [`BSA01_Stakeholders/ex03__HAIR__glossary.pdf`](BSA01_Stakeholders/ex03__HAIR__glossary.pdf)  
  В рамках задания актуализирован глоссарий **HAIR** после анализа стейкхолдеров.  
  Навыки: управление изменениями терминологии.

- [`BSA01_Stakeholders/ex03__SHOP__glossary.pdf`](BSA01_Stakeholders/ex03__SHOP__glossary.pdf)  
  В рамках задания актуализирован глоссарий **SHOP** после анализа стейкхолдеров.  
  Навыки: согласование понятий между участниками.

---

### 4.3. BSA02_Requirements
**Фокус:** as-is/to-be, контекст, входные/выходные потоки.

- [`BSA02_Requirements/ex00__HAIR_asis.pdf`](BSA02_Requirements/ex00__HAIR__asis.pdf)  
  В рамках задания описаны роли и действия в текущем процессе (**as-is**) для **HAIR**.  
  Навыки: фиксация текущего состояния, выявление проблемных точек.

- [`BSA02_Requirements/ex00__SHOP_asis.pdf`](BSA02_Requirements/ex00__SHOP__asis.pdf)  
  В рамках задания описаны роли и действия (**as-is**) для **SHOP**.  
  Навыки: анализ текущих процессов.

- [`BSA02_Requirements/ex01__SHOP_context.svg`](BSA02_Requirements/ex01__SHOP__context.svg)  
  В файле описан контекст системы **SHOP** (внешние акторы/системы и взаимодействия).  
  Навыки: контекстное моделирование, границы системы.

- [`BSA02_Requirements/ex02__HAIR_tobe.pdf`](BSA02_Requirements/ex02__HAIR__tobe.pdf)  
  В рамках задания разработано целевое состояние (**to-be**) для **HAIR** с учетом проблем/потребностей.  
  Навыки: проектирование будущего процесса, формирование требований.

- [`BSA02_Requirements/ex02__SHOP_tobe.pdf`](BSA02_Requirements/ex02__SHOP__tobe.pdf)  
  В рамках задания разработано **to-be** для **SHOP**.  
  Навыки: улучшение процессов, формулировка целевых изменений.

- [`BSA02_Requirements/ex03__HAIR_streams.pdf`](BSA02_Requirements/ex03__HAIR__streams.pdf)  
  В рамках задания описаны входные/выходные потоки данных системы **HAIR**.  
  Навыки: data-flow thinking, подготовка к интеграциям/данным.

- [`BSA02_Requirements/ex03__SHOP_streams.pdf`](BSA02_Requirements/ex03__SHOP__streams.pdf)  
  В рамках задания описаны потоки данных **SHOP**.  
  Навыки: определение границ данных и взаимодействий.

- [`BSA02_Requirements/ex04__HAIR_glossary.pdf`](BSA02_Requirements/ex04__HAIR__glossary.pdf)  
  В рамках задания обновлен глоссарий **HAIR** по итогам требований.  
  Навыки: управление знаниями, согласование терминов.

- [`BSA02_Requirements/ex04__SHOP_glossary.pdf`](BSA02_Requirements/ex04__SHOP__glossary.pdf)  
  В рамках задания обновлен глоссарий **SHOP**.  
  Навыки: единая терминология требований.

---

### 4.4. BSA03_HowToRequirements
**Фокус:** техники выявления требований (SHOP), Vision.

- [`BSA03_HowToRequirements/ex00__SHOP_rolegame.pdf`](BSA03_HowToRequirements/ex00__SHOP__rolegame.pdf)  
  В рамках задания описана техника **role game** для выявления требований **SHOP** (сценарии взаимодействия ролей).  
  Навыки: facilitation, интервью/воркшопы, выявление требований через сценарии.

- [`BSA03_HowToRequirements/ex01__SHOP_brainstorming.pdf`](BSA03_HowToRequirements/ex01__SHOP__brainstorming.pdf)  
  В рамках задания зафиксированы результаты **brainstorming** (идеи/проблемы/гипотезы).  
  Навыки: генерация требований, структурирование идей.

- [`BSA03_HowToRequirements/ex02__SHOP_seminar.pdf`](BSA03_HowToRequirements/ex02__SHOP__seminar.pdf)  
  В рамках задания оформлены выводы **seminar** по требованиям.  
  Навыки: фасилитация обсуждений, фиксация решений.

- [`BSA03_HowToRequirements/ex03__SHOP_vision.pdf`](BSA03_HowToRequirements/ex03__SHOP__vision.pdf)  
  В файле сформирован документ **Vision** для **SHOP** (цели, контекст, ценность, границы).  
  Навыки: продуктовое мышление, формирование видения и scope.

---

### 4.5. BSA04_Domains
**Фокус:** сущности, CRUD-валидация, словарь данных, ER-модель.

- [`BSA04_Domains/ex00__HAIR_entity.pdf`](BSA04_Domains/ex00__HAIR_entity.pdf)  
  В рамках задания выделены сущности домена **HAIR**.  
  Навыки: domain modeling, выявление объектов предметной области.

- [`BSA04_Domains/ex00__SHOP_entity.pdf`](BSA04_Domains/ex00__SHOP_entity.pdf)  
  В рамках задания выделены сущности домена **SHOP**.  
  Навыки: domain modeling.

- [`BSA04_Domains/ex01__HAIR_crud.pdf`](BSA04_Domains/ex01__HAIR_crud.pdf)  
  В рамках задания построена CRUD-матрица для ключевых сущностей **HAIR**.  
  Навыки: валидация полноты требований, распределение операций по ролям/процессам.

- [`BSA04_Domains/ex02__HAIR_dict.pdf`](BSA04_Domains/ex02__HAIR_dict.pdf)  
  В рамках задания составлен словарь данных (атрибуты сущностей/справочников) для **HAIR**.  
  Навыки: спецификация данных, атрибутный уровень требований.

- [`BSA04_Domains/ex02__SHOP_dict.pdf`](BSA04_Domains/ex02__SHOP_dict.pdf)  
  В рамках задания составлен словарь данных для **SHOP**.  
  Навыки: data dictionary.

- [`BSA04_Domains/ex03__HAIR_model.svg`](BSA04_Domains/ex03__HAIR_model.svg)  
  В файле построена логическая модель данных (ERD) для **HAIR**.  
  Навыки: ERD/relationships, нормализация на уровне концепта.

- [`BSA04_Domains/ex03__SHOP_model.svg`](BSA04_Domains/ex03__SHOP_model.svg)  
  В файле построена логическая модель данных (ERD) для **SHOP**.  
  Навыки: проектирование данных.

---

### 4.6. BSA05_Diagrams
**Фокус:** DFD/Swimlane/State.

- [`BSA05_Diagrams/ex00_HAIR_dfd.png`](BSA05_Diagrams/ex00_HAIR_dfd.png)  
  В рамках задания построена DFD-диаграмма для **HAIR** (потоки данных и процессы).  
  Навыки: DFD, системное представление потоков.

- [`BSA05_Diagrams/ex00_SHOP_dfd.png`](BSA05_Diagrams/ex00_SHOP_dfd.png)  
  DFD для **SHOP**.  
  Навыки: DFD.

- [`BSA05_Diagrams/ex01_HAIR_swd.png`](BSA05_Diagrams/ex01_HAIR_swd.png)  
  Swimlane-диаграмма процесса **HAIR** (разделение по ролям/ответственности).  
  Навыки: моделирование процессов, RACI-like разделение ответственности.

- [`BSA05_Diagrams/ex01_SHOP_swd.png`](BSA05_Diagrams/ex01_SHOP_swd.png)  
  Swimlane для **SHOP**.  
  Навыки: процессный анализ.

- [`BSA05_Diagrams/ex02_HAIR_adswd.png`](BSA05_Diagrams/ex02_HAIR_adswd.png)  
  В рамках задания уточнена swimlane-диаграмма **HAIR** с артефактами/данными.  
  Навыки: повышение точности процесса, связка действий с данными.

- [`BSA05_Diagrams/ex02_SHOP_adswd.png`](BSA05_Diagrams/ex02_SHOP_adswd.png)  
  Аналогично для **SHOP**.  
  Навыки: детализация процессов.

- [`BSA05_Diagrams/ex03_HAIR_dst.png`](BSA05_Diagrams/ex03_HAIR_dst.png)  
  В рамках задания построена диаграмма состояний (state diagram) для объекта домена **HAIR**.  
  Навыки: жизненный цикл сущностей, статусы и переходы.

- [`BSA05_Diagrams/ex03_SHOP_dst.png`](BSA05_Diagrams/ex03_SHOP_dst.png)  
  Диаграмма состояний для **SHOP**.  
  Навыки: state modeling.

- [`BSA05_Diagrams/ex04_HAIR_tst.pdf`](BSA05_Diagrams/ex04_HAIR_tst.pdf)  
  В рамках задания оформлена таблица состояний (state transition table) для **HAIR**.  
  Навыки: формализация переходов, условия, события.

- [`BSA05_Diagrams/ex04_SHOP_tst.pdf`](BSA05_Diagrams/ex04_SHOP_tst.pdf)  
  Таблица состояний для **SHOP**.  
  Навыки: проверяемость логики статусов.

---

### 4.7. BSA06_BPMN
**Фокус:** BPMN-процессы HAIR + согласование/ревизия.

- [`BSA06_BPMN/ex00_HAIR_base_information.pdf`](BSA06_BPMN/ex00_HAIR_base_information.pdf)  
  В рамках задания собрана базовая информация для моделирования процессов **HAIR** (контекст/участники/объекты).  
  Навыки: подготовка BPMN, сбор исходных данных.

- [`BSA06_BPMN/ex00_SHOP_base_information.pdf`](BSA06_BPMN/ex00_SHOP_base_information.pdf)  
  Базовая информация для **SHOP**.  
  Навыки: подготовка к моделированию.

- [`BSA06_BPMN/ex01_HAIR_mpr.pdf`](BSA06_BPMN/ex01_HAIR_mpr.pdf)  
  В рамках задания определен перечень основных бизнес-процессов **HAIR**.  
  Навыки: выделение процессов, декомпозиция по value stream.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp01_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp01_disc.pdf)  
  В рамках задания оформлено обсуждение/уточнения процесса BPMN №1 (замечания, вопросы, согласование).  
  Навыки: коммуникации, протоколирование, работа с обратной связью.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp02_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp02_disc.pdf)  
  Обсуждение процесса BPMN №2.  
  Навыки: согласование артефактов.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp03_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp03_disc.pdf)  
  Обсуждение процесса BPMN №3.  
  Навыки: управление изменениями.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp04_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp04_disc.pdf)  
  Обсуждение процесса BPMN №4.  
  Навыки: уточнение требований через процесс.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp05_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp05_disc.pdf)  
  Обсуждение процесса BPMN №5.  
  Навыки: согласование.

- [`BSA06_BPMN/ex02/ex02_HAIR_bp06_disc.pdf`](BSA06_BPMN/ex02/ex02_HAIR_bp06_disc.pdf)  
  Обсуждение процесса BPMN №6.  
  Навыки: согласование.

- [`BSA06_BPMN/ex03_HAIR_mpr.pdf`](BSA06_BPMN/ex03_HAIR_mpr.pdf)  
  В рамках задания описаны основные бизнес-процессы **HAIR** (текстовое описание/границы/участники).  
  Навыки: спецификация процессов.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp01.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp01.jpg)  
  В рамках задания построена BPMN-диаграмма процесса **HAIR** №1.  
  Навыки: BPMN notation, события/шлюзы/сообщения.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp02.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp02.jpg)  
  BPMN процесса №2.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp03.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp03.jpg)  
  BPMN процесса №3.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp04.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp04.jpg)  
  BPMN процесса №4.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp05.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp05.jpg)  
  BPMN процесса №5.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp06.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp06.jpg)  
  BPMN процесса №6.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex05_HAIR_glossary.pdf`](BSA06_BPMN/ex05_HAIR_glossary.pdf)  
  В рамках задания выполнена актуализация глоссария **HAIR** после BPMN.  
  Навыки: консистентность терминов между процессами и требованиями.

- [`BSA06_BPMN/ex05_HAIR_rev.pdf`](BSA06_BPMN/ex05_HAIR_rev.pdf)  
  В рамках задания проведена ревизия артефактов **HAIR** по итогам обсуждений и BPMN.  
  Навыки: quality review, управление изменениями, выравнивание артефактов.

---

### 4.8. BSA07_UserStory
**Фокус:** User Stories (HAIR).

- [`BSA07_UserStory/ex00_HAIR_us_MANAGER_.pdf`](BSA07_UserStory/ex00_HAIR_us_MANAGER_.pdf)  
  В рамках задания сформированы User Stories для роли **Manager** в домене **HAIR**.  
  Навыки: user-centric требования, ценность/цель, критерии приемки.

- [`BSA07_UserStory/ex01_HAIR_us_Client, Guest Website Visitor, Master, Accountant_.pdf`](BSA07_UserStory/ex01_HAIR_us_Client,%20Guest%20Website%20Visitor,%20Master,%20Accountant_.pdf)  
  В рамках задания сформированы User Stories для ролей: Client / Guest Website Visitor / Master / Accountant.  
  Навыки: покрытие ролей, согласование ожиданий разных пользователей.

- [`BSA07_UserStory/ex02_HAIR_us.pdf`](BSA07_UserStory/ex02_HAIR_us.pdf)  
  В рамках задания оформлен итоговый документ по User Stories (компоновка/согласование/протокол).  
  Навыки: консолидация требований, управление набором US.

---

### 4.9. BSA08_UseCase
**Фокус:** Use Cases (HAIR).

- [`BSA08_UseCase/ex00_HAIR_UC.pdf`](BSA08_UseCase/ex00_HAIR_UC.pdf)  
  В рамках задания описаны Use Cases HAIR (набор UC и/или основной сценарий).  
  Навыки: формализация сценариев, акторы, предусловия/постусловия.

- [`BSA08_UseCase/ex01_HAIR_UC.pdf`](BSA08_UseCase/ex01_HAIR_UC.pdf)  
  Use Case документ №2 (детализация/дополнение UC).  
  Навыки: альтернативные потоки, исключения.

- [`BSA08_UseCase/ex02_HAIR_UC.pdf`](BSA08_UseCase/ex02_HAIR_UC.pdf)  
  Use Case документ №3.  
  Навыки: полнота сценариев.

- [`BSA08_UseCase/ex03_HAIR_UC.pdf`](BSA08_UseCase/ex03_HAIR_UC.pdf)  
  Use Case документ №4.  
  Навыки: согласование бизнес-правил через сценарии.

- [`BSA08_UseCase/ex04_HAIR_UC.pdf`](BSA08_UseCase/ex04_HAIR_UC.pdf)  
  Use Case документ №5.  
  Навыки: трассировка к объектам/статусам.

- [`BSA08_UseCase/ex05_HAIR_UC.pdf`](BSA08_UseCase/ex05_HAIR_UC.pdf)  
  Use Case документ №6 (закрытие набора UC).  
  Навыки: систематизация UC.

---

### 4.10. BSA09_Objects-and-Roles
**Фокус:** объекты, роли, классы (HSR).

- [`BSA09_Objects and Roles/ex00_HSR_class_persons.pdf`](BSA09_Objects%20and%20Roles/ex00_HSR_class_persons.pdf)  
  В рамках задания выделены классы/сущности для персон (пользователи/персоны) в системе HSR.  
  Навыки: объектное моделирование, атрибуты, роли.

- [`BSA09_Objects and Roles/ex01_HSR_clients_employees.pdf`](BSA09_Objects%20and%20Roles/ex01_HSR_clients_employees.pdf)  
  В рамках задания описаны сущности клиентов и сотрудников, их различия и атрибуты.  
  Навыки: моделирование ролей и прав, доменная сегментация.

- [`BSA09_Objects and Roles/ex02_HSR_dict_entities.pdf`](BSA09_Objects%20and%20Roles/ex02_HSR_dict_entities.pdf)  
  В рамках задания описаны справочники и сущности, связанные с ними.  
  Навыки: reference data, классификаторы.

- [`BSA09_Objects and Roles/ex03_HSR_slots.pdf`](BSA09_Objects%20and%20Roles/ex03_HSR_slots.pdf)  
  В рамках задания описан объект “слот услуги” и связанные атрибуты/состояния/операции.  
  Навыки: анализ ключевого объекта, подготовка к статусной модели и CRUD.

- [`BSA09_Objects and Roles/ex04_HSR_class_diagram.jpg`](BSA09_Objects%20and%20Roles/ex04_HSR_class_diagram.jpg)  
  В файле построена UML class diagram (классы и связи).  
  Навыки: UML, связи/агрегации, целостность модели.

- [`BSA09_Objects and Roles/ex05_HSR_discount_notif_entities.pdf`](BSA09_Objects%20and%20Roles/ex05_HSR_discount_notif_entities.pdf)  
  В рамках задания выделены сущности скидок и уведомлений и их место в модели.  
  Навыки: расширение модели, учет бизнес-правил.

- [`BSA09_Objects and Roles/ex06_HSR_diagram.jpg`](BSA09_Objects%20and%20Roles/ex06_HSR_diagram.jpg)  
  В файле представлена итоговая диаграмма (модель/связи) после уточнений.  
  Навыки: итеративное улучшение модели.

---

### 4.11. BSA10_FunctionalRequirements
**Фокус:** функциональные требования, статусы, CRUD, права.

- [`BSA10_FunctionalRequirements/Exercise 00 — Identifying Objects with Status Model.pdf`](BSA10_FunctionalRequirements/Exercise%2000%20%E2%80%94%20Identifying%20Objects%20with%20Status%20Model.pdf)  
  В рамках задания определены объекты, для которых требуется статусная модель.  
  Навыки: выделение управляемых сущностей, подготовка статусов.

- [`BSA10_FunctionalRequirements/Exercise 01 — Life Cycle of the Service Slots.pdf`](BSA10_FunctionalRequirements/Exercise%2001%20%E2%80%94%20Life%20Cycle%20of%20the%20Service%20Slots.pdf)  
  В рамках задания описан жизненный цикл объекта “слот услуги”.  
  Навыки: state lifecycle, события и переходы.

- [`BSA10_FunctionalRequirements/Exercise 02 — Status Models of Entities.pdf`](BSA10_FunctionalRequirements/Exercise%2002%20%E2%80%94%20Status%20Models%20of%20Entities.pdf)  
  В рамках задания разработаны статусные модели для сущностей системы.  
  Навыки: формализация статусов, условия переходов.

- [`BSA10_FunctionalRequirements/Exercise 03 — Description of Actions on References.pdf`](BSA10_FunctionalRequirements/Exercise%2003%20%E2%80%94%20Description%20of%20Actions%20on%20References.pdf)  
  В рамках задания описаны действия над справочниками/референсными данными.  
  Навыки: CRUD для справочников, администрирование данных.

- [`BSA10_FunctionalRequirements/Exercise 04 — CRUD Operations on the Service Slots Object.pdf`](BSA10_FunctionalRequirements/Exercise%2004%20%E2%80%94%20CRUD%20Operations%20on%20the%20Service%20Slots%20Object.pdf)  
  В рамках задания определены CRUD-операции над “слотом услуги”.  
  Навыки: детализация операций, права/ограничения.

- [`BSA10_FunctionalRequirements/Exercise 05 — Detailed Operations on the Service Slot Object.pdf`](BSA10_FunctionalRequirements/Exercise%2005%20%E2%80%94%20Detailed%20Operations%20on%20the%20Service%20Slot%20Object.pdf)  
  В рамках задания детализированы операции над объектом “слот услуги” (условия, проверки, эффекты).  
  Навыки: спецификация логики, проверяемость.

- [`BSA10_FunctionalRequirements/Exercise 06 — Role Access Rights.pdf`](BSA10_FunctionalRequirements/Exercise%2006%20%E2%80%94%20Role%20Access%20Rights.pdf)  
  В рамках задания определены права доступа по ролям.  
  Навыки: RBAC, безопасность на уровне требований.

---

### 4.12. BSA11_UserInterfaces
**Фокус:** UI-спецификация, сценарии, wireframes.

- [`BSA11_UserInterfaces/Exercise 00 — Choosing the Form of Product Presentation.pdf`](BSA11_UserInterfaces/Exercise%2000%20%E2%80%94%20Choosing%20the%20Form%20of%20Product%20Presentation.pdf)  
  В рамках задания определен подход к представлению продукта/данных в интерфейсе.  
  Навыки: UX-логика, выбор формы подачи информации.

- [`BSA11_UserInterfaces/Exercise 01 — Screen Forms of Classifiers and References.pdf`](BSA11_UserInterfaces/Exercise%2001%20%E2%80%94%20Screen%20Forms%20of%20Classifiers%20and%20References.pdf)  
  В рамках задания описаны экранные формы для классификаторов и справочников.  
  Навыки: проектирование админ-интерфейсов.

- [`BSA11_UserInterfaces/Exercise 02 — Data on the Screen Forms of Classifiers and References.pdf`](BSA11_UserInterfaces/Exercise%2002%20%E2%80%94%20Data%20on%20the%20Screen%20Forms%20of%20Classifiers%20and%20References.pdf)  
  В рамках задания определены данные/поля, отображаемые на формах.  
  Навыки: data-to-UI mapping, спецификация полей.

- [`BSA11_UserInterfaces/Exercise 03 — Key Role Scenarios.pdf`](BSA11_UserInterfaces/Exercise%2003%20%E2%80%94%20Key%20Role%20Scenarios.pdf)  
  В рамках задания описаны ключевые сценарии ролей в UI.  
  Навыки: user flow, приоритизация сценариев.

- [`BSA11_UserInterfaces/Exercise 04 — List of Screen Forms.pdf`](BSA11_UserInterfaces/Exercise%2004%20%E2%80%94%20List%20of%20Screen%20Forms.pdf)  
  В рамках задания составлен перечень экранных форм.  
  Навыки: UI inventory, coverage.

- [`BSA11_UserInterfaces/ex05/Exercise 05 — Master Schedule (wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise%2005%20%E2%80%94%20Master%20Schedule%20(wireframe).pdf)  
  В рамках задания создан wireframe экрана расписания мастера.  
  Навыки: wireframing, UX для расписаний/слотов.

- [`BSA11_UserInterfaces/ex05/Exercise 05 — Preview Your Own Schedule (wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise%2005%20%E2%80%94%20Preview%20Your%20Own%20Schedule%20(wireframe).pdf)  
  Wireframe просмотра собственного расписания.  
  Навыки: UX сценарии пользователя.

- [`BSA11_UserInterfaces/ex05/Exercise 05 — Slot Reservation (wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise%2005%20%E2%80%94%20Slot%20Reservation%20(wireframe).pdf)  
  Wireframe бронирования слота.  
  Навыки: UX критического сценария “запись”.

- [`BSA11_UserInterfaces/Exercise 06 — Controls Description.pdf`](BSA11_UserInterfaces/Exercise%2006%20%E2%80%94%20Controls%20Description.pdf)  
  В рамках задания описаны элементы управления, проверки, ограничения ввода.  
  Навыки: UI-валидации, нефункциональные аспекты удобства/ошибок.

---

## 5. Артефакты бизнес-системного анализа
- Требования (as-is/to-be): `BSA02_Requirements/*`
- Стейкхолдеры и контекст: `BSA01_Stakeholders/*`, `BSA02_Requirements/ex01__SHOP_context.svg`
- BPMN / процессная модель: `BSA06_BPMN/*`
- UML / объектная модель: `BSA09_Objects and Roles/*`
- ERD / модель данных и словари: `BSA04_Domains/*`
- Диаграммы потоков и состояний: `BSA05_Diagrams/*`
- User Stories: `BSA07_UserStory/*`
- Use Cases: `BSA08_UseCase/*`
- Функциональная детализация (статусы/CRUD/права): `BSA10_FunctionalRequirements/*`
- UI-спецификация и wireframes: `BSA11_UserInterfaces/*`

## 6. Какие навыки бизнес-системного аналитика демонстрирует проект
- Анализ предметной области: декомпозиция, глоссарий, сущности
- Стейкхолдер-анализ: карта окружения (onion), потребности/боли
- Формализация требований: as-is/to-be, user stories, use cases
- Процессное моделирование: DFD, swimlane, BPMN
- Моделирование данных: ERD, data dictionary, CRUD-валидация
- Проектирование функциональности: статусы, CRUD-операции, RBAC
- UI-аналитика: сценарии, перечень экранов, wireframes, контроли/валидации
