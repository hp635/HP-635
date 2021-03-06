- [О разделе HP 635 ноутбук клуб (laptop hp 635 club)](#О-разделе-hp-635-ноутбук-клуб-laptop-hp-635-club)
- [Характеристики (могут различаться в разных моделях)](#Характеристики-могут-различаться-в-разных-моделях)
- [Какие операционные системы идут на HP 635?](#Какие-операционные-системы-идут-на-hp-635)
- [Какую операционную систему выбрать и почему?](#Какую-операционную-систему-выбрать-и-почему)
- [Какие игры идут?](#Какие-игры-идут)
- [Какие драйвера установить на Windows 7 SP1 x64?](#Какие-драйвера-установить-на-windows-7-sp1-x64)
- [Последовательность установки системы и драйверов на HP 635](#Последовательность-установки-системы-и-драйверов-на-hp-635)
- [Настройка Windows 7 для HP 635](#Настройка-windows-7-для-hp-635)
- [Настройка Ubuntu/LinuxMint](#Настройка-ubuntulinuxmint)
- [Известные проблемы ноутбука HP 635](#Известные-проблемы-ноутбука-hp-635)
- [Разборка ноутбука, замена деталей, чистка](#Разборка-ноутбука-замена-деталей-чистка)
- [Про возгорание батареи HP 635 (не волнуйтесь сразу! читайте)](#Про-возгорание-батареи-hp-635-не-волнуйтесь-сразу-читайте)

# О разделе HP 635 ноутбук клуб (laptop hp 635 club)

Тема про ноубук HP 635 (hp635), обсуждения, советы, клуб владельцев.  
Эта страница только для старых владельцев ноутбука HP 635, **покупать не рекомендую** (только если по дешевке)!

**Обсуждение:** в раздел [Issues](https://github.com/hp635/readme/issues)

**Обновление от 28.01.2019 :** Шел 2019 год, а ноутбук по прежнему живой. По сравнению с современными моделями главные недостатки: **заметно греется** в жару, сильно шумит и **относительно медленно работает**.

**Важно, про замедленне на всех современных операционных системах.** За время с прошлого обновления статьи нашли уязвимости в CPU, через них могут похитить пароли через порограммы работающие с сетью. Уязвимости называются **Spectre** и **Meltdown**. Для **Windows 7-10** и **Linux** вышли обновления в которых эта уязвимость устраняется путем отключения ускоряющих функцию ноутбука.  
**Результат:** все системы, которые вы установите и обновите будут работать медленнее. Уровень снижения производительности точно не описан в статьях, примерно 1-5% снижения производительности CPU. Но CPU этого ноутбука и так медленный, поэтому неясно как это может повлиять на некоторые задачи. Все рекомендации по этому поводу ниже в статье.

**Примечание:** В этой статье много мест, где я пишу, что **Windows 7** намного быстрее любой системы **Linux**, как ее не настраивай. Это верно для **ПРАВИЛЬНО** настроенной Windows 7, где вы отключили лишние сервисы, установили последние версии рекомендуемых мной драйверов и не устанавливали замедляющих систему программ.

# Характеристики (могут различаться в разных моделях)

**Процессор:** 2-ух ядерный APU 1.3 ГГц (AMD E-300, Zacate, не съемный)  
**Оперативная память:** 4 ГБ (часто модели бывают с 2 Гб, как правило в этой модели 2 слота, можно докупить еще 2 Гб)  
**Видеокарта:** AMD HD 6310 M (интегрированна в APU)  
<sub>**Примечание:** Модели HP 635 могут различаться. Например чаще всего стоит 2-ух ядерный процессор APU 1.6 ГГц</sub>

# Какие операционные системы идут на HP 635?

* Windows 7 SP1 x64 (**рекомендуется**) - после установки отключите сбор статистики замедляющий работу
	* <sub>установите [этот](http://download.windowsupdate.com/d/msdownload/update/software/updt/2016/05/windows6.1-kb3125574-v4-x64_2dafb1d203c8964239af3048b5dd4b1264cd93b9.msu) комулятивный пакет обновлений (перед этим установите [3020369](https://support.microsoft.com/en-us/kb/3020369) для исправления ошибок установки). Затем отключите сбор статистики, чтобы не отнимала производительность, инструкции: [1](http://www.overclock.net/t/1587577/windows-7-updates-list-descriptions-windows-7-8-telemetry-preparation), [2](http://techne.alaya.net/?p=12499), [3](http://www.dslreports.com/forum/r30348398-WIN7-Win-7-updates-to-avoid-or-be-careful-with) (прочитайте каждую и выполните, возможно позже скину готовый скрипт)</sub>
* Windows 7 SP1 x32 (**рекомендуется, если мало оперативной памяти**) - аналогично Windows 7 SP1 x64, но занимает меньше оперативной памяти. Если у вас 2 Гб или меньше, то можете попробовать ее. **Проблема:** работает медленнее чем x64, не работают некоторые программы, которые есть только под x64 версию.
* Windows XP - **проблема:** нету регуляции подсветки  
* Windows 10 - **проблема:** съедает драгоценную производительность на этом слабом ноутбуке  
* Ubuntu/LinuxMint (mate или xfce) - **проблема:** ноутбук сильнее греется, видео карта работает медленнее, могут быть помехи в колонках, без фирменной технологии Ultra Bass звук может быть хуже чем на Windows (возможно настройка эквалайзера поможет это исправить). В целом работает медленнее чем Windows, как ни настраивай и какие патчи на ядро linux не ставь
* Ubuntu/LinuxMint (kde, cinnamon и другие) - **проблема:** будет тормозить или имеют баги, эти системы активно используют GPU для эффектов и сильнее грузят CPU

# Какую операционную систему выбрать и почему?

**Ставьте Windows 7 SP1 x64. Все остальное у вас будет дико тормозить. Никакие компиляции ядра linux с ускоряющими патчами, установленные особые дистрибутивы linux (напр. Manjaro или Lubuntu) и прочее вам не помогут. Не тратьте время на эксперименты.** Бедным не выбирать. **(-:**

Если у вас мало оперативной памяти установите Windows 7 SP1 x32, можете даже поставить 2-ве системы одновременно и перезагружаться между ними.

Можете поставить 3-ей системой Ubuntu/LinuxMint и использовать ее для работы, а Windows 7 для игр и тяжелых программ. Но я бы рекомендовал просто использовать Windows 7 единственной системой. На этом ноутбуке действительно трудно пользоваться Linux системами из-за тормозов.

# Какие игры идут?

* **The Elder Scrolls 5: Skyrim**
  * Есть две версии Skyrim. Первая, 32-ух битная называется **Legendary Edition** и в теории работает быстрее, но она более старая и возможно для нее не будет обновлений. И вторая 64-ех битная **Special Edition**, с исправлениями, дополнительными эффектами и анимациями, она в теории будет работать медленнее.
* **Dota 2**
* **Far Cry 3** (и **Blood Dragon**)
* **Dishonored 1**
* **BioShock Infinity**
* **Mass Effect 3**

<sub>**Примечание:** Это самые "тяжелые" игры, верхняя планка. Игры более требовательные уже могут не запустится.</sub>

# Какие драйвера установить на Windows 7 SP1 x64?

1. С [сайта HP](https://support.hp.com/by-ru/drivers/selfservice/hp-635-notebook-pc/5086719) установите <sub>(список может отличаться для вашей модели)</sub>:
   1. Atheros 2011 Wireless LAN Driver
   2. Realtek Local Area Network (LAN) Driver
   3. Atheros Bluetooth Driver
   4. Realtek Card Reader Driver
   5. Synaptics Touchpad Driver - родной драйвер может быть лучше более новых неродных версий
2. С сайта AMD
   1. [Catalyst Software Suite 15.7.1](https://www.amd.com/en/support/apu/amd-e-series-processors/amd-dual-core-processor-e-300/e-300-radeon-hd-6310) или [Crimson Edition 16.2.1 Beta](https://www.amd.com/en/support/apu/amd-e-series-processors/amd-dual-core-processor-e-300/e-300-radeon-hd-6310)
   2. AMD Chipset Drivers - драйвер чипсета на сайте HP более старый <sub>к сожалению AMD изменила дизайн своего сайта, поэтому найти подходящую версию драйвера я пока не смог :)</sub>
   3. AMD RAIDXpert Utility - эта утилита не очень нужна, если у вас нет RAID
3. С [сайта realtek](https://www.realtek.com)
   1. [High Definition Audio Codecs](https://www.realtek.com/en/component/zoo/category/pc-audio-codecs-high-definition-audio-codecs-software)
4. С сайта synaptics <sub>(раньше последние версии драйвера можно было найти на этом сайте, теперь ссылки убрали, возможно где-то они остались и их можно найти поиском)</sub>
   1. Synaptics Touchpad Driver - на выбор, вы можете найти более новые драйвера с сайта synaptics, но есть вероятность, что они будут хуже тех что на сайте HP

**Примечание 1:** Windows 7 через систему обновления может предлагать установить драйвер (в дополнительных компонентах). Не устанавливайте их, они проблемные.

**Примечание 2:** [Crimson Edition 16.2.1 Beta](https://www.amd.com/en/support/apu/amd-e-series-processors/amd-dual-core-processor-e-300/e-300-radeon-hd-6310) видео драйвер для Windows не имеет OpenCL, но субьективно чуть быстрее других версий. Советую его. Есть [неофициальный способ добавления OpenCL](https://forum.radeon.ru/viewtopic.php?p=918761#p918761) в этот видео драйвер.

**Примечание 3:** С выходом Windows 10 началась мода не давать ссылки на самые новые версии драйверов на сайтах производителей оборудования. Рекомендуют или драйвера с сайта HP, или те что загрузит сама Windows 10 (которая не всегда загружает то, что нужно и не всегда драйвера новые). Поэтому лучше сохраняйте драйвера так, чтобы они у вас остались.

# Последовательность установки системы и драйверов на HP 635

1. Запишите на флэшку [Xubuntu](http://xubuntu.org/getxubuntu/) через программу [UNetbootin](https://unetbootin.github.io/), загрузитесь с неё и разметьте диск через программу **GParted** (может находиться в настройках системы и иметь другое название) <sub>**Не используйте разметку диска в Windows 7, могут быть проблемы**</sub>
2. [Rufus](https://rufus.akeo.ie/) - программа для записи Windows 7 на флэшку и установки Windows 7 с неё <sub>**во время включения компьютера нажмите F9 чтобы выбрать с какого устройства загрузиться, загрузитесь с флэшки**</sub>
3. Установите все драйвера из раздела [Какие драйвера установить на Windows 7 SP1 x64?](https://github.com/hp635/HP-635#%D0%9A%D0%B0%D0%BA%D0%B8%D0%B5-%D0%B4%D1%80%D0%B0%D0%B9%D0%B2%D0%B5%D1%80%D0%B0-%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%B8%D1%82%D1%8C-%D0%BD%D0%B0-windows-7-sp1-x64) этой статьи
4. Если пакет исправлений SP1 для Windows 7 не установлен, то установите его через обновление системы в "Панель управления"
5. Установите пакет исправлений [3020369](https://support.microsoft.com/en-us/kb/3020369) - он понадобится для дальнейшей установки обновлений
6. Установите [kb3125574](http://download.windowsupdate.com/d/msdownload/update/software/updt/2016/05/windows6.1-kb3125574-v4-x64_2dafb1d203c8964239af3048b5dd4b1264cd93b9.msu) - коммулятивный пакет обновлений, это сборка всех обновлений для Windows 7 SP1 до лета 2016 года
7. Установите обновление для производительности видео: [Platform Update for Windows 7](https://www.microsoft.com/en-us/download/details.aspx?id=36805)
8. Посмотрите в раздел [Известные проблемы ноутбука HP 635](https://github.com/hp635/HP-635#%D0%98%D0%B7%D0%B2%D0%B5%D1%81%D1%82%D0%BD%D1%8B%D0%B5-%D0%BF%D1%80%D0%BE%D0%B1%D0%BB%D0%B5%D0%BC%D1%8B-%D0%BD%D0%BE%D1%83%D1%82%D0%B1%D1%83%D0%BA%D0%B0-hp-635) этой статьи и исправьте, что посчитаете нужным
9.  Обновите Windows 7 через стандартную функцию обновления Windows 7, стабильность в итоге возрастет.
10. После установки Window 7 установите второй системой [Xubuntu](http://xubuntu.org/getxubuntu/), как резервную

<sub>**Примечание 1:** Чтобы настройки каждый раз не сбивались при переустановки Windows вы можете использовать портативные программы [PortableApps.com](http://portableapps.com/download)</sub>

**Примечание 2:** Когда поддержка Windows 7 закончится придется искать неофициальные пакеты обновлений или способ подключиться к обновлениям для коммерческих версий с длительным сроком поддержки. Чем раньше вы "запасетесь" Windows 7, тем проще для вас.

# Настройка Windows 7 для HP 635

1. В настройках драйвера AMD придется поставить максимальную производительность, чтобы всё работало нормально. Отключите все эффекты какие можете. В настройках игр отключайте "вертикальную синхронизацию"
2. Старайтесь использовать DirectX 9 вместо DirectX 10, 11 или OpenGL. Во многих играх запуск DirectX 9 делается коммандой -dx9
3. Не устанавливайте никакой антивирус, они сильно замедляют систему! Отключите Defender в настройках системы (встроенный антивирус) и отключите фаервол. Если вы не будете устанавливать зараженные программы риск заражения минимален.
4. В Windows 7 по умолчанию включена авто загрузка программ со вставленной флэшки, отключите это или заразите систему.

# Настройка Ubuntu/LinuxMint

**Что вам нужно знать:** Linux всегда будет медленнее чем Windows 7 на этом ноутбуке, если Windows 7 правильно настроена и отключены лишние процессы и телеметрия.

Устанавливайте Ubuntu/LinuxMint с mate (удобнее) или xfce (быстрее). Все остальное у вас будет тормозить.

После установки:
1. Включите BFQ, иначе копирование большого количества мелких файлов на медленные диски будет тормозить. BFQ еще и ускоряет систему. Инструкция [тут](https://unix.stackexchange.com/questions/375600/how-to-enable-and-use-the-bfq-scheduler)
2. Зайдите в панель настроек, найдите там пункт **драйвера** и установите, если в списке драйверов что-то будет
3. Отключите все эффекты какие сможете. Кроме вертикальной синхронизации рабочего стола, иначе будет tearing в видео (разрывы). В xfce давняя проблема с tearing, поэтому тут mate лучше.
4. Попробуйте видеодрайвера из репозиториев. Можно установить одновременно только один из них:
   1. XSWAT (официальный, относительно стабилен)
   2. Oibaf (неофициален, нестабилен)
   3. Padoka (неофициален, нестабилен)
5. Поиграйтесь с установкой pf-kernel патчей на ядро, возможено будет какое-то ускорение работы

# Известные проблемы ноутбука HP 635

1. В системах Linux странное дребезжание звука. Видимо от того, что драйвер звука с ошибками.
	* **Решение:** использовать Windows 7.
2. Не регулируется подсветка в Windows XP.
	* **Решение:** возможно поможет правка реестра, встречал в сети инструкцию для другого ноутбука, но не проверял.
3. В Lubuntu нету звука из-за ошибки в настройках.
	* **Решение:** поправить файл конфигурации.
4. Если заряд батареи дойдет до нуля даже на версии BIOS F.48 потом будет показывать не правильный заряд.
	* **Решение:** переустановить обновление BIOS.
5. После Windows систем могут быть проблемы с переключением Wi-Fi, тачпада и других устройств в Ubuntu.
	* **Решение:** сделать сброс настроек BIOS.
6. Аппаратное ускорение видео плохо работает в браузере Firefox.
	* **Решение:** использовать Google Chrome или Chromium.
7. По умолчанию в Windows 7 включено "пассивное охлаждение". Что сильно замедляет куллер и ноутбук перегревается.
	* **Решение:** в настройках питания Windows 7 поставить "активное охлаждение".
8. AMD не доделала новые драйвера серии Crimson (доступна только beta версия) для видеокарты AMD HD 6310 M. Поддержка OpenCL в этих недоделанных драйверах сломана. Но в интернете есть инструкция о том, как перенести библиотеки OpenCL из старых драйверов в эту beta версию драйвера.
9. Звук в наушниках может пищать или иметь помехи. Причина скорее всего в проблемах с конструкцией и отсутствии изоляции помех. Может быть причина в драйверах.
	* **Решение:** нету
10. В некоторых играх звук может хрипеть. Причина неизвестна.
	* **Решение:** нету
11. Новые модели ноутбуков HP получили обновление BIOS, исправления багов Spectre и Meltdown работают в паре с BIOS. HP 635 таких исправлений не получил, насколько это снизило производительность или защиты неясно.
    * **Решение:** нету

# Разборка ноутбука, замена деталей, чистка

**Разборка.** Посмотреть как разбирается ноутбук HP 635 можно на youtube: [HP 635](https://www.youtube.com/results?search_query=hp+635), [HP 635](https://www.youtube.com/results?search_query=hp+625) (hp 625 разбирается так же, как и hp 635). Главная сложность это не сломать заклепки по краям ноутбука при разъединении верхней и нижней частей корпуса. И не задеть провода внутри ноутбука, они очень тонкие и их легко повредить.

**Чистка.** В этой модели при нормальном использовании скапливается очень мало пыли. Но если будут проблемы с перегревом всё же откройте и проверьте (хотя мой даже чистым греется сильно).

**Чистка монитора.** Протирайте влажными салфетками для рук без спирта. Спирт может попасть под антибликовые слои покрытия дисплея и они могут слипнуться. Получите белые пятна в местах слипания. Слипнуться антибликовые слои могут от сильного надавливания на дисплей или других жидкостей. Если слипнутся от воды, со временем она может испариться и слипания исчезнут.

**Белые пятна на дисплее (слипшиеся антибликовые слои).** Если между слоями антибликового покрытия ноутбука попала жидкость или испарения (напр. пары спирта). То слои могут слипнуться и на месте слипания появятся белые пятна. Исправить это можно чисткой. Для этого нужно разобрать ноутбук, снять дисплей, **аккуратно** снять антибликовые слои с него, промыть их и вернуть на место. Я **не гарантирую работоспособность этого способа** (сам не пробовал). На youtube вы можете найти различные ролики по этой теме.

**Замена клавиатуры.** Я заменял только клавиатуру. Клавиатуру можно найти по запросу [hp 635 keyboard](http://www.aliexpress.com/popular/hp-635-keyboard.html). В местных магазинах она как правило тоже продается, наценка не сильно выше чем в китайских магазинах и на ebay. Заменяется очень легко. Главное быть аккуратным и не повредить шину (провод которым соединяется клавиатура).

**Заменя дисплея.** Не пробовал, но на youtube есть ролики, где это делают. Главная проблема судя по роликам это подобрать дисплей с подходящей шиной (проводом которым дисплей подключается к ноутбуку).

# Про возгорание батареи HP 635 (не волнуйтесь сразу! читайте)

У HP некоторые батареи подвержены возгоранию. С их сайта можно скачать утилиту для Windows, которая проверит батарею и скажет вам результат. Если батарея окажется подверженной возгоранию, они беспалтно заменят ее на хорошую. У моего HP 635 с ней все ОК, она подходила под текстовое описание, но утилита сказала, что все ОК. Я уточнил по email у HP и они подтвердили, что все ОК. Это не значит, что для вашего HP 635 все тоже в порядке!