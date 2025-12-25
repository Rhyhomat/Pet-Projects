# System-Integration-API — интеграции, REST и SOAP (BSA14–BSA16)

## Оглавление
- [1. Краткое описание проекта](#1-краткое-описание-проекта)
- [2. Цель проекта и бизнес-контекст](#2-цель-проекта-и-бизнес-контекст)
- [3. Стек и инструменты](#3-стек-и-инструменты)
- [4. Структура репозитория](#4-структура-репозитория)
  - [4.1. BSA14_SystemIntegration](#41-bsa14_systemintegration)
  - [4.2. BSA15_REST](#42-bsa15_rest)
  - [4.3. BSA16_SOAP](#43-bsa16_soap)
- [5. Артефакты бизнес-системного анализа](#5-артефакты-бизнес-системного-анализа)
- [6. Какие навыки бизнес-системного аналитика демонстрирует проект](#6-какие-навыки-бизнес-системного-аналитика-демонстрирует-проект)

---

## 1. Краткое описание проекта
Репозиторий содержит артефакты по интеграции систем и API:
- **BSA14 (SHOP):** анализ интеграционных потоков данных (источники/получатели/словарь/сценарии/нагрузка/частота).
- **BSA15 (HAIR):** спецификация REST API (методы, контракты request/response, mapping, errors, актуализация UC).
- **BSA16:** SOAP/WSDL (структура WSDL, portType, schema, reverse engineering сообщений, endpoints).

## 2. Цель проекта и бизнес-контекст
**Цель:** показать умение аналитика проектировать интеграции и API:
- выделять data flows и ответственных владельцев данных (master),
- описывать сценарии интеграции и требования к передаче,
- формировать спецификации REST (методы, параметры, ответы, ошибки, маппинг),
- читать WSDL/XSD и выполнять обратное проектирование контрактов SOAP.

## 3. Стек и инструменты
- Integration analysis: Data Flows, Master/Receiver systems, Data Dictionary, Integration Scenarios, Volume/Frequency requirements
- REST: методы, контракты, mapping, error model
- SOAP: WSDL, XSD schema, reverse engineering, endpoint definition
- Форматы: PDF

> Swagger/OpenAPI в виде отдельных YAML/JSON файлов в репозитории не представлен.

---

## 4. Структура репозитория

### 4.1. BSA14_SystemIntegration
**Фокус:** системная интеграция (SHOP).

- [`BSA14_SystemIntegration/Exercise 00 — Data Flows Identification.pdf`](BSA14_SystemIntegration/Exercise%2000%20%E2%80%94%20Data%20Flows%20Identification.pdf)  
  В рамках задания идентифицированы потоки данных между системами/участниками (что и куда передается).  
  Навыки: integration discovery, границы обмена данными.

- [`BSA14_SystemIntegration/Exercise 01 — Master Systems Identification.pdf`](BSA14_SystemIntegration/Exercise%2001%20%E2%80%94%20Master%20Systems%20Identification.pdf)  
  В рамках задания определены мастер-системы (владельцы/источники истины по данным).  
  Навыки: data ownership, MDM логика.

- [`BSA14_SystemIntegration/Exercise 02 — Recipient Systems Identification.pdf`](BSA14_SystemIntegration/Exercise%2002%20%E2%80%94%20Recipient%20Systems%20Identification.pdf)  
  В рамках задания определены системы-получатели данных и цели получения.  
  Навыки: архитектурное мышление, потребители данных.

- [`BSA14_SystemIntegration/Exercise 03 — Data Dictionary.pdf`](BSA14_SystemIntegration/Exercise%2003%20%E2%80%94%20Data%20Dictionary.pdf)  
  В рамках задания оформлен словарь данных для потоков (состав полей/структура передаваемых данных).  
  Навыки: контракт данных, атрибутная спецификация интеграций.

- [`BSA14_SystemIntegration/Exercise 04 — Integration Scenarios Description.pdf`](BSA14_SystemIntegration/Exercise%2004%20%E2%80%94%20Integration%20Scenarios%20Description.pdf)  
  В рамках задания описаны сценарии интеграции (когда и по какому событию выполняется обмен).  
  Навыки: event-driven thinking, описание сценариев передачи.

- [`BSA14_SystemIntegration/Exercise 05 — Define Volume and Quantity Requirements for Data Flows.pdf`](BSA14_SystemIntegration/Exercise%2005%20%E2%80%94%20Define%20Volume%20and%20Quantity%20Requirements%20for%20Data%20Flows.pdf)  
  В рамках задания определены требования к объему/количеству данных (нагрузка, объемы сообщений).  
  Навыки: non-functional thinking для интеграций, capacity.

- [`BSA14_SystemIntegration/Exercise 06 — Determining Frequency and Timing for Data Flows.pdf`](BSA14_SystemIntegration/Exercise%2006%20%E2%80%94%20Determining%20Frequency%20and%20Timing%20for%20Data%20Flows.pdf)  
  В рамках задания определены частота и временные требования обмена (периодичность, окна).  
  Навыки: SLA обмена, требования к расписанию интеграций.

---

### 4.2. BSA15_REST
**Фокус:** REST API (HAIR).

- [`BSA15_REST/Exercise 00 — Terminology.pdf`](BSA15_REST/Exercise%2000%20%E2%80%94%20Terminology.pdf)  
  В рамках задания зафиксирована терминология REST/API для единых определений.  
  Навыки: терминологическая точность, контрактная дисциплина.

- [`BSA15_REST/Exercise 01 — Data Preparation.pdf`](BSA15_REST/Exercise%2001%20%E2%80%94%20Data%20Preparation.pdf)  
  В рамках задания подготовлены исходные данные/объекты для проектирования REST.  
  Навыки: подготовка доменных сущностей к API.

- [`BSA15_REST/Exercise 02 — UC Update.pdf`](BSA15_REST/Exercise%2002%20%E2%80%94%20UC%20Update.pdf)  
  В рамках задания актуализированы Use Cases с учетом интеграции/API.  
  Навыки: согласование UC с интерфейсами системы.

- [`BSA15_REST/Exercise 03 — References Integration.pdf`](BSA15_REST/Exercise%2003%20%E2%80%94%20References%20Integration.pdf)  
  В рамках задания описана интеграция справочников/референсных данных.  
  Навыки: reference data через API, согласованность справочников.

- [`BSA15_REST/Exercise 04 — Definition and Description of Methods.pdf`](BSA15_REST/Exercise%2004%20%E2%80%94%20Definition%20and%20Description%20of%20Methods.pdf)  
  В рамках задания определены и описаны REST-методы (endpoint, назначение, операции).  
  Навыки: API design, соответствие CRUD/HTTP.

- [`BSA15_REST/Exercise 05 — Description of RequestResponse Elements.pdf`](BSA15_REST/Exercise%2005%20%E2%80%94%20Description%20of%20RequestResponse%20Elements.pdf)  
  В рамках задания описаны элементы request/response (поля, типы, обязательность).  
  Навыки: контракт API, спецификация данных.

- [`BSA15_REST/Exercise 06 — Mapping.pdf`](BSA15_REST/Exercise%2006%20%E2%80%94%20Mapping.pdf)  
  В рамках задания выполнен маппинг данных (соответствие полей между системами/моделями).  
  Навыки: data mapping, интеграционная совместимость.

- [`BSA15_REST/Exercise 07 — Errors Description.pdf`](BSA15_REST/Exercise%2007%20%E2%80%94%20Errors%20Description.pdf)  
  В рамках задания описана модель ошибок и обработка нештатных ситуаций (коды/сообщения/условия).  
  Навыки: error model, устойчивость API.

- [`BSA15_REST/Exercise 08 — UC Update.pdf`](BSA15_REST/Exercise%2008%20%E2%80%94%20UC%20Update.pdf)  
  В рамках задания выполнено повторное уточнение Use Cases после спецификации API.  
  Навыки: итеративность, выравнивание требований.

- [`BSA15_REST/Exercise 09 — Definition and Description of Methods.pdf`](BSA15_REST/Exercise%2009%20%E2%80%94%20Definition%20and%20Description%20of%20Methods.pdf)  
  В рамках задания продолжено/завершено описание методов REST (дополнение набора endpoint).  
  Навыки: полнота API покрытия.

---

### 4.3. BSA16_SOAP
**Фокус:** SOAP/WSDL.

- [`BSA16_SOAP/Exercise 00 — Functions of WSDL First Level Tags.pdf`](BSA16_SOAP/Exercise%2000%20%E2%80%94%20Functions%20of%20WSDL%20First%20Level%20Tags.pdf)  
  В рамках задания разобраны теги верхнего уровня WSDL и их назначение.  
  Навыки: чтение WSDL, понимание структуры контракта.

- [`BSA16_SOAP/Exercise 01 — Methods of port Type.pdf`](BSA16_SOAP/Exercise%2001%20%E2%80%94%20Methods%20of%20port%20Type.pdf)  
  В рамках задания проанализированы операции (methods) в portType.  
  Навыки: операции SOAP, интерфейс сервиса.

- [`BSA16_SOAP/Exercise 02 — Section schema.pdf`](BSA16_SOAP/Exercise%2002%20%E2%80%94%20Section%20schema.pdf)  
  В рамках задания разобран раздел schema (XSD) и структура сообщений.  
  Навыки: XSD/типы, спецификация данных в SOAP.

- [`BSA16_SOAP/Exercise 03 — Reverse Engineering.pdf`](BSA16_SOAP/Exercise%2003%20%E2%80%94%20Reverse%20Engineering.pdf)  
  В рамках задания выполнено обратное проектирование (восстановление структуры сообщений/контрактов).  
  Навыки: reverse engineering, аналитика интеграционного контракта.

- [`BSA16_SOAP/Exercise 04 — Reverse Engineering, Addition.pdf`](BSA16_SOAP/Exercise%2004%20%E2%80%94%20Reverse%20Engineering,%20Addition.pdf)  
  В рамках задания дополнено обратное проектирование (уточнение элементов сообщений).  
  Навыки: уточнение контрактов, точность модели.

- [`BSA16_SOAP/Exercise 05 — Endpoint Definition.pdf`](BSA16_SOAP/Exercise%2005%20%E2%80%94%20Endpoint%20Definition.pdf)  
  В рамках задания определены endpoint и параметры доступа к SOAP-сервису (по структуре WSDL).  
  Навыки: endpoint discovery, практическая применимость спецификации.

---

## 5. Артефакты бизнес-системного анализа
- Интеграции (flows, словарь, SLA обмена): `BSA14_SystemIntegration/*`
- REST (методы, контракт, mapping, errors, UC updates): `BSA15_REST/*`
- SOAP/WSDL (структура, reverse, endpoints): `BSA16_SOAP/*`

## 6. Какие навыки бизнес-системного аналитика демонстрирует проект
- Системная интеграция: data flows, мастер-данные, потребители, сценарии обмена
- Требования к интеграциям: объемы, частота, timing, SLA
- API-анализ (REST): методы, request/response контракт, mapping, errors
- SOAP/WSDL: чтение контрактов, XSD, reverse engineering, endpoints
