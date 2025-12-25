# Requirements-Management-QA — NFR, управление требованиями и QA (BSA12–BSA13)

## Оглавление
- [1. Краткое описание проекта](#1-краткое-описание-проекта)
- [2. Цель проекта и бизнес-контекст](#2-цель-проекта-и-бизнес-контекст)
- [3. Стек и инструменты](#3-стек-и-инструменты)
- [4. Структура репозитория](#4-структура-репозитория)
  - [4.1. BSA12_NonfunctionalRequirements](#41-bsa12_nonfunctionalrequirements)
  - [4.2. BSA13_RequirementsManagements](#42-bsa13_requirementsmanagements)
- [5. Артефакты бизнес-системного анализа](#5-артефакты-бизнес-системного-анализа)
- [6. Какие навыки бизнес-системного аналитика демонстрирует проект](#6-какие-навыки-бизнес-системного-аналитика-демонстрирует-проект)

---

## 1. Краткое описание проекта
Репозиторий содержит артефакты нефункциональных требований (NFR), управления требованиями и QA-части (тест-кейсы) на основе учебного кейса (система онлайн-записи **HAIR**).

## 2. Цель проекта и бизнес-контекст
**Цель:** показать умение аналитика:
- выявлять и формулировать NFR,
- классифицировать NFR и задавать измеримые атрибуты качества,
- регистрировать требования с атрибутами/типами/статусами,
- проектировать позитивные и негативные тест-кейсы на основе Use Case/требований.

## 3. Стек и инструменты
- NFR: performance, availability/reliability, scalability, security
- ReqMgmt: учет требований (скриншоты карточек требований)
- QA: test case design (positive/negative)
- Форматы: PDF / PNG

---

## 4. Структура репозитория

### 4.1. BSA12_NonfunctionalRequirements
**Фокус:** полный цикл работы с NFR — от идентификации до атрибутов.

- [`BSA12_NonfunctionalRequirements/Exercise 00 — Identification of Non-Functional Requirements.pdf`](BSA12_NonfunctionalRequirements/Exercise%2000%20%E2%80%94%20Identification%20of%20Non-Functional%20Requirements.pdf)  
  В рамках задания выявлены нефункциональные требования для системы и сформирован первичный список NFR.  
  Навыки: elicitation NFR, системное качество.

- [`BSA12_NonfunctionalRequirements/Exercise 01 — Classification Non-Functional Requirements.pdf`](BSA12_NonfunctionalRequirements/Exercise%2001%20%E2%80%94%20Classification%20Non-Functional%20Requirements.pdf)  
  В рамках задания классифицированы NFR по группам качества.  
  Навыки: taxonomy NFR, структурирование.

- [`BSA12_NonfunctionalRequirements/Exercise 02 — Selection of NFRs.pdf`](BSA12_NonfunctionalRequirements/Exercise%2002%20%E2%80%94%20Selection%20of%20NFRs.pdf)  
  В рамках задания выполнен отбор/уточнение релевантных NFR (фокус на наиболее значимые).  
  Навыки: приоритизация качества, scope NFR.

- [`BSA12_NonfunctionalRequirements/Exercise 03 — Performance Attributes.pdf`](BSA12_NonfunctionalRequirements/Exercise%2003%20%E2%80%94%20Performance%20Attributes.pdf)  
  В рамках задания определены атрибуты производительности (метрики/пороговые значения).  
  Навыки: измеримость NFR, формулировка SLA/SLO.

- [`BSA12_NonfunctionalRequirements/Exercise 04 — Availability and Reliability Attributes.pdf`](BSA12_NonfunctionalRequirements/Exercise%2004%20%E2%80%94%20Availability%20and%20Reliability%20Attributes.pdf)  
  В рамках задания определены атрибуты доступности и надежности.  
  Навыки: reliability engineering на уровне требований.

- [`BSA12_NonfunctionalRequirements/Exercise 05 — Scalability Attributes.pdf`](BSA12_NonfunctionalRequirements/Exercise%2005%20%E2%80%94%20Scalability%20Attributes.pdf)  
  В рамках задания определены требования к масштабируемости.  
  Навыки: рост нагрузки, capacity thinking.

- [`BSA12_NonfunctionalRequirements/Exercise 06 — Security Attributes.pdf`](BSA12_NonfunctionalRequirements/Exercise%2006%20%E2%80%94%20Security%20Attributes.pdf)  
  В рамках задания определены требования безопасности (контроль доступа, защищенность данных и т.п.).  
  Навыки: security-by-requirements, RBAC/защита данных.

---

### 4.2. BSA13_RequirementsManagements
**Фокус:** учет требований + тест-кейсы.

#### 4.2.1. ex00 — Exercise 00 (регистрация разных типов требований)
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - BRD001.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20BRD001.png)  
  В рамках задания зарегистрировано бизнес-требование (BRD) в системе управления требованиями.  
  Навыки: documentation, типизация требований.

- [`BSA13_RequirementsManagements/ex00/Exercise 00 - FCR001.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20FCR001.png)  
  В рамках задания зарегистрировано функциональное требование (FCR).  
  Навыки: детализация функций, формализация.

- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR001.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR001.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR002.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR002.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR003.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR003.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR004.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR004.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR005.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR005.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - NFR006.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20NFR006.png)  
  В рамках задания зарегистрированы NFR (несколько карточек) с атрибутами/статусами.  
  Навыки: req attributes, управление качеством через требования.

- [`BSA13_RequirementsManagements/ex00/Exercise 00 - USR001.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20USR001.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - USR002.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20USR002.png)  
- [`BSA13_RequirementsManagements/ex00/Exercise 00 - USR003.png`](BSA13_RequirementsManagements/ex00/Exercise%2000%20-%20USR003.png)  
  В рамках задания зарегистрированы пользовательские требования (USR) как отдельные элементы в системе.  
  Навыки: user-centric требования, трассировка.

- [`BSA13_RequirementsManagements/ex00/Exercise 00 - Скриншот всей доки.png`](BSA13_RequirementsManagements/ex00/%D0%AD%D0%BA%D1%81%D0%B5%D1%80%D1%81%D0%B0%D0%B9%D0%B7%2000%20-%20%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%20%D0%B2%D1%81%D0%B5%D0%B9%20%D0%B4%D0%BE%D0%BA%D0%B8.png)  
  В рамках задания зафиксирован общий вид документации/структуры требований в системе управления.  
  Навыки: контроль целостности, обзор набора требований.

#### 4.2.2. ex01 — Exercise 01 (декомпозиция требования на части)
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - IFR001.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20IFR001.png)  
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - IFR002.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20IFR002.png)  
  В рамках задания зарегистрированы элементы IFR (части требования, уточняющие информацию/информирование).  
  Навыки: декомпозиция требований, детализация.

- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SFR001.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SFR001.png)  
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SFR002.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SFR002.png)  
  В рамках задания зарегистрированы элементы SFR (подтребования/частные функции в рамках исходного требования).  
  Навыки: структурирование FR, связность.

- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SHR001.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SHR001.png)  
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SHR002.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SHR002.png)  
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SHR003.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SHR003.png)  
- [`BSA13_RequirementsManagements/ex01/Exercise 01 - SHR004.png`](BSA13_RequirementsManagements/ex01/Exercise%2001%20-%20SHR004.png)  
  В рамках задания зарегистрированы элементы SHR (части требования, связанные с заинтересованными сторонами/согласованиями/ограничениями — согласно типизации курса).  
  Навыки: разбиение требований, управление зависимостями.

#### 4.2.3. ex02 — Exercise 02 (позитивные тест-кейсы)
- [`BSA13_RequirementsManagements/ex02/Exercise 02 - Creating a Positive Test Case.pdf`](BSA13_RequirementsManagements/ex02/Exercise%2002%20-%20Creating%20a%20Positive%20Test%20Case.pdf)  
  В рамках задания описана методика и структура позитивного тест-кейса.  
  Навыки: test design, корректная структура тестов.

- [`BSA13_RequirementsManagements/ex02/TC-UC02-01.png`](BSA13_RequirementsManagements/ex02/TC-UC02-01.png)  
- [`BSA13_RequirementsManagements/ex02/TC-UC02-02.png`](BSA13_RequirementsManagements/ex02/TC-UC02-02.png)  
- [`BSA13_RequirementsManagements/ex02/TC-UC02-03.png`](BSA13_RequirementsManagements/ex02/TC-UC02-03.png)  
  В рамках задания подготовлены позитивные тест-кейсы, привязанные к UC (TC-UC02-xx).  
  Навыки: покрытие основного сценария, воспроизводимость.

#### 4.2.4. ex03 — Exercise 03 (негативные тест-кейсы)
- [`BSA13_RequirementsManagements/ex03/Exercise 03 — Creating a Negative Test Case.pdf`](BSA13_RequirementsManagements/ex03/Exercise%2003%20%E2%80%94%20Creating%20a%20Negative%20Test%20Case.pdf)  
  В рамках задания описана методика и структура негативного тест-кейса.  
  Навыки: negative testing, граничные случаи.

- [`BSA13_RequirementsManagements/ex03/Exercise 03 - NTC-UC02-01.png`](BSA13_RequirementsManagements/ex03/Exercise%2003%20-%20NTC-UC02-01.png)  
- [`BSA13_RequirementsManagements/ex03/Exercise 03 - NTC-UC02-02.png`](BSA13_RequirementsManagements/ex03/Exercise%2003%20-%20NTC-UC02-02.png)  
- [`BSA13_RequirementsManagements/ex03/Exercise 03 - NTC-UC02-03.png`](BSA13_RequirementsManagements/ex03/Exercise%2003%20-%20NTC-UC02-03.png)  
  В рамках задания подготовлены негативные тест-кейсы (NTC-UC02-xx) для проверки ошибок/ограничений.  
  Навыки: проверка валидаций, обработка исключений.

#### 4.2.5. Exercise 04 — Result Evaluation
- `BSA13_RequirementsManagements/Exercise 04 – Result Evaluation`  
  Раздел указан в структуре репозитория; отдельные файлы не перечислены.  
  Навыки: оценка результатов тестирования/качества (если отражено внутри раздела).

---

## 5. Артефакты бизнес-системного анализа
- NFR: `BSA12_NonfunctionalRequirements/*`
- ReqMgmt: `BSA13_RequirementsManagements/ex00/*`, `BSA13_RequirementsManagements/ex01/*`
- QA test cases: `BSA13_RequirementsManagements/ex02/*`, `BSA13_RequirementsManagements/ex03/*`

## 6. Какие навыки бизнес-системного аналитика демонстрирует проект
- NFR engineering: выявление, классификация, метрики качества
- Requirements management: типизация, статусы, атрибуты, декомпозиция требований
- QA: проектирование тест-кейсов (positive/negative), трассировка к UC/требованиям
