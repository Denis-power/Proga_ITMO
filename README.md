# Proga_ITMO

# Лабораторная работа #3

Вариант: 340290

Описание предметной области, по которой должна быть построена объектная модель:

А Снифф глубоко вздохнул и сказал: Король рубинов сверкал красным глазом на окутанной ночной тьмою Земле, и Волшебник на Луне заметил его. Он уже совсем было отказался от дальнейших поисков. Усталый и печальный, отдыхал он на краю кратера, а его черная пантера спала поодаль. Он сразу понял, что это сверкает красным там, на Земле. Самый большой рубин на свете, Король рубинов, который он проискал не одну сотню лет! Не спуская с Земли горящего взора, он вскочил, натянул перчатки и набросил на плечи плащ. Собранные в него драгоценные камни он попросту вытряхнул -- ведь его интересовал один-единственный самоцвет и он рассчитывал меньше чем через полчаса держать его в своих руках.

Программа должна удовлетворять следующим требованиям:
    
    Доработанная модель должна соответствовать принципам SOLID.
    Программа должна содержать как минимум два интерфейса и один абстрактный класс (номенклатура должна быть согласована с преподавателем).
    В разработанных классах должны быть переопределены методы equals(), toString() и hashCode().
    Программа должна содержать как минимум один перечисляемый тип (enum).

# Лабораторная работа #4

Доработать программу из лабораторной работы #3, обновив реализацию объектной модели в соответствии с новой версией описания предметной области.

Вариант: 340290.3

Описание предметной области, по которой должна быть построена объектная модель:

Уж полночь прошла, как вдруг весь сад озарился розовым светом. Танцы приостановились: все решили, что это какой-то новый вид фейерверка. Но это просто Тофсла и Вифсла открыли свой чемодан. Король рубинов, сверкая, лежал на лужайке, прекрасный как никогда. Все огни, фонари и даже сама луна померкли, потеряли свой блеск. В благоговейном молчании пылающий самоцвет обступала все более густая и многочисленная толпа. А Снифф глубоко вздохнул и сказал: Король рубинов сверкал красным глазом на окутанной ночной тьмою Земле, и Волшебник на Луне заметил его. Он уже совсем было отказался от дальнейших поисков. Усталый и печальный, отдыхал он на краю кратера, а его черная пантера спала поодаль. Он сразу понял, что это сверкает красным там, на Земле. Самый большой рубин на свете, Король рубинов, который он проискал не одну сотню лет! Не спуская с Земли горящего взора, он вскочил, натянул перчатки и набросил на плечи плащ. Собранные в него драгоценные камни он попросту вытряхнул -- ведь его интересовал один-единственный самоцвет и он рассчитывал меньше чем через полчаса держать его в своих руках. Пантера с хозяином на спине поднялась в воздух.

Программа должна удовлетворять следующим требованиям:

    В программе должны быть реализованы 2 собственных класса исключений (checked и unchecked), а также обработка исключений этих классов.
    В программу необходимо добавить использование локальных, анонимных и вложенных классов (static и non-static).

# Лабораторная работа #5

Вариант: 1231

Реализовать консольное приложение, которое реализует управление коллекцией объектов в интерактивном режиме. В коллекции необходимо хранить объекты класса HumanBeing, описание которого приведено ниже.


Разработанная программа должна удовлетворять следующим требованиям:

    Класс, коллекцией экземпляров которого управляет программа, должен реализовывать сортировку по умолчанию.
    Все требования к полям класса (указанные в виде комментариев) должны быть выполнены.
    Для хранения необходимо использовать коллекцию типа java.util.LinkedHashSet
    При запуске приложения коллекция должна автоматически заполняться значениями из файла.
    Имя файла должно передаваться программе с помощью: переменная окружения.
    Данные должны храниться в файле в формате csv
    Чтение данных из файла необходимо реализовать с помощью класса java.util.Scanner
    Запись данных в файл необходимо реализовать с помощью класса java.io.PrintWriter
    Все классы в программе должны быть задокументированы в формате javadoc.
    Программа должна корректно работать с неправильными данными (ошибки пользовательского ввода, отсутсвие прав доступа к файлу и т.п.).

В интерактивном режиме программа должна поддерживать выполнение следующих команд:

    help : вывести справку по доступным командам
    info : вывести в стандартный поток вывода информацию о коллекции (тип, дата инициализации, количество элементов и т.д.)
    show : вывести в стандартный поток вывода все элементы коллекции в строковом представлении
    add {element} : добавить новый элемент в коллекцию
    update id {element} : обновить значение элемента коллекции, id которого равен заданному
    remove_by_id id : удалить элемент из коллекции по его id
    clear : очистить коллекцию
    save : сохранить коллекцию в файл
    execute_script file_name : считать и исполнить скрипт из указанного файла. В скрипте содержатся команды в таком же виде, в котором их вводит пользователь в интерактивном режиме.
    exit : завершить программу (без сохранения в файл)
    add_if_min {element} : добавить новый элемент в коллекцию, если его значение меньше, чем у наименьшего элемента этой коллекции
    remove_greater {element} : удалить из коллекции все элементы, превышающие заданный
    remove_lower {element} : удалить из коллекции все элементы, меньшие, чем заданный
    group_counting_by_real_hero : сгруппировать элементы коллекции по значению поля realHero, вывести количество элементов в каждой группе
    count_by_impact_speed impactSpeed : вывести количество элементов, значение поля impactSpeed которых равно заданному
    filter_greater_than_soundtrack_name soundtrackName : вывести элементы, значение поля soundtrackName которых больше заданного

Формат ввода команд:

    Все аргументы команды, являющиеся стандартными типами данных (примитивные типы, классы-оболочки, String, классы для хранения дат), должны вводиться в той же строке, что и имя команды.
    Все составные типы данных (объекты классов, хранящиеся в коллекции) должны вводиться по одному полю в строку.
    При вводе составных типов данных пользователю должно показываться приглашение к вводу, содержащее имя поля (например, "Введите дату рождения:")
    Если поле является enum'ом, то вводится имя одной из его констант (при этом список констант должен быть предварительно выведен).
    При некорректном пользовательском вводе (введена строка, не являющаяся именем константы в enum'е; введена строка вместо числа; введённое число не входит в указанные границы и т.п.) должно быть показано сообщение об ошибке и предложено повторить ввод поля.
    Для ввода значений null использовать пустую строку.
    Поля с комментарием "Значение этого поля должно генерироваться автоматически" не должны вводиться пользователем вручную при добавлении.

Описание хранимых в коллекции классов:

    public class HumanBeing {
        private Long id; //Поле не может быть null, Значение поля должно быть больше 0, Значение этого поля должно быть уникальным, Значение этого поля должно генерироваться автоматически
        private String name; //Поле не может быть null, Строка не может быть пустой
        private Coordinates coordinates; //Поле не может быть null
        private java.time.LocalDateTime creationDate; //Поле не может быть null, Значение этого поля должно генерироваться автоматически
        private Boolean realHero; //Поле не может быть null
        private boolean hasToothpick;
        private double impactSpeed;
        private String soundtrackName; //Поле не может быть null
        private double minutesOfWaiting;
        private Mood mood; //Поле может быть null
        private Car car; //Поле не может быть null
    }
    public class Coordinates {
        private Double x; //Значение поля должно быть больше -213, Поле не может быть null
        private Long y; //Поле не может быть null
    }
    public class Car {
        private Boolean cool; //Поле может быть null
    }
    public enum Mood {
        SORROW,
        LONGING,
        GLOOM,
        APATHY,
        CALM;
    }
