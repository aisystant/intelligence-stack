---
title: Мета-моделирование aka онтологическая инженерия и место математики и физики
---

Из семантики мы уже понимаем, что нам нужно иметь какие-то
идеальные/ментальные/математические объекты (понятия), знаки для этих
понятий, а также объекты реального/физического мира, обозначаемые
знаками/символами. И тогда их все можно связать друг с другом, чем и
занимается семантика как «теория B» компьютерной науки. Это даёт
возможность определить отдельные дисциплины для тех объектов, которые
потом связываются семантикой:

-   **Математика** изучает поведение ментальных/идеальных/математических
    объектов
-   **Физика** изучает поведение объектов реального/физического мира
-   **Семиотика** изучает поведение знаков (нейросемиотика изучает
    знаки, чьё поведение определяется нейросетями)

Семантика устанавливает отношения между объектами, определяемыми этими
разными дисциплинами. Эти дисциплины сами по себе не являются частями
семантики. Хотя иногда семиотику в состав семантики включают, но отнюдь
не всегда. Да ещё иногда и семантику считают не отдельной дисциплиной, а
частью информатики/computer science, а саму информатику считают
познанием/исследованием того, насколько физические объекты-вычислители
могут своим поведением моделировать поведение математических
объектов^[<https://www.litres.ru/devid-doych/nachalo-beskonechnosti-obyasneniya-kotorye-menyaut-mir/>]
(это не такой тривиальный вопрос для создателей компьютеров, например,
оптических^[<https://en.wikipedia.org/wiki/Optical_computing>],
квантовых^[<https://en.wikipedia.org/wiki/Church%E2%80%93Turing%E2%80%93Deutsch_principle>]
или даже биологических на
нейросетях^[<https://www.frontiersin.org/journals/science/articles/10.3389/fsci.2023.1017235>]).

Математика как практика (роль практикующего математику ---
«**математик**») изучает поведение идеальных/ментальных объектов: какие
они могут быть, как могут создаваться (construct, конструироваться), как
преобразовываться друг в друга, какие у них могут быть свойства. Что не
изучает математика, так это связь этих объектов с окружающим миром:

-   В физике математические объекты служат для описания поведения
    физических объектов, математика тем самым --- язык естественных
    наук. Это основная цель математики: давать хорошо изученные
    ментальные/математические объекты (геометрические точки, поля,
    тензоры), поведение которых может быть использовано для
    формального/строгого/точного описания поведения объектов окружающего
    физического мира. Есть на эту тему замечательная статья про
    немыслимую эффективность математики в естественных
    науках^[<https://en.wikipedia.org/wiki/The_Unreasonable_Effectiveness_of_Mathematics_in_the_Natural_Sciences>].
    Но математика используется готовой.
-   В информатике/вычислительной науке/computer science математические
    объекты служат предметом рассмотрения того, насколько точно и
    насколько полно физические объекты-вычислители могут моделировать их
    поведение. Математика опять же используется уже какая есть, как
    устоявшаяся уже дисциплина. Это обратная задача: **в естественных
    науках (и, в частности,** **физике) мы подбираем математические
    объекты, чтобы выразить поведение физических объектов, а в
    информатике мы подбираем физические объекты, чтобы выразить
    поведение математических объектов.**

Это взрослым людям кажется, что тут всё прозрачно и понятно. Но если
взять ребёнка, которому нужно посчитать в компьютерной программе, на
какой угол надо повернуть мотор робота, чтобы тот прошёл заданный путь,
то быстро выяснится:

-   Ребёнок отлично понимает всё про физического робота и путь (это
    буквально бытовое знание, но и физика это изучает)
-   Ребёнок отлично понимает всё про математические формулы, по которым
    надо будет считать путь: что там с диаметром круга, пи, окружностью,
    углами
-   Ребёнок отлично программирует: пишет программы с циклами, формулами,
    вызовами подпрограмм.
-   Ребёнок абсолютно не понимает, каким образом описание поведения
    физического робота можно выразить математическими формулами, с
    которыми можно много чего интересного делать (по одной величине
    определять другую величину, и наоборот), а затем каким образом можно
    эти формулы писать в программе, чтобы получить нужное значение, и
    затем каким образом формулы-из-программы вдруг становятся поведением
    реального робота. Это знание даётся ребёнку в конечном итоге
    «исподволь», путём решения десятка похожих задач. Но если чуть-чуть
    пошевелить условия (перейти на язык программирования с другой
    парадигмой вычислений, робот будет другого типа, физика будет не
    механикой), то всё надо будет повторять. Интуиция какая-то будет, но
    она будет сбоить. А если традиционный компьютер заменить квантовым,
    то и у взрослого будут затруднения: что там в реальном физическом
    мире, какая там должна быть математика (иногда говорят даже «какая
    там физика», имея в виду математические формулы), как эту математику
    выражать в программе, чтобы добиться нужных изменений в реальном
    мире. Если идти в какую-нибудь вычислительную оптику, то с этими
    задачами только специалисты справятся --- вопрос только в том, как
    они научились так думать, чтобы справляться?

Если забежать вперёд в **онтологию**, которая рассказывает об описании
мира на разных уровнях абстракции (само описание мира --- это задача
физики и других естественных наук, а вот какие объекты брать в мире,
чтобы их описывать и какие методы описания брать для этого --- это
задача «над физикой», как раньше говорили, «метафизика». Онтология ---
это извод метафизики, эпистемология (рациональное познание) --- это
способ, которым мы создаём онтологии, «как узнаём, какие объекты надо
брать в физическом мире, чтобы их потом описывать объектами
математического/ментального мира»). Это всё мы будем рассматривать
дальше по интеллект-стеку, но там везде уже потребуется математика как
универсальный пополняемый язык, на котором может вестись описание чего
угодно (в том числе и описание описаний).

Математика --- это мета-мета-мета-модель/теория/абстракция/онтология для
science, естественных наук. Понятия/онтологии/описания самих
естественных наук --- это мета-мета-модели («из учебников
фундаментальных наук»), прикладных/деятельностных/инженерных/трудовых
предметных областей --- мета-модели, описания объектов конкретных
ситуаций (экземпляров) --- модели. Материал про многоуровневое
мета-моделирование (оно же --- онтологическая инженерия, применение
его --- многоуровневое применение операции присвоения типа,
задействование «машинки типов») описывается в онтологии, вместе с
нюансами о том, что сама онтология --- это про объекты окружающего мира
или про описания объектов окружающего мира. Нюанс в том, что онтологией
сейчас более чем часто называют онтологическое описание (определение по
Gruber, Borst, and Studer: «ontology is a formal, explicit specification
of a shared conceptualization», спецификация::описание), но и раньше, и
сейчас онтологией называлась нарезка на объекты самого мира, а не
описание этой нарезки. Но об этом подробней уже в курсе онтологии, а тут
пока важно, что математика как раз должна дать типы объектов для
строгого/formal явного/explicit specification/описания общей для разных
агентов (служащей для целей обсуждения/коммуникации/коллективного
мышления и действия) концептуализации/набора понятий. То есть математика
должна дать описания интересных объектов идеального мира.

Что это за такие «интересные объекты»? Дело в том, что математика может
выдумывать любые объекты, это же «ментальный мир», мир выдумки. Но
большинство объектов будут неинтересными. Поэтому математики ищут
«интересные» объекты, которые ведут себя как-то контринтуитивно. К
сожалению, понятие «интересных объектов» не формализуется, оно даётся
через обучение будущих математиков работой с нынешними математиками и
этот поиск интересных объектов неожиданно оказывается сопряжён с путями
организации математического труда (математического познания,
математических исследований) учёными-математиками. Например, как
описывает Роман Михайлов, математик должен продемонстрировать, что он
понимает суть математики, решив одну из проблем, оставленных великими
математиками прошлого. Это просто «сдача экзамена» на то, что математик
может отличить «**интересное**» от «банального». Дальше такой математик
получает не только право, но чуть ли не обязанность поставить какие-то
проблемы перед следующими поколениями математиков --- ибо он доказал
решением предыдущих проблем своё право судить о том, что является
интересным, а что нет, какие проблемы считать интересными для решения и
достойными вложения труда, а какие нет. В том числе по Михайлову глубоко
неправ Михаил Перельман, который одну из проблем прошлого решил, но свои
проблемы не предложил. Дальше, конечно, сразу ставится задача
определения «интересного» --- но это же задача дисциплины
познания/исследований в целом (там даже есть теория
любопытства/curiosity), это даже не предмет математики как дисциплины,
математики просто пользуются этим понятием, когда занимаются
математическими исследованиями.

Так что с точки зрения употребления математики --- она поставщик
описаний важных объектов внимания (типов
мета-мета-мета-модели/foundational ontology, а в прикладной части ---
мета-мета-модели/upper ontology) для рассуждения об объектах внимания
естественных наук/sciences как типах мета-мета-модели и далее объектах
каких-то прикладных инженерных практик как мета-моделях.

Так что у естественных наук уровень моделирования/онтологический
уровень/уровень абстракции/уровень по отношениям классификации примерно
тот же, что у моделей трансдисциплинарного методологического стека
(мета-мета-модель/upper ontology с заходами на middle ontology), физика
при этом просто входит в интеллект-стек, а другие науки входят как
основания для инженерных/трудовых практик создания объектов какого-то
масштаба и сложности --- химия для вещества, биология для существа, и
так далее. С одной стороны, это немного кривовато (много стройней было
бы указание «метафизики» в интеллект-стеке фундаментальных
трансдисциплин и разных вариантов «физик» в инженерных практиках, ибо
квантовая физика микромира связана сегодня с малым масштабом, теория
относительности с большим космическим масштабом, общей физики как-то ещё
нет, только «принципы» --- то есть метафизика), но интуитивно понятно,
что всё-таки физика как базисная дисциплина на уровне **принципов**
(«законов о законах» --- принципы симметрии, принципы сохранения и
т.д.), а не законов для отдельных явлений, которые могут быть
использованы в инженерии, должна быть в интеллект-стеке. А вот
прикладная физика --- это как раз отдельные «законы», она идёт в
прикладные/инженерные практики, наряду с химией и приложениями механики
для механической инженерии.

Вот ещё раз про то же самое и чуть-чуть примеров (по-прежнему забегая
вперёд: мы не обсуждаем сейчас содержание математики, мы обсуждаем для
чего эта математика потребуется, поэтому хотим, чтобы она была такой,
какая сможет потом пригодиться. Даже число уровней и их именование ---
предмет обсуждения):

-   **M3, мета-мета-мета-модель** --- foundational ontology, «основания
    математики» (чаще всего это логика, но отнюдь не все математики
    логицисты, о foundational ontology в математике договориться пока
    невозможно по совокупности причин), язык формального описания самой
    математики. На этом уровне определяются объекты и их группы,
    предикаты, субъекты, термы, а ещё и как это всё выражается (имена и
    прочее про «форму» из «формальности», как у Spencer-Brown с его Laws
    of
    Form^[<https://www.goodreads.com/book/show/584140.Laws_of_Form>]).
-   **M2, мета-мета-модель** --- описание типов в методологической
    трансдисциплине, включая математику как типы для физики на уровне
    принципов (законов о законах). Система::объект, который включён в
    состав надсистемы::объекта и выполняет функцию::предикат. Дисциплины
    интеллект-стека главным образом определяются на этом уровне.
-   **M1, мета-модель** --- описание типов объектов в прикладном (из
    практики инженерного стека, включая законы физики, химии и т.д., и
    там подтипы от кругозорной практики до прикладных практик уровня
    стандарта предприятия) domain. «Вот это стол --- за ним едят, вот
    это стул --- на нём сидят», при этом «Вот это стол::система --- за
    ним едят::функция, вот это стул::система, за ним сидят::функция».
    Можно ввести два подуровня, метаУ-модель как именно «научная
    дисциплина/теория из Учебника» и метаС-модель как «Ситуационная
    модель/теория/онтология предметной области конкретного проекта», как
    это принято в конкретном проекте, возможно даже уникально на одном
    предприятии, объекты вводимые, например, только регламентом какой-то
    службы.
-   **M0, модель** --- описание свойств экземпляров объектов физического
    мира. «Стол обеденный номер 5, стул кухонный номер 10», при этом
    «Стол обеденный номер пять»::стол, «стул кухонный номер 10»:: стул.
-   И не забываем, что есть ещё и **физические
    объекты/экземпляры/индивиды**, и как связана модель/M0 с этими
    объектами, будет обсуждать семантика, а как операции с этими
    объектами (взаимодействия физических объектов) отражаются операциями
    с описаниями (вычисления в физическом объекте-компьютере) --- это
    будет предмет computer science.

**Языком, на котором всё это будет обсуждаться,** **как раз и** **будет
математический язык: основные объекты, которые предлагает математика
(множества, категории, топосы и т.д.).**

Дальше можно обсуждать, надо ли щепить M3 на отдельно «M4 --- основания
математики» и «M3 --- математика» примерно так же, как щепим «физику на
уровне принципов» и «прикладную физику как законы» по разным уровням. Но
пока не будем этого делать: foundational ontology и upper ontology
всё-таки относительно искусственное разделение (онтология тем и хороша,
что «модель данных и данные --- это просто разные уровни одной
онтологии», в отличие от моделирования данных в классических базах
данных, где данные отдельно, а модель данных отдельно, потому как живут
в разных мирах моделирования). Мегамодель какой-нибудь ситуации включает
в себя все эти мета-уровни.
