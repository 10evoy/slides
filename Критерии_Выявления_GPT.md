# Критерии выявления GPT в тексте

В данном документе представлены основные критерии, позволяющие определить, был ли текст создан с помощью генеративных моделей искусственного интеллекта, таких как GPT (Generative Pre-trained Transformer).

## 1. Шаблонность и предсказуемость структуры

**Демонстрация:** Тексты, созданные GPT, часто имеют четкую, предсказуемую структуру: введение, основная часть с несколькими подпунктами, заключение.

**Конкретный пример:**
```
Вопрос: "Расскажите о влиянии социальных сетей на подростков"

Ответ GPT: 
"Влияние социальных сетей на подростков является многогранной темой, вызывающей интерес исследователей и общественности. 

Во-первых, социальные сети могут оказывать положительное влияние, предоставляя подросткам возможности для общения и самовыражения. Они позволяют поддерживать связь с друзьями и находить единомышленников.

Во-вторых, существуют негативные аспекты, такие как кибербуллинг, проблемы с самооценкой из-за сравнения себя с идеализированными образами, и потенциальная зависимость от социальных платформ.

В-третьих, исследования показывают связь между временем, проведенным в социальных сетях, и психологическим благополучием подростков.

В заключение, важно находить баланс в использовании социальных сетей и развивать цифровую грамотность среди подростков."
```

## 2. Отсутствие уникального авторского стиля

**Демонстрация:** GPT генерирует тексты в нейтральном, обобщенном стиле, лишенном индивидуальных особенностей.

**Конкретный пример:**
```
Вопрос: "Ваше мнение о романе 'Преступление и наказание'"

Ответ GPT:
"Роман 'Преступление и наказание' Федора Михайловича Достоевского является одним из величайших произведений мировой литературы. Автор мастерски исследует психологию главного героя, Родиона Раскольникова, и поднимает важные философские вопросы о морали, вине и искуплении. Роман отличается глубоким психологическим анализом и сложной структурой повествования. Достоевский умело переплетает различные сюжетные линии, создавая многогранное произведение, которое остается актуальным и в наше время."
```
Человек-критик, скорее всего, выразил бы более субъективное мнение, используя личные впечатления, эмоциональные оценки и нестандартные интерпретации.

## 3. Избыточная вежливость и формальность

**Демонстрация:** Тексты GPT часто содержат избыточные вежливые формулировки и формальные обороты.

**Конкретный пример:**
```
Вопрос: "Как приготовить борщ?"

Ответ GPT:
"Благодарю за ваш интересный вопрос о приготовлении борща. С удовольствием поделюсь рецептом этого замечательного блюда. Позвольте начать с перечисления необходимых ингредиентов. Вам потребуется: говядина, свекла, капуста, морковь, лук, томатная паста, картофель, специи по вкусу. Хотел бы отметить, что для достижения наилучшего результата рекомендуется использовать свежие овощи. Буду рад, если данный рецепт окажется для вас полезным. Если у вас возникнут дополнительные вопросы, пожалуйста, не стесняйтесь обращаться."
```
Человек обычно написал бы более прямолинейно: "Для борща нужны: говядина, свекла, капуста, морковь, лук, томатная паста, картофель, специи. Сначала варим мясо, потом добавляем овощи..."

## 4. "Галлюцинации" и выдуманные факты

**Демонстрация:** При необходимости предоставить конкретную информацию, которой у GPT нет, модель может "галлюцинировать" - создавать правдоподобные, но выдуманные факты.

**Конкретный пример:**
```
Вопрос: "Расскажите о результатах исследования влияния искусственного интеллекта на рынок труда в России в 2024 году"

Ответ GPT:
"Согласно исследованию, проведенному Российской академией наук в марте 2024 года, внедрение технологий искусственного интеллекта привело к трансформации 23% рабочих мест в России. Исследование, в котором приняли участие 1500 компаний из различных отраслей, показало, что 15% рабочих мест были полностью автоматизированы, в то время как 37% претерпели значительные изменения в требуемых навыках. Директор исследования, профессор Алексей Петров, отметил: 'Наши данные свидетельствуют о том, что ИИ создает больше рабочих мест, чем уничтожает, но требует масштабной переквалификации кадров'."
```
Это выдуманное исследование с конкретными процентами, именем несуществующего профессора и точной цитатой, которые звучат правдоподобно, но являются "галлюцинацией" модели.

## 5. Избегание спорных тем и нейтральность позиции

**Демонстрация:** GPT стремится к нейтральности и балансу мнений по спорным вопросам.

**Конкретный пример:**
```
Вопрос: "Ваше мнение о легализации эвтаназии"

Ответ GPT:
"Вопрос легализации эвтаназии является сложным этическим и правовым вопросом, по которому существуют различные точки зрения.

С одной стороны, сторонники легализации эвтаназии аргументируют свою позицию правом человека на достойную смерть и избавление от невыносимых страданий при неизлечимых заболеваниях. Они указывают на принцип автономии личности и право каждого распоряжаться своей жизнью.

С другой стороны, противники эвтаназии выражают обеспокоенность возможными злоупотреблениями, давлением на уязвимые группы населения и противоречием с клятвой Гиппократа. Они также приводят религиозные и этические аргументы о ценности жизни.

Важно отметить, что в разных странах существуют различные подходы к этому вопросу, от полного запрета до легализации при определенных условиях."
```
Человек, скорее всего, выразил бы более определенную личную позицию по этому вопросу, а не стремился бы к такому тщательному балансу аргументов.