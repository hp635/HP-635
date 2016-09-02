# О разделе HP 635 ноутбук клуб (laptop hp 635 club)

Тема про ноубук HP 635 (hp635), обсуждения, советы, клуб владельцев.  
Эта страница только для старых владельцев ноутбука HP 635, **покупать не рекомендую** (только если б. у. по дешевке)!

**Обсуждение:** в раздел [Issues](https://github.com/hp635/readme/issues)

# Характеристики (могут различаться в разных моделях)

**Процессор:** APU 1.3 ГГц (AMD E-300, Zacate, не съемный)  
**Оперативная память:** 4 ГБ  
**Видеокарта:** AMD HD 6310 M (интегрированна в APU)

# Какие операционные системы идут на HP 635?

* Windows 7 SP1 x64 (**рекомендуется**) - после установки отключите сбор статистики замедляющий работу
	* <sub>установите [этот](http://download.windowsupdate.com/d/msdownload/update/software/updt/2016/05/windows6.1-kb3125574-v4-x64_2dafb1d203c8964239af3048b5dd4b1264cd93b9.msu) комулятивный пакет обновлений (перед этим установите [3020369](https://support.microsoft.com/en-us/kb/3020369) для исправления ошибок установки). Затем отключите сбор статистики, чтобы не отнимала производительность, инструкции: [1](http://www.overclock.net/t/1587577/windows-7-updates-list-descriptions-windows-7-8-telemetry-preparation), [2](http://techne.alaya.net/?p=12499), [3](http://www.dslreports.com/forum/r30348398-WIN7-Win-7-updates-to-avoid-or-be-careful-with) (прочитайте каждую и выполните, возможно позже скину готовый скрипт)</sub>  
* Ubuntu 14.04.1 (**рекомендуется**) - советую редакцию быстрого рабочего стола XFCE (т.е. устанавливайте Xubuntu 14.04.1)  
* Windows XP - проблема: нету регуляции подсветки  
* Windows 10 - проблема: съедает драгоценную производительность на этом слабом ноутбуке  
* Ubuntu 16.04 - проблема: нету проприетарного драйвера AMD

# Какие игры идут?

* The Elder Scrolls: Skyrim
* Dota 2
* Far Cry 3 (и Blood Dragon)
* Dishonored 1
* BioShock Infinity
* Mass Effect 3

# Какие драйвера установить на Windows 7 SP1 x64?

1. Драйвера [на сайте HP](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061)
	1. Atheros 2011 Wireless LAN Driver - драйвер Wi-Fi
	2. Realtek Local Area Network (LAN) Driver - драйвер для сетевой карты
	3. Atheros Bluetooth Driver - драйвет Bluetooth
	4. Realtek Card Reader Driver - драйвер для Card Reader, SD карточек
2. Драйвер для видеокарты [Catalyst Software Suite 15.7.1](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1)
3. Драйвер для чипсета [AMD Chipset Drivers](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1)
4. Драйвер RAID [AMD RAIDXpert Utility](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1)
5. Realtek [High Definition Audio Codecs](http://www.realtek.com.tw/downloads/) - драйвер для звука
6. [Драйвер сенсорной панели Synaptics](http://www.synaptics.com/resources)
7. [HP Notebook System BIOS Update (AMD Processors)](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - BIOS версии F.48

# Известные проблемы ноутбука HP 635

1. В системах Linux странное дребезжание колонок. Видимо от того, что драйвер звука с ошибками.
	* Решение: использовать Windows 7
2. Не регулируется подсветка в Windows XP.
	* Решение: возможно поможет правка реестра
3. В Lubuntu нету звука из-за ошибки в настройках.
	* Решение: поправить файл конфигурации
4. Если заряд батареи дойдет до нуля даже на версии BIOS F.48 потом будет показывать не правильный заряд.
	* Решение: переустановить обновление BIOS.
5. После Windows систем могут быть проблемы с переключением Wi-Fi, тачпада и других устройств в Ubuntu.
	* Решение: сделать сброс настроек BIOS.
6. Аппаратное ускорение видео плохо работает в браузере Firefox.
	* Решение: использовать Google Chrome или Chromium
7. По умолчанию в Windows 7 включено "пассивное охлаждение". Что сильно замедляет куллер и ноутбук перегревается.
	* Решение: в настройках питания Windows 7 поставить "активное охлаждение"
