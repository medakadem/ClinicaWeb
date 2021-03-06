# Нормативы анализов

Для того, чтобы работать с формой лаборанта, нужно: <a href="./Price">добавить услуги</a> типа анализ, добавить в эти услуги компоненты, которые будут исследоваться, из списка существующих на вкладке Компоненты анализа.    
  
Чтобы добавить новый компонент анализа, зайдите в "Справочники" - "Анализы" - "Компоненты анализа". Здесь можно редактировать существующий компонент или добавить новый, а также добавить нормы для этого компонента. Для работы с компонентами анализов должны быть созданы Классы и Группы анализов(в один класс может входить несколько групп), а также единицы измерений.   
 Для того, чтобы добавить компонент, нажмите "+", заполните все поля и нажмите "сохранить" в последнем столбце таблицы. Далее нужно добавить нормы для данного компонента. Разверните нужный, нажав на стрелочку возле названия. Здесь Вы сможете создать нормы для конкретных возрастов и различные по полу пациента. Заполните все необходимые поля и сохраните. Вы можете создать отдельно для каждого пола свою норму для каждого диапазона возрастов (возраст вводите только диапазоном). Если же норма зависит только от возраста и одинакова для обоих полов, выберите Универсальный.      
 Для корректной работы с нормативами придерживайтесь правил заполнения:
 1. Если норма являет собой текст, например "не виявлено", вводите лишь этот текст, без цифр, лишних пробелов и других знаков. При заполнении результатов анализа вводите текст точно так, как в норме. *В нашем примере нормой будет считаться только вариант "не виявлено", любое отклонение будет считаться патологией - "виявлено", "Не виявлено" и т.д.*
 2. Если норма представляет собой сравнение с числом, то вводите знак сравнения ("<",">" или "=") и далее без пробела число, с которым сравнить. Дробные числа вводите через точку (50.5). *Например, <25. Тогда результат анализа будет сравниваться с числом 25, и если результат будет меньше 25, он будет входить в норму. В этом примере, если результат будет равняться 25 или будет больше 25, он будет считаться патологией.*      
 Если нормой является одно число, вводите его со знаком "=".
 3. Если норма - интервал чисел, вводите первое(меньшее) число, далее дефис и второе(большее) число без пробелов. В этом случае, результат также можно вводить интервалом чисел. *Пример нормы: "1-10". Пример результата: "5" или "4.5-5". В обоих случаях результат входит в норму.*
 ![Image](Image/components.gif)

В <a href="./labsform">форме лаборанта</a>, и как следствие - в <a href="./PatientCard">карточке пациента</a> автоматически будет отображаться норма в зависимости от возраста и пола пациента. 
