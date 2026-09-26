# Asterisk-Bridge-GLPI

**Попап звонка, click-to-call и заявки из телефона — прямо в GLPI.** 

> важно! через промежуточную локальную ATC | important! through an intermediate local ATC

**Русский** · [English](#en)

Asterisk Bridge связывает **Asterisk / FreePBX** с **GLPI**. Звонит телефон — GLPI показывает карточку звонящего. В один клик: перезвонить, открыть карточку или создать заявку. Больше никакого копирования номеров руками.

<p align="center">
  <img src="https://github.com/user-attachments/assets/42df7c0a-654b-4cd2-bc1d-d37ea3312746" width="380" />
  <img src="https://github.com/user-attachments/assets/98d0d2c8-3bc4-499c-8e27-f76ad1f8ffc6" width="380" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/931f9974-2df7-4e60-a056-c26bc58df876" width="700" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/3842a22b-1b94-4a57-a8cf-9c3e76ff0b47" width="550" />
</p>

---

<a name="ru"></a>

## Asterisk Bridge для GLPI — возможности

**Соединяет телефонию (Asterisk) и сервисдеск GLPI: звонки, статистика, справочник добавочных и рабочее место оператора — прямо внутри GLPI.**

### Звонки и работа оператора
- **Журнал звонков** — входящие, исходящие, внутренние и пропущенные; с привязкой к сотруднику, фильтрами и постраничным просмотром.
- **Кнопка «Позвонить» прямо из заявки**: сначала звонит телефон оператора, после подъёма трубки — клиенту.
- **Всплывающая карточка при входящем** — кто звонит и какая за этим заявка или пользователь, не переключаясь между окнами.
- **Уведомление о пропущенном** звонке.
- **Точные длительности**: «время до ответа» и «чистое время разговора» — по каждому звонку.

### Отчёты и статистика
- **Сводка**: всего / входящие / исходящие / внутренние, отвечено / пропущено, доля пропущенных.
- **Средняя длительность разговора** и **среднее время до ответа**.
- **Разрез по операторам**: кто сколько принял и пропустил.
- Журнал **«Кто кому звонил»** с фильтрами по времени, направлению и статусу.
- **История по номеру**: кто и в какие периоды пользовался добавочным (удобно при передаче номеров между сотрудниками).
- Экспорт отчётов.

### Справочник добавочных
- Добавочные с привязкой к сотруднику, именем и CallerID.
- **Пароли добавочных**: генерация, смена и просмотр. Пароли хранятся **в защищённом виде**, а каждый показ **фиксируется в аудите**.
- **Состояние номера**: активен, применён на АТС, ошибки применения — с кнопкой **«Создать в АТС»**.
- Единый центр: сам номер, правила набора, пароль и применение — в одном месте.

### Правила набора
- Настраиваемые правила исходящих звонков (префиксы и маршруты) — куда уходит вызов из кнопки «Позвонить».

### Доступ и безопасность
- **Права по профилям**: Телефония · Статистика · Кнопка «Позвонить» · Правила набора · Номера · Аудит.
- **Вкладка «Аудит»** — кто, когда и с какого адреса открывал пароли добавочных.
- Пароли номеров хранятся **в защищённом виде**; ключ шифрования — **отдельно от базы**.

### Прочее
- Русский и английский интерфейс.
- Работает с отдельной АТС на **Asterisk** и стыкуется с головной АТС.
- **Связь «звонок ↔ заявка»**: из звонка можно создать заявку, а в журнале видно, к какой заявке относится разговор.

### В планах
Статусы операторов (обед / отошёл / смена окончена) · очереди с правилами распределения · переводы между линиями · возврат клиента к «своему» оператору · обратные звонки.

---

<a name="en"></a>

[Русский](#ru) · **English**

## Asterisk Bridge for GLPI — Features

**Connects your telephony (Asterisk) with the GLPI service desk: calls, statistics, an extension registry and the agent workspace — right inside GLPI.**

### Calls and agent workspace
- **Call log** — inbound, outbound, internal and missed calls; linked to the employee, with filters and paging.
- **“Call” button right from a ticket**: your phone rings first, and once you pick up, the system calls the client.
- **Incoming-call pop-up** — who is calling and which ticket or user is behind it, without switching windows.
- **Missed-call notification.**
- **Accurate durations**: “time to answer” and “talk time” for every call.

### Reports and statistics
- **Summary**: total / inbound / outbound / internal, answered / missed, missed share.
- **Average talk time** and **average time to answer**.
- **Per-agent breakdown**: who answered and who missed.
- **“Who called whom”** journal with filters by time, direction and status.
- **Number history**: who used an extension and in which periods (handy when numbers are handed over between employees).
- Report export.

### Extension registry
- Extensions linked to an employee, with name and CallerID.
- **Extension passwords**: generate, change and view. Passwords are stored **securely**, and every reveal is **recorded in the audit**.
- **Number status**: active, provisioned on the PBX, provisioning errors — with a **“Create on PBX”** button.
- One place for the number, its dial rules, its password and provisioning.

### Dial rules
- Configurable outbound dial rules (prefixes and routes) — where a call from the “Call” button goes.

### Access and security
- **Per-profile rights**: Telephony · Statistics · “Call” button · Dial rules · Numbers · Audit.
- **“Audit” tab** — who, when and from which address opened extension passwords.
- Number passwords are stored **securely**; the encryption key is kept **separately from the database**.

### Other
- Russian and English UI.
- Works with a dedicated **Asterisk** PBX and connects to a head-office PBX.
- **Call ↔ ticket link**: create a ticket from a call, and see in the journal which ticket a conversation belongs to.

### Planned
Agent statuses (lunch / away / shift end) · queues with distribution rules · transfers between lines · returning the client to “their” agent · callbacks.
