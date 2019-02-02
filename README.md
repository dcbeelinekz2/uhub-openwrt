# uhub-openwrt
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
