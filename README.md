# О разделе HP 635 ноутбук клуб (laptop hp 635 club)

Тема про ноубук HP 635 (hp635), обсуждения, советы, клуб владельцев.  
Эта страница только для старых владельцев ноутбука HP 635, **покупать не рекомендую** (только если б. у. по дешевке)!

**Обсуждение:** в раздел [Issues](https://github.com/hp635/readme/issues)

# Характеристики (могут различаться в разных моделях)

**Процессор:** APU 1.3 ГГц (AMD E-300, Zacate, не съемный)  
**Оперативная память:** 4 ГБ  
**Видеокарта:** AMD HD 6310 M (интегрированна в APU)

<sub>**Примечание:** Модели HP 635 могут различаться. Например чаще всего стоит процессор APU 1.6 ГГц</sub>

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

<sub>**Примечание:** Это самые "тяжелые" игры, верхняя планка. Игры более требовательные уже могут не запустится.</sub>

# Какие драйвера установить на Windows 7 SP1 x64?

1. Драйвера [на сайте HP](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061)
	1. [Atheros 2011 Wireless LAN Driver](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - драйвер Wi-Fi
	2. [Realtek Local Area Network (LAN) Driver](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - драйвер для сетевой карты
	3. [Atheros Bluetooth Driver](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - драйвет Bluetooth
	4. [Realtek Card Reader Driver](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - драйвер для Card Reader, SD карточек
2. Драйвер для видеокарты [Catalyst Software Suite 15.7.1](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1)
3. Драйвер для чипсета [AMD Chipset Drivers](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1) - в разделе Optional Downloads (опциональные загрузки)
4. Драйвер RAID [AMD RAIDXpert Utility](http://support.amd.com/ru-ru/download/desktop/previous/detail?os=Windows%207%20-%2064&rev=15.7.1) - в разделе Optional Downloads (опциональные загрузки)
5. Realtek [High Definition Audio Codecs](http://www.realtek.com.tw/downloads/) - драйвер для звука
6. [Драйвер сенсорной панели Synaptics](http://www.synaptics.com/resources)
7. [HP Notebook System BIOS Update (AMD Processors)](http://h20566.www2.hp.com/hpsc/swd/public/readIndex?sp4ts.oid=5086720&swLangOid=8&swEnvOid=4061) - BIOS версии F.48

# Последовательность установки системы и драйверов на HP 635

0. Запишите на флэшку [Xubuntu](http://xubuntu.org/getxubuntu/) через программу [UNetbootin](https://unetbootin.github.io/), загрузитесь с неё и разметьте диск через программу GParted (может находиться в настройка системы и иметь другое название) <sub>**Не используйте разметку диска в Windows 7, могут быть проблемы**</sub>
1. Скачать [Windows 7 x64 Enterprise Eval](http://care.dlservice.microsoft.com/dl/download/evalx/win7/x64/EN/7600.16385.090713-1255_x64fre_enterprise_en-us_EVAL_Eval_Enterprise-GRMCENXEVAL_EN_DVD.iso) - это Windows 7 с бесплатным пробным периодом после бесплатной активации через интернет в течении 180 дней, плюс пробный период можно продлить три раза командой ```slmgr -rearm```
2. [Rufus](https://rufus.akeo.ie/) - программа для записи Windows 7 на флэшку и установки Windows 7 с неё <sub>**во время включения компьютера нажмите F9 чтобы выбрать с какого устройства загрузиться, загрузитесь в флэшки**</sub>
3. Установите все драйвера из раздела [Какие драйвера установить на Windows 7 SP1 x64?](https://github.com/hp635/HP-635#%D0%9A%D0%B0%D0%BA%D0%B8%D0%B5-%D0%B4%D1%80%D0%B0%D0%B9%D0%B2%D0%B5%D1%80%D0%B0-%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D1%82%D1%8C-%D0%BD%D0%B0-windows-7-sp1-x64) этой статьи
4. Установите пакет исправлений SP1 для Windows 7 через обновление системы в "Панель управления"
5. Установите пакет исправлений [3020369](https://support.microsoft.com/en-us/kb/3020369) - он понадобится для дальнейшей установки обновление
6. Установите [kb3125574](http://download.windowsupdate.com/d/msdownload/update/software/updt/2016/05/windows6.1-kb3125574-v4-x64_2dafb1d203c8964239af3048b5dd4b1264cd93b9.msu) - коммулятивный пакет обновлений, это сборка всех обновлений для Windows 7 SP1 до лета 2016 года
7. Посмотрите в раздел [Известные проблемы ноутбука HP 635](https://github.com/hp635/HP-635#%D0%98%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D1%8B%D0%B5-%D0%BF%D1%80%D0%BE%D0%B1%D0%BB%D0%B5%D0%BC%D1%8B-%D0%BD%D0%BE%D1%83%D1%82%D0%B1%D1%83%D0%BA%D0%B0-hp-635) этой статьи и исправьте, что посчитаете нужным
8. После установки Window 7 установите второй системой [Xubuntu](http://xubuntu.org/getxubuntu/), как резервную

<sub>**Примечание:** Чтобы настройки каждый раз не сбивались при переустановки Windows вы можете использовать портативные программы [PortableApps.com](http://portableapps.com/download)</sub>

# Известные проблемы ноутбука HP 635

1. В системах Linux странное дребезжание колонок. Видимо от того, что драйвер звука с ошибками.
	* **Решение:** использовать Windows 7
2. Не регулируется подсветка в Windows XP.
	* **Решение:** возможно поможет правка реестра
3. В Lubuntu нету звука из-за ошибки в настройках.
	* **Решение:** поправить файл конфигурации
4. Если заряд батареи дойдет до нуля даже на версии BIOS F.48 потом будет показывать не правильный заряд.
	* **Решение:** переустановить обновление BIOS.
5. После Windows систем могут быть проблемы с переключением Wi-Fi, тачпада и других устройств в Ubuntu.
	* **Решение:** сделать сброс настроек BIOS.
6. Аппаратное ускорение видео плохо работает в браузере Firefox.
	* **Решение:** использовать Google Chrome или Chromium
7. По умолчанию в Windows 7 включено "пассивное охлаждение". Что сильно замедляет куллер и ноутбук перегревается.
	* **Решение:** в настройках питания Windows 7 поставить "активное охлаждение"

# Разборка ноутбука, замена деталей, чистка

**Разборка.** Посмотреть как разбирается ноутбук HP 635 можно на youtube: [HP 635](https://www.youtube.com/results?search_query=hp+635), [HP 635](https://www.youtube.com/results?search_query=hp+625) (hp 625 разбирается так же, как и hp 635)

**Чистка.** В этой модели при нормальном использовани скапливается мало очень мало пыли. Но если будут проблемы с перегревом всё же откройте и проверьте (хотя мой даже чистым греется сильно).

**Чистка монитора.** Протирайте влажными салфетками для рук без спирта.