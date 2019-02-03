## uHUB для LEDE|OPENWRT 
Powered by uhub/0.5.0-git-444add1 on Linux/MIPS

![rafa центравой](https://pp.userapi.com/c847220/v847220549/198398/hA1GFMLHwAk.jpg)


µHub (micro-Hub) — ADC хаб написанный на C под лицензией GPLv3. Работает в операционных системах Linux, Windows, BSD и других. Имеет только базовую функциональность для p2p. Крайне нетребователен к ресурсам — при 350 пользователях занимает в памяти несколько десятков килобайт ОЗУ. Возможна работа на устройствах поддерживающих ПО OpenWRT.

Advanced Direct Connect (ADC) — протокол для файлообменных сетей, основанный на протоколе Direct Connect (DC). ADC-клиенты подключаются к центральному серверу и обмениваются файлами напрямую между участниками сети.

Начиная с версии 3.2 поддерживает шифрование server-client, так называемую ADCS-mode. Начиная с версии 4.0 будет введена система плагинов с простым API. Тестовый хаб автора: adcs://adc.extatic.org:1511

-----------------
0.5.0:
- Use TLS 1.2 and strong ciphers by default, but made this configurable.
- Fix TLS event handling which caused some busy loops
- TLS: Support certificate chains
- Fix bug #211: Better Hublist pinger support by adding the AP flag of the INF message.
- Fix bug #198:  Timers could cause infinite loops
- Sqlite3 is now mandatory
- Added mod_chat_history_sqlite and mod_chat_is_privileged.
- Support for systemd notify and journal logging
- Improved flood control counting to strictly not allow more than the given amount of messages in the configured interval.
- Optimize lookups by CID and nick.
- Added an NMDC and ADC hub redirectors written in Python.
- Fix all Clang compile warnings.
- Install uhub-passwd also.
- Add support for detecting HTTP connections to the hub. Enough to tell browsers to stop calling.
- Compile fixes for OpenBSD, including warnings about strcat.
- Fix crashing autotest due to wrong initialization of the usermanager.
- mod_topic: check argument for NULL
- rename !cleartopic to !resettopic


Пакеты, прошивки https://downloads.openwrt.org/releases/
