---
title: 'Новая алгоритмика: изучение универсальных алгоритмов'
---

В алгоритмике (Theory A из информатики/computer science) предметом
заботы являются алгоритмы вычислений --- нахождение таких способов
вычислений (практик выполнения операций), которые как дают точный
результат, так и укладываются в ресурсный бюджет. Ресурсы оказываются
важны. Если у тебя есть выбор  --- точно моделировать ситуацию, затратив
на это время и энергию, или моделировать очень грубо, но затем сразу
действовать, то побеждает не всегда идея точного моделирования. Тебя
просто съедят, если ты будешь много думать и мало бегать! Но если ты
будешь быстро и экономно моделировать с большой точностью, то придётся
меньше бегать, и направление бега будешь вычислять точнее  --- и тебя не
успеют съесть. Так что есть задача моделирования мира с большой
точностью, но с затратой малого количества ресурсов и времени.

Проблема в том, что точность моделирования мира и потребность в
вычислительных ресурсах в большинстве случаев увязаны между собой. Если
вы хотите отмоделировать мир точно, то вам нужно много исходных данных и
много вычислений. Иногда это удаётся обойти придумыванием нового способа
моделирования, новых алгоритмов вычислений, но иногда теория говорит,
что в общем случае это невозможно. Например, сегодня для многих и многих
задач находится максимум какой-то функции методом градиентного спуска. В
конце 2021 года выяснилось, что точность и вычислительная сложность
(время вычисления при последовательном выполнении операций) для таких
задач связаны пропорционально. Если точность удвоить, то время нужно
увеличить вчетверо (и это обычно приемлемо), но если для некоторых
приложений нужна точность в квадрате, то время (число вычислительных
шагов) нужно увеличивать тоже в квадрате --- и это может оказаться за
пределами разумного. Скажем, один миллиард шагов одинарной точности
могут выполняться одну секунду, но вот миллиард секунд для квадрата этой
точности --- это 32 года работы вычислителя! При этом подобные ресурсные
оценки сложности алгоритмов неприменимы при переходе к другой физике
вычислителей/компьютеров, например, при переходе к квантовым
компьютерам. Такое впечатление, что алгоритмик как версий науки о
сложности и ресурсоёмкости алгоритмов может быть множество, для каждой
физики вычислений своя версия, и ещё варианты для различных сложных
вычислителей, объединяющих вычисления, ведущиеся в разной физике.

Похожие рассуждения по ресурсным (а не теоретическим!) ограничениям на
вычисления на одном классическом одноядерном электронном компьютере есть
и для многих других классов задач. Например, криптографические задачи
основываются на том, что вы легко проверяете ключ на его правильность,
за долю секунды. Но вот найти этот ключ, если вы его не знаете, может
потребовать тысяч лет вычислений, хотя всего одного года, если у вас
тысячи компьютеров, алгоритм ведь хорошо распараллеливается! Ситуация
опять-таки осложняется тем, что при переходе на другую физику (например,
квантовый вычислитель/компьютер разбрасывает нужные для получения
операции по бесконечному числу вселенных, а потом собирает их результаты
для получения конечного ответа, подробно это рассказывается в книгах
Дэвида Дойча) оценка сложности алгоритмов меняется. И ещё всё время
придумываются новые алгоритмы, причём нахождение нового алгоритма ---
это творческий процесс, для многих классов задач до сих пор непонятно,
можно ли вообще найти быстрый алгоритм получения решения (проблема
перебора^[[https://ru.wikipedia.org/wiki/Равенство\_классов\_P\_и\_NP](https://ru.wikipedia.org/wiki/Равенство_классов_P_и_NP)]):
можно ли для задач, которые заведомо решаются методом перебора,
придумать алгоритм, который решает их не за экспоненциальное по
отношению к объёму входных данных время, а за меньшее, полиномиальное
или даже линейное. Алгоритмика до сих пор не даёт ответа на этот важный
вопрос!

Есть математический результат 1989 года (теорема Джорджа
Цыбенко^[[https://ru.wikipedia.org/wiki/Теорема\_Цыбенко](https://ru.wikipedia.org/wiki/Теорема_Цыбенко)]),
который показывает, что нейронная сеть с одним скрытым слоем является
универсальным аппроксиматором, то есть может отмоделировать с заданной
точностью любую функцию, если в ней есть «достаточное количество
нейронов». Любая функция --- это таки математически любая, например,
«распознавание речи» --- это из входных бит огибающей сигнала на выходе
аналого-цифрового преобразователя с сигнала микрофона вычислить по
функции распознавания речи последовательность бит слов текста в
подходящей символьной кодировке. Синтез речи --- это обратная функция,
из букв в звуки. Диагноз --- это функция из входных данных множества
анализов больного в выходные с текстом диагноза. Назначение лечения ---
обратная функция.

Проблема только в том, что на существующих классических компьютерах
моделирование даже простых функций занимает на такой нейронной сети
огромное время, это математически очень крутой результат, но практически
он бесполезен. Алгоритмика как раз наука о том, как получить практически
полезные результаты, то есть получить результат достаточной точности,
использовав минимальные ресурсы, которые можно было бы потратить на
вычисления так, чтобы вычисления были выгодны (полезность результата
вычислений оценивалась выше, чем полезность ресурсов, потраченных на
вычисления).

При этом подход «универсального вычисления на нейронной сети»
оказывается таким общим, что вся Вселенная представляется таким большим
«нейросетевым компьютером» (работы группы Ванчурина, о которых мы уже
довольно много говорили, но появляются и более новые работы, которые
представляют «космическую нейронную сеть» из небесных
тел^[<https://www.frontiersin.org/articles/10.3389/fphy.2020.525731/full>]
и уподобляют её нейронной сети мозга).

Так, если сделать глубокую нейронную сеть (несколько скрытых слоёв), то
свойства универсального аппроксиматора остаются, но время моделирования
оказывается вполне приемлемым --- хотя опыт показывает, что один расчёт
большой языковой модели может стоить несколько миллионов долларов за
аренду вычислительных мощностей для этого, нейронная сеть GPT-3 была
вычислена за примерно \$4.6
млн^[<https://www.reddit.com/r/MachineLearning/comments/i49jf8/d_biggest_roadblock_in_making_gpt4_a_20_trillion/>].

Интеллект компьютеров, похоже, зависит главным образом от вычислительной
мощности --- это так называемый «горький
урок»^[<http://incompleteideas.net/IncIdeas/BitterLesson.html>],
полученный анализом всех прошлых прорывов в области AI. Все эти прорывы
оказывались прорывами не столько в хитрых конструкциях самого интеллекта
как исполняемого на хитрых компьютерах хитрыми алгоритмами, сколько
прорывами в не очень хитрой алгоритмически аппаратной вычислительной
мощности. Простые алгоритмы и большая вычислительная мощность  --- вот в
чём оказался секрет искусственного интеллекта! То есть вы в конечном
итоге терпите неудачу, когда пытаетесь сочинить сложный алгоритм,
управляющий каким-нибудь автомобилем в поездке. Но если вы в автомобиль
включаете суперкомпьютер, и этот суперкомпьютер выполняет относительно
простые вычисления в просто устроенной алгоритмически нейросети, то вы
получите такие результаты, какие не получите от специально
разрабатываемого традиционного «алгоритма вождения автомобиля по
правилам». Поэтому внимание исследователей машинного интеллекта
обращается к HPC, high performance computing и универсальным
аппроксиматорам, вычисления с которыми ведутся на этих компьютерах.

Новые универсальные алгоритмы отличаются тем, что сами функции не
программируются/моделируются/описываются вручную/аналитически, но
познаются/выучиваются/learn/вычисляются компьютером при минимальном
вмешательстве человека. Универсальные алгоритмы нейронных сетей, когда
применяются вместо традиционных «императивных» алгоритмов моделирования
физических процессов, могут давать ускорение до миллиона раз на
аналогичной
аппаратуре^[<https://www.sciencealert.com/a-new-neural-network-solved-the-hardest-of-maths-problems-a-million-times-faster>].

Распознавание речи, изображений, поиск аномалий (тут нюанс: аномалия
характеризуется тем, что нужно распознать не то, что компьютер уже
видел, а наоборот --- то, чего он ещё не видел!) компьютер делает уже
лучше, чем человек.

После того, как универсальные алгоритмы упёрлись в барьер по ресурсам,
начались массовые работы по оптимизации этих алгоритмов. Так,
выяснилось:

-   Есть зависимость между размером данных для обучения и размером
    нейронной сети. Огромные сети языковых моделей первого поколения
    (2018-2023) на 175 миллиардов обучаемых весов оказались банально
    недообучены, для полного использования такого размера сетей нужно
    было бы больше данных, больше вычислений, учить нужно было бы ещё
    дольше и больше. Поэтому можно для тех же результатов для одного
    размера обучающих данных брать нейросети поменьше  --- и за меньшие
    деньги получать «умные» большие языковые модели. Другой резерв  ---
    использование данных с меньшей разрядностью (не 32 разряда, а 16
    разрядов, не плавающие, а целые 8 разрядов или даже плавающие 8
    разрядов, а современные предложения  --- обойтись 3-4 разрядами!).
-   Если хочется сделать сеть поумнее, нужно выполнить все рекомендации
    предыдущего пункта (для эффективности!), но поднять размер сети
    (число весов) и поднять размер данных для обучения, причём данные
    нужно брать «от людей», а не
    сгенерированные^[<https://arxiv.org/abs/2305.17493>]!

А алгоритмы творчества есть такие? Если вернуться к универсальным
алгоритмам, которые работают с универсальными аппроксиматорами, могут ли
они творить? Да, могут. Творчество идёт по тому же пути, что и эволюция:
в шуме (например, шуме, получаемом при помощи генератора случайных чисел
на тепловом/квантовом шуме, чтобы надёжно этот шум был свободен от любых
закономерностей) потенциально содержится всё новое, что может быть
придумано в мире. И дальше можно просто модифицировать этот шум так,
чтобы он попал под необходимые ограничения. Если немного
поманипулировать со сжатием информации
(моделированием/онтологизацией/абстрагированием) и последующим разжатием
(демоделированием/рендерингом/конкретизацией), то вычислительно это всё
может быть вполне осмысленным, «воображение» шума бесконечно
разнообразно!

Если каждый алгоритм распознавания основывается на какой-то модели,
сохраняющей знания о важном для распознавания аспекте входных сигналов,
то можно всегда предложить алгоритм порождения, который в выходном
сигнале сохранит это важное --- алгоритм распознавания признает
творчески сгенерированный новый объект «своим». Алгоритм GAN (generative
adversarial network, порождающей соревновательной сети) устроен примерно
так: тренируют подалгоритм распознавания, и на вход ему подают шум от
подалгоритма генератора --- распознаватель говорит «это не то» и
сообщает генератору, что ему особо не понравилось. Генератор
подстраивает свой выход, чтобы понравиться распознавателю --- и так
много раз, пока ему не удаётся обмануть распознаватель и подсунуть вроде
как «то». Если распознаватель умеет распознавать картины Ван Гога, то
генератор в конце концов сумеет сделать картину, которую и человек, и
этот распознаватель (качество работы распознавателей сейчас может быть
при надлежащем их обучении не хуже, чем у людей) признают, как картину
Ван Гога, но готовил эту картину не Ван Гог, а генератор. Это и есть
алгоритмика: придумать такого сорта алгоритм, как этот
GAN^[<https://en.wikipedia.org/wiki/Generative_adversarial_network>]!

Коннективистские модели (однородные вычислительные алгоритмы,
подразумевающие распределение вычислений по многим мелким элементам,
типа нейронных сетей) тоже по факту включены в информатику. Авторы
алгоритмов обучения нейронных сеток ЛеКун, Бенжио и Хинтон стали
лауреатами Тьюринговской премии 2018
года^[<https://awards.acm.org/about/2018-turing>],
то есть машинный интеллект (занимающийся мышлением-не-в-человеке)
признали частью computer science и software engineering в профильной
ассоциации, Association for Computing Machinery.

По мере ухода всей науки/science в компьютеры вполне возможно, что
«наука» как «познание» будет по-английски называться learning (обучение
алгоритма-интеллекта решать какие-то классы задач), а в пределе ---
self-supervising learning (обучение без учителя, по собственной
инициативе, используя научное мышление --- выдвигая гипотезы и проводя
эксперименты). По мере ухода инженерии в компьютеры она будет называться
search (поиск инженерного решения в пространстве решений как поиск
оптимума функции). Всё это будет алгоритмика обучения и поиска, computer
science, а мышление на эти темы --- computer thinking/вычислительное
мышление.

В алгоритмике вычисления ведутся над данными. В data science обсуждаются
разные алгоритмы работы с данными прежде всего --- хотя предметом вроде
как являются сами данные. Данные стали весьма и весьма «кучерявыми»,
отражающими результаты больших проектов корпоративного моделирования и
множество уровней мета-моделирования: поглядим на корпоративные базы
данных, составленные из десятков тысяч таблиц, или представленные
графами знаний на сотни миллионов узлов! Одна из популярных методологий
разработки корпоративного софта Domain driven design
(DDD)^[<https://en.wikipedia.org/wiki/Domain-driven_design>]
по факту представляет собой моделирование предметной области работы
компании, и результаты этого моделирования отражены обычно в сложных
структурах баз данных --- там используются главным образом предыдущие
перед алгоритмикой дисциплины интеллект-стека. Но затем эти данные
всё-таки нужно обрабатывать, как-то их использовать. И вот тут пока
работают относительно простые алгоритмы, но не факт, что так будет
всегда. Алгоритмы обработки этих данных могут быть вполне сложными!
Вычислительное мышление оказывается не столько про собственно
вычисления, но и про виды моделей, над которыми эти вычисления могут
проводиться --- оно неразрывно связано с мышлением про данные, про
поддерживаемые экзокортексом модели. Пока простые, но непрерывно
усложняющиеся алгоритмы вывода/оценки/вычислений над сложными моделями
мира, выраженными в данных --- и вот эти сложные алгоритмы, похоже,
будут реализованы как настройки параметров для универсальных алгоритмов.

Как и вся остальная мыслительная деятельность,
вычислительное/алгоритмическое мышление само по себе начинает
поддерживаться компьютерами с универсальными алгоритмами, это предмет
сегодняшней программной инженерии, базирующейся прежде всего на
современной алгоритмике. У людей постепенно будет исчезать рутинная
инженерная/программистская работа по написанию программного кода,
настроек нейронной сети, описанию каких-то компьютерных сложных
процедур, и можно будет больше времени посвятить чему-то другому.
Землекопы не жалеют, что их работу взял на себя экскаватор.
Экскаваторщик не будет жалеть, что работу экскаватора берёт на себя
автопилот экскаватора. Программисты не будут жалеть, что написание
программного кода берут на себя программы. Но всем остальным людям
планеты нужно понимать, что происходит: когда нужно вырыть канаву или
котлован, к кому обращаться  --- рыть самому, обращаться к землекопу,
экскаваторщику, экскаватору с прилагающимся к нему экскаваторщику? Когда
нужно разработать информационную систему, к кому нужно обращаться  ---
разрабатывать самому, обращаться к программисту, программирующему AI с
прилагающимся к нему программисту?

Классическая информатика по факту занималась изучением алгоритмов
перекодирования: как из одного компьютерного кода получить другой
компьютерный код (компиляция программ на языках программирования). Речь
в вычислительном мышлении идёт главным образом о расширении этого
понимания до менее формальных текстов.
