---
title: Учим физическому мышлению на среднем уровне формальности, а не «разделам физики»
---

Сегодняшняя попытка учить физическому мышлению сводится к попытке
рассказывать физику как линнеевскую классификацию в биологии: какие
чудесные у нас законы в оптике, магнетизме, механике и так далее,
огромный список разделов физики, в каждом есть какие-то уникальные
знания. Нет, в образование по физике должны попасть самые важные и общие
идеи о том, как делать догадки об объектах окружающего мира таким
образом, чтобы их потом можно было попытаться описать математическими
объектами. Гипотеза: «Очень Умные Физтехи» (tm) именно так и думают о
мире, используют физическое мышление. И именно поэтому успешны отнюдь не
только в физике и математике, но и просто в жизни. Физика и математика
удобны для описания окружающего мира, мы просто не требуем тут лишней
точности/строгости/формальности в описании. Вот этому тоже надо учить:
проигрываем в точности и формальности, но отслеживаем уровень возможной
ошибки. Например, «считаем с точностью до порядка величины», зато
выигрываем во времени как обучения, так и последующего рассуждения.

Основные идеи конечной точки этого путешествия по основным понятиям
физики должно быть можно рассказать «на пальцах», без указания формул
для точного расчёта. Это должно делаться без математической нотации, без
строгих формул (текстом! на среднем уровне спектра формальности!), но
более-менее используя явное присвоение типов и задействуя математические
и физические понятия как задаваемые математикой и физикой объекты
внимания и отношения между ними, нужные для физического/математического
(тут оно по факту одно и то же, «физмат») моделирования. Идея эта
немного отличается от идеи научно-популярного изложения научных идей,
когда этой популяризацией занимаются сами крупные учёные (а не какие-то
«профессиональные популяризаторы науки»). Эти учёные иногда выбирают
популяризовать свои труды в текстах «концепции использования важной
теории, изложение почти без формул» в надежде, что кто-то потом
заинтересуется и формульным изложением результатов, «конструктивной
частью» с математикой. Таких работ довольно много. Может показаться, что
мы тут идём по линии:

-   David Deutsch, который «на пальцах» писал про эвереттовскую
    интерпретацию квантовой механики в двух своих книгах (и даже
    рассказывал нужную ему математику «на пальцах», все эти идеи по
    поводу счётных и несчётных бесконечностей)
-   Judea Pearl, который описывал «на пальцах» в «Книге почему» свою
    лестницу причинности
-   Nassim Taleb, который «на пальцах» рассказывал про ренормализацию,
    хотя ему это нужно было для очень узкого случая, а не для описания
    удобного универсального приёма многоуровневого мультимасштабного
    моделирования.
-   Pedro Domingos так описывал алгоритмы машинного обучения (поиск
    «универсального алгоритма»), практически без формул (и это при том,
    что все книги по машинному обучению по факту начинаются с разделов
    математики, используемой в машинном обучении!)
-   ... этих «науч-поповцев» много, их методическая («как объяснить
    сложные идеи попроще за ограниченное время») работа бесценна!

Karl Friston так и говорил, что хорошо бы создать популярное
«телеологическое» (функциональное, «зачем это надо») изложение идей
active inference, а затем заинтересовавшихся теорией плотно погрузить в
математическое изложение этих идей.

В какой-то мере мы в наших описаниях SoTA практик интеллект-стека, в том
числе и математики с физикой, следуем этой традиции, но всё-таки не
совсем именно этой. Мы не считаем, что передаём студентам «попсовую»
завлекательно-мотивирующую/«маркетинговую» версию трансдисциплин. Нет,
мы учим вполне работающим версиям трансдисциплин, знания по которым
могут приносить ощутимую пользу во многих проектах, где встречаются
плохо понимаемые проблемы. Вот с этим «плохим пониманием проблем» и
работают трансдисциплины интеллект-стека, и мы их преподаём на среднем
(псевдокод) уровне строгости/формальности.

Мы учим студентов «концепции использования» какой-то теории, выдаём
знания и умения по использованию «интерфейса вычислителя/объяснителя»
для этой теории, то есть обучаем задействовать какой-то «специальный
порождающий моделер» для этой теории. В большинстве случаев такого
знания будет хватать для многих и многих прикладных задач. Пользоваться
фотоаппаратом можно, если знаешь его интерфейс, не надо знать
особенностей его софта, пока не встретишься с необходимостью что-то
сильно поменять в параметрах фотографирования --- тогда придётся
разобраться в устройстве, и даже подхакать софт. То же самое относится к
математике и физике: знать их надо на уровне «прикинуть результат,
поговорить со специалистом, даже если этот специалист --- моделер с
подключённым AI», и только после необходимости плотно поработать в
области физики и математики надо будет разобраться в каких-то разделах
математики (и потратить на это несколько лет обучения).

Выполнение точных вычислений согласно формулам теории надо отдать
компьютеру (возможно, по пути использовав какой-то «компилятор»,
переводящий не слишком формальное описание проблем в более формальное
задание на вычисление или рассуждение). Не надо выполнять за компьютер
то, что может сделать компьютер. Не надо руками заколачивать гвозди, не
надо «ногами» бегать на марафонские дистанции (используйте хотя бы
велосипед), «руками» решать интегральные уравнения. Надо использовать
инструменты, если хотите делать какое-то дело. Если это хобби, или «для
здоровья», или «для учёбы» --- нет проблем, обучайте-тренируйте тело и
нейронную сеть в мозгу. Если для работы --- пользуйтесь инструментами,
не хвастайтесь «ручным трудом», даже если это «труд голого мозга».

И вот тут нужно понимать, чему учить, что оставить компьютерам, а что не
нужно учить, даже если каким-то физикам это представляется очень важным
в самой физике. Нужна важность не в физике, а важность физики в жизни,
причём жизни студента-выпускника!

«Важно для препода, он считает это ключевым в его предмете» нельзя
путать с «важно для студента, ему это использовать в жизни, и
использовать часто»: как передать студенту то знание (в нашем случае
физического мышления как способа моделирования окружающего мира и
какого-то содержания разделов физики как удачно выполненных примеров
этого моделирования), которое будет не «для сведения» и «ой, как
любопытно!», а реально снизит общие затраты на обучение плюс
использование. Скажем, **если я учил месяц в университетском курсе, как
решать уравнение Гамильтона, а потом в жизни решал его аж один раз
десять минут, то оценка** **требуемого моего** **ресурса** **на решение
этих уравнений ---** **1 месяц 10 минут на одно решение** **(обучение
плюс время использование мастерства), а если мне не пришлось ни разу
решать это уравнение, то оценка ресурса будет минус месяц из жизни**
**(только обучение, использования не было).**

По такому методу расчёта почти всё школьное и вузовское образование
оказывается зря потраченным временем: дисциплинам интеллект-стека,
нужным для решения самых разных задач, учат только «исподволь» (то есть
чаще всего не научают, даже если планировали), а всяческие «разделы»
математики и физики, да ещё и намеренно данные на уровне каких-то
прошлых представлений (скажем, ньютоновской физики в варианте времён ещё
лично Ньютона) оказываются неприменимыми. И ещё нужна форма учебного
курса, гарантирующая умение применения изученных понятий для мышления в
самых разных предметных областях. Мы ж учим трансдисциплинарному знанию,
это ж интеллект-стек, знание должно быть полезным во всех проектах, и
это очень интересный критерий: во всех проектах надо уметь считать, во
всех проектах учитывать их физичность и отсутствие потусторонних
(божественных или демонических) сил, и знание физики и математики должно
быть на уровне, помогающем как-то по-быстрому провести численное
моделирование ситуации на уровне студента физтеха или выпускника
executive MBA (как ни странно, студентов MBA немного учат
математическому моделированию для решения менеджерских задач).

Когда John Doyle в своих
работах^[<https://ailev.livejournal.com/1622346.html>]
говорит, что для понимания описанной в них физики (какого-то
управления/control, происходящего в физическом мире) достаточно школьной
математики, он явно приукрашивает ситуацию: школьной математики
недостаточно. Когда в маркетинге, менеджменте требуется выдать какие-то
«оценки плохо измеримого», то надо давать или квантовоподобные оценки
вероятностей, или хотя бы байесовские каких-то величин, которые ещё надо
сформулировать как измеримые. Школьной и вузовской математики и физики
«по разделам» для этого недостаточно, нужно понимать принципы измерений
и их точности как таковых, это трансдисциплинарное знание.

Все эти научно-попсовые книжки Дойча, Перла и подобных авторов
рассказывают «вот такое бывает для вот таких целей», а когда вы
интересуетесь применением знания, то вас отсылают на четыре курса
естественнонаучного бакалавриата, за первые же несколько семестров вам
расскажут много чего разного на предмет беглого чтения текстов по
линейной алгебре в классической математической нотации и заодно
расскажут подробно о классической механике и классической статистике, а
затем --- магистратура, но по итогам обучения вы окажетесь по вопросу
применения содержания «научно-попсовых книг» примерно в том же месте: не
будете понимать, как использовать это знание здесь и сейчас, в рабочем
проекте, да ещё практически в каждом проекте!

Вот эту «трансдисциплинарную математику» и «трансдисциплинарную физику»
вместо «избранных разделов математики» и «избранных разделов физики»
нужно выявить и преподавать в рамках обучения интеллект-стеку. Физика и
математика нам нужны не просто «ум в порядок привести» (мы и сейчас это
делаем без особой на них опоры, например, изучая семантику, онтологию,
логику). Нам они нужны только потому, что с мета-мета-моделью физики и
математики удобно думать про окружающую жизнь с её разнообразными
предметными областями. Они нужны для усиления мышления, с ними удобно
моделировать! Они задают правильные объекты внимания в окружающем мире.
Представление о многомерном пространстве у современного человека просто
обязано быть, и какие-то идеи о том, что такое оптимизация какой-то
функции в таком пространстве. И должно быть некоторое количество
примеров, показывающих продуктивность этого мыслительного приёма в
рабочих проектах.

Выучился --- и стал думать таким образом. «Информационное поле» --- и у
тебя есть интуиция, как думать о «поле», что там за операции делают с
объектом «поле» и какие там рядом должны быть ещё важные объекты
(скажем, «потенциал»), и само это поле --- что там «физично», а что
«математично». Собственно, интегральное и дифференциальное исчисления
были получены для задач механики, а потом пошли гулять по всем областям
знания. Вариационное исчисление --- то же самое. Квантовая математика
тоже потихоньку отрывается от квантовомеханических задач (Андрей
Хренников тут только один из лидеров). Механика остаётся только удобным
средством для объяснений, что там за задачи когда-то решались. Наша
новация: мы возьмём вот эти основания математики и прямо их предложим
использовать для моделирования самых разных аспектов окружающего
физического мира. Да, это и есть «физическое мышление». Говорить и
думать о мире будем примерно так, как это делают физики, хотя
необязательно это делать на «птичьем языке». Например, можно говорить о
неэргодических системах как системах с памятью состояний, необязательно
заставлять запоминать слово «эргодичность». Но вот понимать, что там
происходит с фазовыми траекториями и что такое физическое действие ---
вот это надо бы, причём учить надо на уровне работы с типами в
онтологике.

Это ни разу не «закон ньютона» из прошлых веков, тут меньше упор на
законы классической механики (толку от того, что они учились в школе!
Они же всё равно не используются в жизни, кроме иногда замечания, что
«палец давит на стол с той же силой, что стол давит на палец»). Больше
внимания нужно уделять **удобным** **объектам** **для разговора и
рассуждений об окружающем мире: действия и принцип наименьшего действия,
движение и энергия, поле и траектория,** вот это вот всё самое базовое.
И да, эргодичность/наличие памяти и выход на стохастические методы
(теорвер!) и обязательно ренормализация для учёта многоуровневой
структуры мира. Как описывать мир и его изменения, как об этом думать:
примерно та же постановка задачи, как при создании курсов системного
мышления и онтологики.

Отобрать именно то, что нужно на кругозорном уровне для описания мира и
его изменений в самых общих чертах. И сформулировать онтологически, как
объекты и отношения (а не как строгие формульные выкладки, эти выкладки
можно потом будет взять из любого справочника, они будут
запрограммированы в любом моделере, их подскажет любая программа AI).
Тут самое важное, что надо будет сделать проверку: мета-мета-модель (эти
самые общие понятия и закономерности) должна помогать выбирать объекты
мета-модели в самых разных предметных областях.

Важно, чтобы все эти важные физические понятия формулировались с учётом
не старинной математики, а с учётом современной математики.
«Математика --- это язык науки», но надо проверять, какую версию языка
науки мы учим, и учить надо свежую версию, а не старинную. Когда-то
международным языком была латынь, затем французский, сейчас английский.
Вот и язык математики надо отслеживать --- какой его брать для выражения
физики?

Отдельный вопрос про нотацию: какую математическую нотацию? Формулы,
которые кроме как с графического планшета не введёшь, или какой-то
вариант записи текстом, как в программах Wolfram Alpha? Лучше бы сразу в
виде, который удобен для моделирования не ручкой и бумажкой (скажем, при
правке формул, записанных ручкой и бумажкой, их часто приходится
переписывать. А в компьютерной записи их можно просто удобно
редактировать --- это же просто цепочка символов!).

И хорошо бы исключить «исторический подход», не надо учить разные
варианты теорий флогистона, надо учить современный вариант теории (хотя
можно упоминать, что «было вот так, вы можете встретить это в старых
книжках и в разговорах со стариками»). Теорию флогистона из истории
физики учить не нужно! И не факт даже, что нужно учить какие-то азы
ньютоновской или даже гамильтоновской механики в физике. А вот основные
идеи, вроде «для чего потребовался именно лагранжиан» --- без
конкретного знания как его точно вычислять и что это такое на уровне
полностью строго формальном --- вот это вполне может потребоваться.

Скажем, в одном из писем Karl Friston в ActInfLab пишет: «expected free
energy (which itself is a euphemism for a path integral of a
Lagrangian)». А ведь expected free energy является в подходе active
inference одним из главных терминов! Но Фристон признаётся, что это
термин введён для того, чтобы не говорить «нецензурные математические
слова» про path integral of a
Lagrangian^[<https://en.wikipedia.org/wiki/Path_integral_formulation>].
Нужно разобраться, какие ещё «культурные синонимы» есть как термины для
то ли физических, то ли математических объектов (помним, что физики эти
объекты отождествляют в мышлении, и различают только в том случае, когда
поведение мат.объектов начинает сильно отличаться от измерений поведения
физ.объектов). В терминологии и математики, и физики есть много
исторических наслоений и бессмысленных наименований именами
исследователей вместо хороших мнемоник (тот же «Лагранжиан»), их хорошо
бы как-то убрать, сделать реформу языка, надо резко упростить разговор и
начальное понимание. Это резко ускорит обучение. В некоторых случаях
можно и предложить свой синоним к куче уже имеющихся --- хуже для самого
предмета не будет (роза пахнет розой, хоть розой назови её, хоть нет),
но время обучения снизится, этот приём очень хорошо показал себя на
курсах онтологики и системного мышления. Тут, конечно, лучше не
переусердствовать, полностью свой новояз лучше не изобретать. Но если
есть три синонима, то выбирать надо не «исторический», а наименее
запутывающий. И, конечно, должны быть не столько упражнения, сколько
задания на использование предлагаемого мышления прямо в рабочих
проектах. Для других трансдисциплин такое обучение хорошо работает,
почему бы этому не сработать с математикой и физикой? Это, конечно, не
быстрое дело. Курс системного мышления создавался примерно 10 лет
(причём безо всякой помощи со стороны искусственного интеллекта). Можно
ожидать, что создание подобного сорта курсов математики и физики займёт
столько же.

Более того, совершенно необязательно делать отдельные курсы математики и
физики, как это принято в вузах. Дисциплины и курсы ортогональны: один
курс может учить нескольким дисциплинам, несколько курсов могут учить
одной дисциплине. Так и с математикой и физикой, а также близко
примыкающими к ним семантикой, логикой и алгоритмикой (впрочем, и всеми
другими трансдисциплинами): это содержание может быть разбросано по
разным курсам.

Это поможет снять и проблему percieved cognitive load из теории
мотивации ожидаемой пользой, expectancy value
theory^[<https://en.wikipedia.org/wiki/Expectancy-value_theory>].
Физика и математика находятся где-то ближе к началу интеллект-стека, но
поскольку решение учиться принимается даже не по реальной трудности
обучения (cognitive
load^[<http://en.wikipedia.org/wiki/Cognitive_load>]),
а по воспринимаемой до начала обучения (perceived cognitive load), то
при обучении «математике» и «физике» как отдельным курсам с этими
«серьёзными именами заведомо сложных дисциплин» появится вот эта
проблема. Хотя способности людей к физике и математике более-менее
одинаковы, восприятие своих способностей у студентов разное, поэтому не
факт, что должны быть именно курсы математики и физики, хорошо бы
избегать этих названий. Заодно это решает проблему с женщинами: женщины
имеют те же способности к обучению физике и математике, что мужчины (у
женщин и мужчин интеллект в среднем одинаковый, это только способности к
физкультуре разные --- мужчины в среднем оказываются банально сильнее и
быстрее), но в силу текущей социокультурной ситуации девочки и женщины
желают обучаться физике-математике меньше даже при наличии возможности
учиться. И мы теряем чуть ли не половину земного шара. Вот и не надо
говорить, что «учим математике и физике». Говорить не надо, а учить ---
надо!

Такой проект обучения «физмату» более чем
рисковый^[Проблемы обучения методологическим
дисциплинам, 2019,
<https://ailev.livejournal.com/1466484.html>], а в
текущей социокультурной ситуации давних традиций преподавания и физики,
и математики, так ещё и более чем скандальный. Каждый образованный
«технарь» учился в школе-вузе-аспирантуре и физике, и математике, и если
не алгоритмике, то программированию, поэтому у каждого-всякого человека
обязательно будут идеи, чему и как в этом плане нужно учить!
Предлагаемый нами критерий тут --- не самоценность обучения физике и
математике, а с целью повседневного использования в мышлении! К
сожалению, работа по выделению из современной математики и физики не
«интересных» (для попыток заинтересовать в изучении «разделов», цель
науч-поп литературы), а повседневно полезных мыслительных приёмов ---
она даже пока не ставится. Нужен прямой повседневный выход
математического и физического мышления (а потом мы добавим к этому и
тесно связанное с ними алгоритмическое мышление, и лежащее в основе их
всех логическое мышление) на проектные ситуации.

Минимальный образовательный ценз на разговор об обучении математике и
физике в рамках интеллект-стека --- это понимание остальных частей
интеллект-стека в части организации непосредственного использования
материала этих курсов для поддержки сильного и эффективного
коллективного мышления в рабочих проектах. То есть для начала разговора
культуртрегеру, методологу и методисту курсов, которые включают обучение
математике и физике надо иметь в своём активе прохождение курсов ШСМ в
объеме как минимум программы первого года «от онтологики и собранности
через системное мышление и методологию к инженерии и менеджменту» (и
квалификацию мастера, то есть «что-то уметь делать, а не только
прочитать учебники»), равно как надо иметь понимание тех самых
унивалентных оснований математики, неформальной теории типов из
математики, а также лагранжиана, эргодичности, ренормализации и
связанного с ними принципа наименьшего действия из физики. Основной
разговор тут --- как вот эту физмат мета-мета-модель (и даже
мета-мета-мета-модель, foundational ontology) использовать в рабочем
мышлении про окружающий мир, выход в широкие классы проектных ситуаций
вместо специальных ситуаций физмат-моделирования отдельных узких
аспектов систем. Упор тут может быть даже не на работу с точными
вычислениями по конкретным формулам, а задействование не слишком
формальных рассуждений по примерно тем шаблонам мышления, которыми
пользуются физики при математическом моделировании.

Отдельный вопрос --- это терминология. Математические и физические
объекты в быту и прикладных дисциплинах (например, менеджменте) часто
имеют плохо переводящиеся на язык математики-физики термины для давно
знакомых понятий/ментальных/математических объектов. Так как надо:
оставить эти термины при изучении прикладных дисциплин «историческими»,
или таки заменить? Скажем, «прирост скорости» --- это вроде как отсылка
к «ускорению», но без включения времени. Давайте попробуем в механике:
«прирост скорости с 20км/час до 30км/час» --- нормально звучит? А теперь
через ускорение: это как с 0 км/час разогнаться до 10 км/час, то есть с
0 м/сек до 2.8 м/сек. Если за пару секунд, то ОК. Если за десятую
секунды, вам мало не покажется. Это то же самое, что затормозить на бегу
об стенку (удар), или наоборот, стенка вас разгонит до беговой скорости
(рывок). Если вы двигались равномерно, а потом вдруг «скорость приросла
на 10 км/час за десятую секунды», это будет один рывок/удар. Если у вас
было две секунды, то совсем другой
рывок/удар/jerk^[[https://ru.wikipedia.org/wiki/Рывок\_(кинематика](https://ru.wikipedia.org/wiki/Рывок_(кинематика))],
и это классический термин для производной третьего порядка. Конечно,
когда мы говорим о скорости работы (которая не имеет массы) или скорости
финансового потока (там тоже массы нет), то рассуждения будут другими,
но выкидывать длительности приложения усилий нельзя. Дальше вопрос: а
что будет, если вместо «прироста скорости» перейти на обсуждение
«ускорения», а вместо «прироста ускорения» говорить о рывке? Это сразу
даст нам ещё и вариант обозначения действия: ускорение и рывок ---
отглагольные существительные.

Если говорить дальше о менеджменте, то нужно быть внимательным: все эти
Flow Time и Touch Time весьма абстрактны, можно пытаться назвать их
поточнее, что регулярно пытаются делать и на английском языке. Скажем,
Flow Time is also known as Time in Process, Process Time or System Lead
Time. Flow Time is often and ambiguously referred to as Cycle Time,
especially by practitioners of the Kanban Method. Все стараются, как
могут, при этом речь идёт о продолжительности, а не о собственно моменте
времени. Очень не хочется сочинять англоязычную и даже русскоязычную
онтику операционного менеджмента, но на кону облегчение понимания. Все
авторы книг по операционному менеджменту подчёркивают, что предмет у них
абсолютно контринтуитивен и понимание даётся очень трудно, справляются
только сугубые технари, и даже люди с финансовым образованием не
прорываются, хотя им вроде как математика не чужда. Проблемы эти в том
числе и из-за весьма специфической терминологии, затрудняющей
непосредственное выражение проблем в терминах математики --- мало того,
что слова не помогают найти нужные объекты в жизни, это всё оказывается
«яблоками из задачи», без намёков на «яблоки из жизни», так ещё и трудны
сопоставления с математическими объектами из формул для расчёта
логистических потоков при операционном менеджменте.

Даже курс системного фитнеса в части соматодинамики должен принять
какую-то терминологию, чтобы обсуждать высшие производные. В танцах как
двигательной практике мало разговора о разгонах и торможениях как
действии ускорения/acceleration (вторая производная), нужно говорить ещё
и о рывке/jerk (третья производная). Разгон в танцах неравномерный:
вначале прикладывается мало усилия, но по окончании разгона --- много
(рывок ненулевой! ускорение меняется, а уж скорость тем более). Конечно,
рывок может быть и при разгоне, и при торможении. Разгон и торможение с
рывком дают некоторый
гистерезис^[(https://ru.wikipedia.org/wiki/Гистерезис]
(тоже термин из физики, он оказывается общеприменимым во многих
проектах!), при гистерезисе отклик системы запаздывает. В танцах у нас
«виртуальная
физика»^[<https://vk.com/wall-179019873_1186>],
но мы там работаем с гистерезисом: фолловер откликается с задержкой, и
существенная задержка отклика входит в стилистику как минимум танго и
модерн свинга, и в этих же танцах особо рассматривается неравномерность
движения (контраст). Скажем, в кизомбе лидер движется более-менее
равномерно, при этом стартует и прекращает движение мгновенно (очень
быстрый разгон и торможение, рывок с места, затем на этом же усилии
разгон и дальше сопровождение инерционного движения, торможение такое же
«внезапное» --- «блок», считающийся неприличным во многих других танцах,
как «резкое прерывание движения»). И вот чтобы всё это описывать,
«рывок» хорошо бы использовать при обучении танцам не в его бытовом
значении^[Тяни-толкай в коннекте и минимизация усилий
для рывка и блокирования ---
<https://vk.com/wall-179019873_1622>], а прямо брать из
физики, равно как и понятие гистерезиса.
