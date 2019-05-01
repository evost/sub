# Подводное дело

0. [Пара таблиц вместо введения](#0-Пара-таблиц-вместо-введения)  
1. [Torpedo Data Computer (TDC)](#1-torpedo-data-computer-tdc)  
2. [Лодочные системы](#2-Лодочные-системы)  
    2.1 [Помпа](#21-Помпа)  
    2.2 [Компрессор](#22-Компрессор)  
    2.3 [Вентиля заполнения балласта](#23-Вентиля-заполнения-балласта)  
    2.4 [Вентиля балласта отрицательной плавучести](#24-Вентиля-балласта-отрицательной-плавучести)  
    2.5 [Вентиль продувки балласта](#25-Вентиль-продувки-балласта)  
    2.6 [Руль глубины](#26-Руль-глубины)  
    2.7 [Машинный телеграф](#27-Машинный-телеграф)  
    2.8 [Рулевая машинка](#28-Рулевая-машинка)  
    2.9 [Радио](#29-Радио)  
    2.10 [Энигма](#210-Энигма)  
    2.11 [Поисковик радиосигналов](#211-Поисковик-радиосигналов)  
    2.12 [Гидрофон](#212-Гидрофон)  
    2.13 [Проигрыватель](#213-Проигрыватель)  
3. [Управление лодкой](#3-Управление-лодкой)  
    3.1 [Порядок всплытия и погружения](#31-Порядок-всплытия-и-погружения)  
    3.2 [Управление режимами машин и руление](#32-Управление-режимами-машин-и-руление)  
    3.3 [Следование курсу по навигационным приборам](#33-Следование-курсу-по-навигационным-приборам)  
    3.4 [Порядок запуска торпед и ведение огня из палубных орудий](#34-Порядок-запуска-торпед-и-ведение-огня-из-палубных-орудий)  
4. [Определение скорости и курса цели по четырем пеленгам](#4-Определение-скорости-и-курса-цели-по-четырем-пеленгам)  
5. [Определение параметров цели с использованием перископа и справочника](#5-Определение-параметров-цели-с-использованием-перископа-и-справочника)  

***

> Подводная лодка, по существу, полностью орудие нападения.
>> Карл Дёниц

# 0. Пара таблиц вместо введения

[![](https://cdn.discordapp.com/attachments/572801769516695564/572861715172294693/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572861715172294693/unknown.png)

Дальность до цели по ее угловой величине вычисляется по формуле D = L / R, где D - дальность до цели в гектометрах, L - длинна/высота/ширина цели в метрах на синус курсового угла цели, R - угол, под которым видна цель (предмет), в сантирадианах (одно деление шкалы перископа при 1,5x = 1 сантирадиан = 10 тысячных = 0.01 радиан, одно деление шкалы перископа при 6x = 0.25 сантирадиан = 2.5 тысячных (результат больше чем при 1,5x в 4 раза), 1000 тысячных = 100 сантирадиан = 1 радиан).

Таблицы служат для вычисления расстояния до объекта по его известным размерам при разной крастности перископа. Например, по вертикали длинна корабля из справочника в метрах, умноженная на синус курсового угла цели, по горизонтали угловая величина - количество рисок на перископе в которые он укладывается: на пересечении будет расстояние до цели в гектометрах.

Логарифмическая шкала справа служит для нахождения одного неизвестного из скорости (уз), времени (мин) и расстояния (км) по двум другим - необходимо построить прямую по двум известным величинам, она будет пересекать искомое значенние на оставшейся шкале.

# 1. Torpedo Data Computer (TDC)

[![](https://cdn.discordapp.com/attachments/572801769516695564/572866047577686055/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572866047577686055/unknown.png)

1) Angle Tracking - выбор перископа для наведения и запуска:
    - A.P. - атакующий перископ;
    - O.P. - зенитный перископ;
    - UZO - прибор управления стрельбой;
    - Off - задание угла по которому видится цель вручную на панели Heading;
2) Target Speed - скорость цели в узлах;
3) Torpedo Depth - глубина на которой пойдет торпеда, чем ближе к килю, тем лучше;
4) Range - расстояние до цели в гектометрах;
5) Length - -
6) Gyro Angle - угол, на который довернет торпеда;
7) Spread Angle - угол разброса торпед при залпе;
8) Time To Impact - время хода торпеды до цели;
9) Angle On Bow - курсовой уголь цели (КУЦ). Угол, под которым наблюдается лодка с цели: 0 - цель идет на лодку, 180 - цель уходит от лодки, "право 90" - лодка справа от цели под прямым углом.
10) Impact Angle - угол удара торпеды, чем ближе к 90 тем лучше;
11) Лампа под IA - сигнализирует о невозможности попасть в цель при текущих настройках (цель слишком далеко или под сильным углом относительно торпедного аппарата);
12) Heading - угол, под которым цель наблюдается с лодки, активен, если AT в положении Off;
13) Torpedo Status - количество оставшихся торпед и их готовность (лампа горит - торпеда готова к запуску). Сверху - носовой аппарат, снизу - кормовой аппарат;
14) Single Shot - выбор торпедного аппарата / залпа (Salvo);
15) Salvo Shot - выбор батареи торпед для залпа, активен, если Single Shot в положении Salvo;

# 2. Лодочные системы

## 2.1 Помпа

Откачивает воду из обитаемых отсеков.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572866945691549727/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572866945691549727/unknown.png)

## 2.2 Компрессор

Накачивает воздух из атмосферы в баки.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572867053669580811/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572867053669580811/unknown.png)

## 2.3 Вентиля заполнения балластаных цистерн

Открывает и закрывает доступ воде к основным балластным цистернам. Для носовой и кормовой цистерны вентиля заполнения свои.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572867430251233300/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572867430251233300/unknown.png)

## 2.4 Вентиля цистерн быстрого погружения

Верхний вентиль - заполнение водой, нижний - продувка воздухом. Левый прибор - уровень воды в цистерне, правый - запас сжатого воздуха. 

[![](https://cdn.discordapp.com/attachments/572801769516695564/572867811064545290/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572867811064545290/unknown.png)

## 2.5 Вентиль продувки балластных цистерн

Центральный прибор - запас сжатого воздуха, боковые - количество воды в носовом и кормовом балластах. Продуваются для экстренного всплытия или для увеличения скорости надводного хода. 

[![](https://cdn.discordapp.com/attachments/572801769516695564/572868489862447124/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572868489862447124/unknown.png)

## 2.6 Управление рулем глубины

- Два верхних прибора - тахометры правой и левой машины;
- Слева - мелководный глубинометр;
- Справа - глубоководный глубинометр;
- Слева внизу - угол рулей подводной лодки;
- Справа внизу - -;
- По центру слева - глубинометр перископа;
- По центру справа - скорость погружения/всплытия;

[![](https://cdn.discordapp.com/attachments/572801769516695564/572869513083617281/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572869513083617281/unknown.png)

## 2.7 Машинный телеграф

AHEAD - вперед, ASTERN - назад. По центру кнопка тревоги.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572869949756932096/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572869949756932096/unknown.png)

## 2.8 Управление рулем

- Справа вверху - счетчик количества энергии в аккумуляторах в килоамперчасах;
- Слева - спидометр в узлах + одометр;
- По цетру - компас;
- Справа - текущее положение руля;

[![](https://cdn.discordapp.com/attachments/572801769516695564/572870522183090206/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572870522183090206/unknown.png)

## 2.9 Радио

Справа передатчик, слева приемник.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572871006549442580/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572871006549442580/unknown.png)

Сообщение, зашифрованное энигмой передается с помощью телеграфного ключа азбукой Морзе.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572871233629323274/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572871233629323274/unknown.png)

## 2.10 Энигма

Вверху выставляется три буквы ключа. На каждое нажатие буквы открытого текста Энигма высвечивает ее зашифрованный вариант. Пробелы не используются - они делают шифр уязвимым к частотному анализу. 

[![](https://cdn.discordapp.com/attachments/572801769516695564/573151402742906880/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573151402742906880/unknown.png)

## 2.11 Локатор радиосигналов

Управление направлением сканирования радиочастот.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572875677221650442/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572875677221650442/unknown.png)

Слева громкость, по центру выбор диапазона частот и самой частоты.

[![](https://cdn.discordapp.com/attachments/572801769516695564/572875881115156511/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572875881115156511/unknown.png)

## 2.12 Гидрофон

- Внизу - изменение пеленга;
- Gain - усиление звука; 
- Внешний лимб - направление относительно курса лодки;
- Внутренний лимб - направление, относительно севера;
- Справа управление частотными фильтрами;

[![](https://cdn.discordapp.com/attachments/572801769516695564/572877083156545566/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/572877083156545566/unknown.png)

## 2.13 Проигрыватель

Слева направо - комнаты, куда играть, звук на лодке/звук снаружи, выбор и остановка музыки.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573151545282265088/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573151545282265088/unknown.png)

# 3. Управление лодкой

## 3.1 Порядок всплытия и погружения

### Теория

По закону Архимеда, чтобы тело полностью погрузилось в воду, его вес должен равняться весу вытесненной им воды. Для погружения ПЛ принимает балласт — воду — в цистерны. Для всплытия балласт продувается: вода вытесняется из цистерн сжатым воздухом. Когда лодка полностью погружена, она меняет глубину с помощью рулей. Прием или откачка балласта после этого производится только для уравновешивания.

Главным элементом являются цистерны главного балласта (ЦГБ). Их заполнением погашается основной запас плавучести ПЛ, и обеспечивается нормальное погружение.Как правило, балласт ПЛ рассчитывается так, чтобы с заполненными концевыми группами лодка плавала «под рубку» — над водой только ограждение рубки. Такое положение называется позиционным.

Когда требуется срочное погружение и заполнение даже всех ЦГБ сразу оказывается слишком медленным, используют цистерну быстрого погружения (ЦБП, иногда называется цистерной срочного погружения). Её объём не входит в расчётный запас плавучести, то есть, приняв в неё балласт, лодка становится тяжелее окружающей воды, что помогает «провалиться» на глубину. После этого, разумеется, цистерна быстрого погружения немедленно продувается.

### Практика

## 3.2 Управление режимами машин, руление, энергетика и живучесть

### Теория

Заполнение и продувка цистерн, выстрел торпед или ракет, движение и вентиляция требуют затрат энергии. Соответственно, без энергии лодка не может не только двигаться, но сколько-нибудь долго сохранять способность «плавать и стрелять». Сжатый воздух является вторым по значению источником энергии на лодке и, во вторую очередь, даёт запас кислорода. Хранить сжатый воздух выгоднее под высоким давлением — занимает меньше места и аккумулирует больше энергии. Пополнение запасов сжатого воздуха — долгая и энергоёмкая операция, и она требует доступа к атмосферному воздуху.

Основными элементами электроэнергетической системы являются генераторы, хранилища и потребители энергии. В классической системе дизель-электрической ПЛ электромотор используется как обратимая машина, то есть может потреблять ток для движения, или вырабатывать его для зарядки. В такой системе имеются:
- Главный дизель. Является двигателем надводного хода и приводом генератора. Также играет второстепенную роль как поршневой компрессор.
- Гребной электродвигатель (ГЭД). Основным его назначением является работа на винт в подводном положении. Может также играть роль генератора.
- Аккумуляторная батарея (АБ). Запасает и хранит электроэнергию от генератора, выдаёт её для расходования когда генератор не работает — прежде всего под водой.

Для такой ПЛ характерными режимами являются:
- Винт-зарядка. Дизель одного борта вращает гребной винт, дизель другого работает на генератор, заряжая АБ.
- Частичное электродвижение. Один дизель работает на генератор, часть энергии которого потребляется электродвигателем, другая часть идёт на зарядку АБ.
- Полное электродвижение. Энергия АБ потребляется электродвигателем.
- Дизель-движение. Дизеля вращают гребной винт.

### Практика

## 3.3 Следование курсу по навигационным приборам

Существует простое мнемоническое правило для быстрого приблизительного пересчёта в уме узлов в километры в час: «умножь на два и вычти 10 процентов». Например, скорость 15 узлов, 15×2 = 30 км/ч, вычитаем 10% = 3 км/ч, получаем 27 км/ч. Правило даёт значения с погрешностью менее 3 %. Для пересчёта км/ч → узлы применяется обратный алгоритм: скорость в км/ч делится на 2 и к полученному значению прибавляется 10%. Например, 20 км/ч → 10 узлов → 11 узлов (точное значение равно 10,8 узла).

## 3.4 Порядок запуска торпед и ведение огня из палубных орудий

Для успешного попадания необходимо выставить скорость, расстояние, курсовой угол цели, выбрать торпедный аппарат, глубину хода торпеды, перескоп наводки. Затем навестись с перископа на цель и произвести пуск.

# 4. Определение скорости и курса цели по четырем пеленгам

1) Остановиться и определить положение лодки.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573151912392654858/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573151912392654858/unknown.png)

2) Запеленговать цель три раза с промежутком в 5\* минут, сразу после третьего замера дать полный ход.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573152878332739585/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573152878332739585/unknown.png)

3) На втором пеленге отметить произвольную точку и построить две прямые через эту точку, параллельные первому и третьему пеленгу.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573152957810606081/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573152957810606081/unknown.png)

4) Прямая, проведенная через точки пересечения построенных прямых и первого и третьего пеленгов даст курс противника ("мнимый" путь - прямая, парралельная истинному пути цели). Для получения истинного местоположения и скорости необходимы дополнительные вычисления.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573153200513744896/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573153200513744896/unknown.png)

5) Из точки пересечения третьего пеленга и прямой, параллельной первому пеленгу, отложим окружность радиусом, равным расстоянию от данной точки до точки пересечения второго пеленга и "мнимого" пути цели - это будет первая точка пересечения этой окружности и "мнимого" пути. Вторая точка перемечения этой окружности и "мнимого" пути даст нам пеленг, который мы получили бы, если бы оставались на месте после получения третьего пеленга - этот пеленг обозначен пунктиром.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573153466516766741/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573153466516766741/unknown.png)

6) Через 5\* минут после получения третьего пеленга и подачи полного хода необходимо сделать четвертый пеленг. Точка пересечения этого пеленга и пунктирного пеленга будет являться истинным положением цели в данный момент (20:38:48).

[![](https://cdn.discordapp.com/attachments/572801769516695564/573155127968399371/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573155127968399371/unknown.png)

7) Далее необходимо построить прямую через эту точку, параллельную "мнимому" пути - это будет истинный путь. Следует замерить расстояние между точками пересечения первого и четвертого пеленгов и истинного пути (3382 m = 3,4 km).

[![](https://cdn.discordapp.com/attachments/572801769516695564/573156319754846218/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573156319754846218/unknown.png)

8) Затем стереть все лишнее и посчитать скорость цели, с помощью номографа или элементарных преобразований.

[![](https://cdn.discordapp.com/attachments/572801769516695564/573157947236941835/unknown.png)](https://cdn.discordapp.com/attachments/572801769516695564/573157947236941835/unknown.png)

\* Промежуток между пеленгами может отличаться от 5 минут, но он должен быть всегда равным! Чем дольше промежуток между пеленгами - тем точнее вычисления. 

# 5. Определение параметров цели с использованием перископа и справочника
