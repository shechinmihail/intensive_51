
# intensive_51

# Задание 1: Реализация своего динамического списка

### Общие требования:
- Клонировать репозиторий https://github.com/SiarheiYurevich/intensive_51
- Создать ветку `task_1_name_surname` от ветки `master`
- Создать Pull Request
- Использовать `.gitignore`

### Задачи:
1. Создать интерфейс `IntensiveList` и класс `ArrayList_NameSurname`, имплементирующий данный интерфейс.
```java
public interface IntensiveList<E> {
    int size();
    void add(E element);
    void add(int index, E element);
    E get(int index);
    E set(int index, E element);
    E remove(int index);
    void clear(); // удаляем все элементы, capacity приводим к дефолтному
    void quickSort(Comparator<E> comparator); // реализуем быструю сортировку, дефолт по возрастанию
    boolean isSorted();
    void split(int size); // обрезаем список до указанного размера
}
```
2. Реализовать методы интерфейса.
3. Задокументировать код на уровне класса и публичных методов (javadoc).

# Задание 2: Реализация аннотации, assertions и test runner

### Общие требования:
- От ветки `master` создать ветку `task_2_name_surname`, создать пакет `task_2`, работать только в своей ветке, создать Pull request.
- Использовать javadoc для документирования кода.

### Задачи:
1. Реализовать аннотацию `@IntensiveTest_NameSurname`.
2. Реализовать класс `Assertions_NameSurname` с статическими методами, например, `assertEquals(List.., List..)`.
3. Реализовать класс `TestRunner_NameSurname`, который сканирует указанные пакеты на наличие методов, аннотированных аннотацией `@IntensiveTest_NameSurname`, и выполняет проверку тестов - запускает тестовые методы.
4. Написать тест для проверки является ли массив отсортированным:
    - Создать класс `IntensiveArrayListTest_NameSurname`.
    - Создать метод `test`, аннотированный аннотацией `@IntensiveTest_NameSurname`, выполняющий проверку является ли массив `IntensiveArrayList_NameSurname` отсортированным.
    - В методе `main` выполнить проверку: создать класс `TestRunner_NameSurname` и передать ему список пакетов, запустить его метод `run`, в консоль должно быть выведено сообщение о результатах теста.
