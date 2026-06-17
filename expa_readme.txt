

    _______________  _____________  _____   
    \_   _____/\   \/  /\______   \/  _  \  	  Expa_Urus Ver...: 1.3 	
     |    __/_  \     /  |     ___/  /_\  \ 	  Last Release....: 17.06.26
     |        \ /     \  |    |  /    |    \	  Dependencies....: RD-2.5.4; expa_xray_cross.xml 
    /_______  //___/\  \ |____|  \____|__  /	  Feedback........: xiodexter@gmail.com 
      Urus  \/       \_/  Realdash Skin  \/		

	
	[РУС]
		 
	1\. УПРАВЛЕНИЕ СКИНОМ (кнопки подрулевого переключателя: ▲ - верхняя, ▼ - нижняя)

    1.1 Одиночные нажатия кнопок ▲ \ ▼ или нажатие по верхним вкладкам — Перемещение по вкладкам пунктов меню, цикличное;
    1.2 Нажатие ▲ + ▼ во вкладке меню Cam (фотоаппарат) — Включает режим контроля слепых зон от поворотника;
    1.3 Нажатие ▲ + ▼ во вкладке меню Car (авто) или нажатие по иконке с покрышкой — Показать\Спрятать датчики TPMS Deelife;
    1.4 Нажатие ▲ + ▼ во вкладке меню Trip (флаг) или нажатие по соответст. суб-вкладке или иконке возле одометра — Переключение TripA\TripB;
    1.5 Нажатие ▲ + ▼ во вкладке меню Rate (канистра) или нажатие по соответст. суб-вкладке — Переключение расхода L/100 или L/H;
    1.6 Нажатие ▲ + ▼ во вкладке меню Navi (глобус) — Запуск приложения ru.yandex.yandexnavi;
    1.7 Нажатие ▲ + ▼ во вкладке меню Setup (шестеренка) или нажатие по соответст. суб-вкладке — Переключение вкладок пресетов цвета шкал;
    1.8 Рычаг поворотника в пункте меню Cam - Если не включен режим слепых зон (см. 1.2), то поворотник переключает камеру (левая\правая) в области меню;
    1.9 Нажатие по крыше авто во вкладке меню Car — Показать\Спрятать поперечины Turtle Air 2;
    1.10 Удержание кнопки ▼ более 5 сек или нажатие по иконке круговой стрелки вкладки Trip — Сброс TripA или TripB (соответст. вкладка см. 1.4);
    1.11 Нажатие по иконке круговой стрелки во вкладке Rate — Сброс сервисного интервала и моточасов;
    1.12 Нажатие по заголовку Fuel Consumption во вкладке Rate — Переключение источника расчетов мгновенного расхода (CAN или RD);  
    1.13 Удержание ▲ более 2 сек или нажатие по схеме переключения МКПП — Переключение отображения шкал Anima: Corsa(гонка)\Strada(улица); 
    1.14 Удержание ▼ более 2 сек или нажатие по иконке аккумулятора — Переключение отображения уровня топлива и температуры двигателя (Bars\Orbs);
    1.15 Удержание ▲ более 5 сек — Переключение на следующий скин в комбайне (Next Page);
    1.16 Нажатие по мини-иконке андроид — Показать\Спрятать зону-лаунчера (ярлыки перехода на следующий скин, запуск приложений и настроек андроида);
    1.17 Нажатие по мини-иконке жука — Показать\Спрятать зону баг-отладки (2 текстовых поля, 2 кнопки и 2 слайдера для трассировки значений);
    1.18 Нажатие по палитре вкладки Setup - Выбор цвета в соответст. суб-вкладке пресетов (4 группы по 7 цветов), иконка круговой стрелки - тестовый взмах;
    1.19 Все из вышеперечисленного можно активировать во вкладке меню Setup нажатием на соответствующий андроидный переключатель;
    

    2\. НЕОЧЕВИДНЫЕ МОМЕНТЫ СКИНА       
 
    2.1 Скин использует свой файл CAN-описания expa_xray_cross.xml. Некоторые параметры считаются без триггеров сразу в xml, поэтому в симуляции могут отображаться некорректно. Для правильной работы нужно также удалить все глобальные триггеры, т.к. возможно будет переопределение переменных от Indash (Settings - Apications - Global Triggers & Actions). На версиях Realdash свежее v2.54 скин не тестировался; 
    2.2 Неважно в каком состоянии сохранен скин после редактирования, в момент его загрузки срабатывают триггеры инициализации на основе считанных параметров из Dash Data (используются все 20шт.), все эти параметры можно изменить и на вкладке Setup, также сохраняются выбранные пресеты цветов на все 4-ре группы шкал и последняя выбранная вкладка основного меню;
    2.3 В файле описания принципиально не используются теги ECU Specific. Для параметров, которым не нашелся свой описательный идентификатор, - сверху файла список имен переопределённых зарезервированных тегов;
    2.4 Если время системы абсурдно (нет интернета, GPS-глушилки или взята дата прошивки) показывается иконка "Нет сигнала" (триггер сравнивает даты в Unix формате);
    2.5 Один из двух звуков проигрывания заставки выбирается псевдослучайно в зависимости от вольтажа (по последнему биту, определяющему четность числа см. ID322), звук активации вкладок также псевдорандомный; 
    2.6 У режимов Corsa\Strada различные звуки поворотников и после 4-ой итерации становится боле тихими, это сделано для комфортного, длительного ожидания на перекрестке;
    2.7 Показания наружной температуры откалиброваны сторонним термометром и зависимость там не линейная (см. ID174 в файле описания);
    2.8 Чтобы избежать перегруженности скина, некоторые элементы показываются только на определенном событии, например, пропадает иконка покрышки на скорости более 4км/ч и пр.;
    2.9 Многие сигнальные лампы имеют два состояния, второе - с восклицательным знаком или черепом, например, появляется на лампе не пристегнутого ремня если скорость превысила 6 км/ч;
    2.10 Размер шлейфа с шестигранниками за стрелками спидометра\тахометра зависит от положения педали акселератора, размер считается сразу в файле CAN-описания (см. ID287), шлейф торможения на противоположной стороне стрелки;
    2.11 Размер шрифта трехзначного значения скорости автоматически уменьшается, чтобы не перекрывать шкалы. Движение значений литража топлива и температуры охл.жидкости выполнены через анимацию value-morph, появившейся в версии Realdash 2.47;
    2.12 Регулировка яркости экрана сделана не через Screen Brightness (из-за проблемной прошивки часто слетало), а через черный, вуальный прямоугольник, меняющий прозрачность в зависимости от состояния габаритов;
    2.13 Замер разгона до 60 км/ч отображается в Сurrent Trip и виден только если активен TripB (см. 1.4), таймер стартует в начале движения, сбрасывается на следующем старте после остановки, задник краснеет по достижению скорости;
    2.14 При повороте ключа в ACC или OFF включается 10-секундный обратный отсчет до выключения, подкорректировать под свое время, выставленное в андроиде, можно через Gauge Math счетчика. В Fyt-настройках время задается параметром Delay Power Off When ACC Off;
	

	[EN] 

 	1\. SKIN CONTROL (steering wheel switch buttons: ▲ - top, ▼ - bottom)

	1.1 Single keystrokes ▲ \ ▼ or clicking on the top tabs — Moving through the menu items tabs, cyclical;
	1.2 Pressing ▲ + ▼ in the Cam menu tab (camera) — Turns on the blind spot monitoring mode from the turn signal;
	1.3 Pressing ▲ + ▼ in the Car menu tab (auto) menu item or clicking on the tire icon — Show\Hide TPMS Deelife Sensors;
	1.4 Pressing ▲ + ▼ in the Trip menu tab (flag) or clicking on the corresponding sub-tab or icon near the odometer — Switching TripA\TripB;
	1.5 Pressing ▲ + ▼ in the Rate menu tab (canister) or clicking on the corresponding sub-tab — Flow rate switching L/100 or L/H;
	1.6 Pressing ▲ + ▼ in the Navi menu tab (globe) - Launching the app ru.yandex.yandexnavi;
	1.7 Pressing ▲ + ▼ in the Setup menu tab (gear) or pressing the corresponding sub-tab — Switching tabs of scale color presets;
	1.8 Turn signal lever in the Cam menu item - If blind spot mode is not enabled (see 1.2), the turn signal switches the camera (left/right) in the menu area;
	1.9 Mouse click on the roof of a car in the Car menu tab — Show\Hide the Turtle Air 2 Crossbars;
	1.10 Keep ▼ button pressed more than 5 seconds or clicking on the circular arrow icon of the Trip tab — Reset TripA or TripB (respectively tab see 1.4);
	1.11 Clicking on the circular arrow icon in the Rate tab — Resets the service interval and motohours;
	1.12 Сlicking on the Fuel Consumption heading in the Rate tab — Switches the source of instant consumption calculations (CAN or RD);
	1.13 Keep ▲ button pressed more than 2 seconds or clicking on the manual transmission scheme — Switching the display of scales Anima: Corsa(race)\Strada(street); 
	1.14 Keep ▼ button pressed more than 2 seconds or clicking on the battery icon — Switches the display of fuel level and engine temperature (Bars\Orbs);
	1.15 Keep ▲ button pressed more than 5 seconds — Switch to the next skin in the Сombine (Next Page);
	1.16 Clicking on the android mini-icon — Show\Hide the Launcher area (shortcuts for switching to the next skin, launching applications and android settings);
	1.17 Clicking on the mini-bag icon — Show\Hide the bug debugging zone (2 text fields, 2 buttons and 2 slider for tracing values);
	1.18 Clicking on the palette of the Setup tab - Selecting the color a sub-tab of presets (4 groups of 7 colors each), the circular arrow icon is a test swipe;
	1.19 All of the above can be activated in the Setup menu tab by clicking on the corresponding android switch;

	
	2\. NON-OBLIVIOUS SKIN POINTS

	2.1 The skin uses its own CAN-description file expa_xray_cross.xml. Some parameters are considered immediately in xml without triggers, so they may not be displayed correctly in the simulation. For proper operation, you also need to remove all global triggers, because it will be possible to redefine variables from Indash (Settings - Applications - Global Triggers & Actions). The skin has not been tested on versions of Realdash newer than v2.54;
	2.2 It does not matter in what state the skin is saved after editing, initialization triggers are triggered at the time of loading based on the read parameters from Dash Data (all 20 pcs are used), all these parameters can be changed on the Setup tab, the selected color presets for all 4 scale groups and the last selected tab of the main menu are also saved;
	2.3 ECU Specific tags are not used in the description file in principle. For parameters that do not have their own descriptive identifier, there is a list of names of redefined reserved tags at the top of the file;
	2.4 If the system time is absurd (there is no Internet, GPS jammers, or the firmware date is taken), the "No signal" icon is displayed (the trigger compares dates in Unix format);
	2.5 One of the two screen saver playback sounds is selected pseudorandomly depending on the voltage (according to the last bit that determines the parity of the number, see ID322), the sound of tab activation is also pseudorandom;
	2.6 Corsa\Strada modes have different turn signal sounds and become quieter after the 4th iteration, this is done for a comfortable, long wait at the intersection;
	2.7 The outdoor temperature readings are calibrated by a third-party thermometer and the dependence there is not linear (see ID174 in the description file);
	2.8 To avoid overloading the skin, some elements are shown only at a certain event, for example, the tire icon disappears at a speed of more than 4 km/h, etc.;
	2.9 Many warning lights have two states, the second one with an exclamation mark or a skull, for example, appears on the lamp of an unbuckled seat belt if the speed exceeds 6 km/h;
	2.10 The size of the hexagon loop behind the speedometer/tachometer arrows depends on the position of the accelerator pedal, the size is calculated immediately in the CAN description file (see ID287), the braking loop is on the opposite side of the arrow;
	2.11 The font size of the three-digit speed value is automatically reduced so as not to overlap the scales. Movement of the values of the litre of fuel and the cooling temperature. The liquids are made through the value-morph animation introduced in Realdash 2.47;
	2.12 Screen brightness adjustment is done not through Screen Brightness (due to problematic firmware, it often flew off), but through a black, veiled rectangle that changes transparency depending on the state of the dimensions;	
	2.13 Acceleration to 60 km/h is displayed in the Current Trip and is visible only if TripB is active (see 1.4), the timer starts at the beginning of the movement, resets at the next start after stopping, the backdrop turns red when the speed is reached;
	2.14 When you turn the key to ACC or OFF, a 10-second countdown is turned on before switching off, you can adjust the time set in android using the meter's Gauge Math. In the Fyt settings, the time is set by the "Delay Power Off When ACC Off" parameter;
