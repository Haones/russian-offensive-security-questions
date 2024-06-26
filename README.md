# Вступление

Этот репозиторий содержит в себе компиляцию вопросов по наступательной безопасности (offensive security). Используя этот материал, можно подготовиться к предстоящему собеседованию или прикинуть какие области знаний Вами не покрыты для самостоятельного обучения. 

Проект является личной инициативой и несет в себе исключительно альтруистические цели. Проект является открытым, каждый желающий может сделать форк или предложить изменения в существующий список вопросов.  Порядок вопросов и их категория носят субъективный характер.  Репозиторий будет наполняться с течением времени, список источников представлен в последнем разделе. Вопросы будут агрегироваться из источников, список источников также будет пополняться. 

# Общие вступительные вопросы

1. Расскажите о себе, о своем опыте, мотивации. В чем выражается интерес к сфере наступательной безопасности?
2. Что вы предпринимаете для личностного и профессионального роста? Как развиваете свои навыки сейчас? Какие ваши источники знаний? 
3. Раскройте понятия "конфиденциальность", "целостность", " доступность " своими словами и приведите примеры.
4. Расскажите ваш воркфлоу по внутрянке/внешке. Какая последовательность действий у вас выстроилась?
5. Расскройте понятия аутентификации и авторизации. В чем фундаментальные отличия этих понятий? Приведите примеры. Могут ли эти процессы быть независимыми друг от друга?

# Сети

1. Расскажите про модель OSI. Что это такое и для чего нужно?
2. Расскажите про канальный уровень. Чем он характеризуется, какие процессы происходят, какие протоколы здесь присутствуют? Какие атаки возможны?
3. Что такое MAC-адрес? Для чего нужен? Как по MAC-адресу определить вендора? Можно ли менять MAC-адрес и на что это влияет?
4. Что такое VLAN? Для чего нужно? Какие потенциальные атаки могут совершаться на этот протокол?
5. Расскажите о протоколе ARP? Какие недостатки безопасности есть в этом протоколе? Как работает атака ARP Spoofing?
6. Расскажите о понятии TTL сетевого уровня модели OSI. Для чего этот атрибут нужен? Как по этому параметру может происходить идентификация операционной системы?
7. Что такое ICMP-flood? На какие параметры атакуемой машины происходит воздействие?
8. Расскажите о протоколе TCP и трехуровневом рукопожатии. Перечислите используемые TCP-флаги в процессе обращения клиента к открытому TCP порту. Что меняется, когда порт становится закрытым?
9. В чем фундаментальные отличия протокола UDP от TCP? Для чего может использоваться UDP?
10. Какую задачу выполняет протокол DNS? Какие типы DNS записей можете перечислить и привести примеры? Что такое передача зоны DNS (DNS Zone Transfer) и как может использоваться злоумышленником? Как протокол DNS может использоваться злоумышленниками при DDoS атаках?

# Операционные системы

## Windows 
1. За что отвечают процессы LSA и LSASS?
2. Что такое база данных SAM? Что в ней находится?
3. Что такое NTLM-хеш? Как его можно извлечь и что с ним делать? Что такое Pass-The-Hash атака?
4. Что такое NetNTLMv1 / NetNTLMv2 хеши. Чем они отличаются от NTLM? Как получить NetNTLM хеш и использовать для дальнейшего продвижения?
5. Расскажите про DPAPI ключи. Где они хранятся и для чего используются? Как можно извлечь?
 
## Linux 
1. Какая информация находится в файле /etc/passwd? Как эта информация может быть использована для повышения привилегий на системе? Что и как влияет на содержимоего этого файла?
2. Что хранится в файле /etc/shadow? Какими привилегиями необходимо обладать для чтения этого файла?
3. Расскажите о переменных окружения. Что это такое и как работает? Дополнительно расскажите о переменной окружения PATH.
4. Что такое SUID-исполняемый файл? Как может использоваться для повышения привилегий в системе?
5. Что такое cron jobs? Как может использоваться для повышения привилегий в системе?
6. О каких уязвимостях ядра Linux вы знаете? Расскажите как они работают. ооооо


## Контейнеры
1. Что такое контейнер? Есть ли отличия между контейнеризацией и виртуализацией?

# Программирование 

# Внешка


## WEB
1. Расскажите о протоколе HTTP. Клиент-серверная архитектура, методы, заголовки, коды ответов, параметры запросов. 
2. Расскажите какие CMS вам известны? На что направлены векторы атаки в этих CMS?
3. Перечислите какие на ваш взгляд самые важные пункты в OWASP TOP 10 и OWASP TOP 10 API. Приведите примеры. 
4. Базовые механизмы изоляции контента в браузерах: Same Origin Policy. Что было бы без SOP?
5. Расскажите про CORS, для чего он используется. Рассказать о типах запросов CORS: обычные и Preflight. Защищает ли CORS от CSRF? Какие бывают неверные конфигурации CORS?
6. XSS и последствия. Какие бывают способы защиты от XSS на уровне приложения и на уровне клиента?
7. Расскажите про SSRF. Меры защиты и обходы этих мер.
8. Расскажите про SQLi и последствия эксплуатации. Способы защиты (экранирование, prepared statements, ORM) и их ограничения / мисконфигурации / варианты обхода. Коротко о NoSQLi и отличия от SQLi.

## Внешние сервисы кроме WEB

# Внутрянка

## Active Directory
1. Расскажите о протоколе LDAP. Для чего и как используется?
2. Расскажите о службе ADCS. Для чего и как используется? Каким атакам может быть подвержен?
3. Расскажите о службе Kerberos. Для чего и как используется? Каким атакам может быть подвержен?
4. Расскажите о сетевой папке SYSVOL. Где она находится в домене ActiveDirectory, для чего предназначена, какие мисконфиги могут быть тут найдены?
4. Каким bloodhound-сбощиком пользуетесь? Назовите известные вам рёбра (edges) в bloodhound и как их эксплуатировать?

# Облака

# Криптография
1. Расскажите как работает ассиметричная криптография на базовом уровне. 
2. Приведите примеры криптографических и некриптографических хеш-функций. Какие могут быть области применения у первых и вторых?
3. Назовите основные свойства криптографической хеш-функций. 
4. Расскажите о протоколе TLS применительно к HTTP.
5. Почему протоколы SSL 1.0, SSL 2.0, SSL 3.0 являются небезопасными?
6. Расскажите о сути атаки Padding Oracle.

# OSINT

1. Назовите используемые вами инструменты технической пассивной разведки.
2. Что такое HumINT, какие средства могут использоваться для такого вида разведки?
3. Какую информацию можно получить из TLS сертификата?
4. Какую информацию можно получить из DNS записей исследуемого домена?
5. Что такое Certificate Transparency в TLS сертификатах и как это свойство может использоваться для задач OSINT?
6. Какая информация может быть получена о юридическом лице и какими источниками вы бы воспользовались?

# Социальная инженерия

# Мобилки

Эта секция вопросов посвящена безопасности мобильных приложений. Затрагиваются вопросы динамического и статического тестирования.

1. Какие вы знаете подходы к хранению данных приложения, как наиболее безопасно хранить данные и как атаковать небезопасное хранение в различных конфигурациях

## Android

1. Дано название мобильного приложения. Какие способы получения APK файла вы знаете? 
2. Что такое AndroidManifest файл? Что в нем находится и как может быть полезно при исследовании безопасности мобильного приложения?
3. Назовите основные компоненты android приложения.
4. В чем опасность экспортируемых компонентов?
5. Назовите несколько способов вызова экспортируемых компонентов.
6. Какими способами можно обойти проверку наличия root-прав в приложении?
7. Что такое SSL-Pinning? От чего защищает? Какими способами может быть реализован?
8. 

## iOS


# Источники
| Номер | URL                                                              |
| ----- | ---------------------------------------------------------------- |
| 1     | https://itanddigital.ru/interviewsecurity                        |
| 2     | https://github.com/redteamcaptain/Pentesting-Interview-Questions |
