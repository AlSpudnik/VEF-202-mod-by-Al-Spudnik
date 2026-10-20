<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/IMG_20261002_144313254.jpg" width="400">

### Оригінальні данні VEF 202:

[![Посібник з експлуатації](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Посібник%20з%20експлуатації-white.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/IMG_20230224_120251051.png)

[![Схема 1973](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Схема_1973-red.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/vef202original_scheme.png)

[![Layout IF, Power Amp](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Layout_IF,_Power_Amp-orange.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/vef_layout.jpg)

[![Таблиця катушок](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Таблиця_катушок-blue.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/VEF206.jpg)

[![Трансформатори](https://img.shields.io/badge/Ctrl_+_клік_мишкою-НЧ_Трансформатори-green.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/Плата_ПЧ/vef_transformer.png)


### VEF 202 mod by Al Spudnik

[![Модифікована схема_від Al Spudnik](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Модифікована_схема_від_Al_Spudnik-orange.svg )](https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/VEF202_by_Spudnik_v1.1.svg)

Відновлення плати ПЧ, НЧ. 

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/%D0%9F%D0%BB%D0%B0%D1%82%D0%B0_%D0%9F%D0%A7/plate01.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/%D0%9F%D0%BB%D0%B0%D1%82%D0%B0_%D0%9F%D0%A7/plate02.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/%D0%9F%D0%BB%D0%B0%D1%82%D0%B0_%D0%9F%D0%A7/plate03.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/%D0%9F%D0%BB%D0%B0%D1%82%D0%B0_%D0%9F%D0%A7/plate04.jpg" width="400">


Частотозадавальні та зв'язкові конденсатори (Ємності від одиниць до сотен пікофарад). Це конденсатори, які стоять безпосередньо всередині коливальних контурів ПЧ (наприклад, паралельно котушкам у металевих екранах) або в каскаді гетеродина.

• Рішення: Ставити туди китайську жовту кераміку «крапельки» класу X7R / Y5V категорично не можна!

• У чому небезпека: Найдешевша китайська кераміка (діелектрики Y5V, Z5U, X7R) сильно змінює свою ємність навіть від легкого подиху тепла. Якщо ви запаяєте таку «крапельку» в контур ПЧ (проміжної частоти 465 кГц), контур повністю розлаштується, приймач втратить чутливість, а частота буде постійно «пливти» в міру нагрівання транзисторів.

- Перевірте за схемою: якщо там стоїть слюдяний КСО чи трубчастий КТ — залишайте їх рідними.
	
- Якщо там раптом виявиться паперовий конденсатор (БМТ-2, МБМ), його можна замінити виключно на кераміку з діелектриком NP0 (C0G). Вони термостабільні. Зовні такі імпортні конденсатори зазвичай виглядають як маленькі однотонні диски сірого, білого або світло-коричневого кольору із чорною цяткою на торці, або на них прямо вказано маркування «NP0».

Китайську жовту кераміку «крапельки» класу X7R / Y5V встановлюйте у блокувальні ланцюги (фільтри живлення каскадів).

Наприклад:

• Конденсатор у ланцюгах автоматичного регулювання посилення (АРУ).

• Конденсатори, що шунтують резистори в емітерах транзисторів ПЧ для усунення зворотного зв'язку за ВЧ.

• Фільтри по шині живлення високочастотної частини.

У цих точках жовта кераміка спрацює ідеально, бо її завдання — просто «коротити» високочастотне сміття на масу, і плавання ємності на 10-20% там ні на що не впливає.

Радянські дискові конденсатори випускалися з різними типами кераміки. На них є позначення ТКЄ (температурного коефіцієнта). Подивіться на їхній корпус:

• Літери «П33», «М47», «М75» або кольорова крапка (синя, зелена, чорна): Це високостабільна термокомпенсаційна кераміка. За своїми властивостями це аналог сучасного діелектрика NP0 / C0G. Вони мають ємність від одиниць до кількох сотень пікофарад.

• Літери «Н30», «Н50», «Н90»: Це низькочастотна кераміка з високою діелектричною проникністю (аналог сучасних X7R / Y5V). Вони зазвичай мають ємність від 1000 пФ (1 нФ) до 0,047 мкФ. Вони сильно пливуть від температури.

Polypropylene Safety Plastic Film 100V, фольговий лавсан К73-15А значно кращі за К73-17 у високочастотних колах. У міжкаскадні зв'язкові ланцюги (УВЧ та ПЧ) сигнал пройде без втрат і ємність не буде «пливти» від температури.

Фільтр зосередженої селективності (ФЗС):

Увага! Навіть попри те, що поліпропілен стабільніший за лавсан, він усе одно програє слюді (КСО). Тому залізне правило залишається: у самому ФЗС та гетеродинних контурах не міняйте рідні КСО ні на К73-17, ні на CBB.

Коротке резюме для монтажу

• Усе, що фільтрує Колектор та Живлення котушок на землю: Ставимо жовту кераміку «крапельки» класу X7R / Y5V (боротьба з ВЧ/УКХ збудженням транзисторів).

• Усе, що фільтрує Базу, АРП та котушки зв'язку баз: Ставимо Плівкові квадратики (стабільність часу АРП, захист від мікрофонного ефекту та термодрейфу робочих точок), фольговий лавсан К73-15А, або керамічний конденсатор з діелектриком класу NP0 (або C0G).

С51 - кераміка «крапелька» (MLCC) з діелектриком X7R (допуск K — ±10%)

Обмотки НЧ трансформаторів збільшені.
- Тр.1:
- 1-2 = 1570 витків
- 3-4 = 462 витка
- 4-5 = 462 витка
- Тр.2:
- 1-2 = 128 витків
- 3-4 = 400 витків
- 4-5 = 400 витків
- 6-7 = 128 витків

ЧМ (FM) плата:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/FM Board/FMboard.jpg" width="400">

Звільнити 13-ий контакт на ДX (LW) та СХ (MW) платах для аудіовиходу ЧМ модуля:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/FM Board/MWboard.jpg" width="400">

- Покрокове складання:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair01.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair02.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair03.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair04.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair05.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair06.jpg" width="400">

- Ноніусний механізм:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair07.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair09.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair08.jpg" width="400">

- Електронний вимикач освітлення шкали та живлення ЧМ (FM) плати:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/electric_keys/repair11.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/electric_keys/repair12.jpg" width="400">

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/repair10.jpg" width="400">

[![Налаштування ПЧ](https://img.shields.io/badge/Ctrl_+_клік_мишкою-Налаштування_ПЧ-orange.svg )](https://github.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/blob/main/%D0%9F%D0%BB%D0%B0%D1%82%D0%B0_%D0%9F%D0%A7/%D0%86%D0%BD%D1%84%D0%BE_%D0%BF%D0%BE_%D0%9F%D0%A7.md)

- Зібраний в корпус:

<img src="https://raw.githubusercontent.com/AlSpudnik/VEF-202-mod-by-Al-Spudnik/main/photo/IMG_20261002_144321573.jpg" width="400">

<https://mrspudnik.blogspot.com>
