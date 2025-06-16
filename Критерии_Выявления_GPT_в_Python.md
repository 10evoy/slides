# Критерии выявления Python-кода, сгенерированного нейросетями (GPT)

В этом документе представлены основные критерии, по которым можно определить, что Python-код был написан искусственным интеллектом, а не человеком. Каждый критерий сопровождается примерами.

## 1. Избыточное комментирование

Нейросети часто создают чрезмерно подробные комментарии, объясняющие даже очевидные операции.

**Пример кода, сгенерированного нейросетью:**

```python
# Функция для сложения двух чисел
def add(a, b):
    # Складываем два числа и сохраняем результат
    result = a + b
    # Возвращаем результат сложения
    return result
```

**Как бы это написал человек:**

```python
def add(a, b):
    return a + b
```

## 2. Шаблонные структуры и решения

Нейросети часто используют стандартные шаблоны решения задач, избегая нестандартных подходов.

**Пример кода, сгенерированного нейросетью:**

```python
def is_palindrome(text):
    """
    Проверяет, является ли строка палиндромом.
    
    Args:
        text (str): Строка для проверки.
        
    Returns:
        bool: True, если строка является палиндромом, иначе False.
    """
    # Приводим к нижнему регистру и удаляем пробелы
    cleaned_text = text.lower().replace(" ", "")
    
    # Сравниваем строку с ее обратной версией
    return cleaned_text == cleaned_text[::-1]
```

**Как бы это написал человек:**

```python
def is_palindrome(s):
    s = s.lower().replace(" ", "")
    return s == s[::-1]
```

## 3. Отсутствие оптимизации и "умных" решений

Нейросети редко используют продвинутые оптимизации или нестандартные приемы.

**Пример кода, сгенерированного нейросетью:**

```python
def find_max(numbers):
    """Находит максимальное число в списке."""
    if not numbers:
        return None
    
    max_number = numbers[0]
    
    for number in numbers:
        if number > max_number:
            max_number = number
    
    return max_number
```

**Как бы это написал человек:**

```python
def find_max(numbers):
    if not numbers:
        return None
    return max(numbers)
```

## 4. Избыточная обработка ошибок

Нейросети часто добавляют избыточную обработку ошибок и проверки граничных условий.

**Пример кода, сгенерированного нейросетью:**

```python
def get_element(lst, index):
    """
    Получает элемент списка по индексу.
    
    Args:
        lst (list): Список элементов.
        index (int): Индекс элемента.
        
    Returns:
        any: Элемент списка.
        
    Raises:
        TypeError: Если lst не является списком или index не является целым числом.
        IndexError: Если index выходит за границы списка.
    """
    # Проверяем, является ли lst списком
    if not isinstance(lst, list):
        raise TypeError("Первый аргумент должен быть списком")
    
    # Проверяем, является ли index целым числом
    if not isinstance(index, int):
        raise TypeError("Второй аргумент должен быть целым числом")
    
    # Проверяем, находится ли index в допустимом диапазоне
    if index < 0 or index >= len(lst):
        raise IndexError("Индекс выходит за границы списка")
    
    # Возвращаем элемент списка
    return lst[index]
```

**Как бы это написал человек:**

```python
def get_element(lst, index):
    try:
        return lst[index]
    except IndexError:
        return None  # или raise
```

## 5. Стандартизированное форматирование

Нейросети строго придерживаются стандартов форматирования кода (PEP 8 для Python).

**Пример кода, сгенерированного нейросетью:**

```python
def process_data(data_list, threshold=0.5, include_metadata=False):
    """
    Обрабатывает данные из списка.
    
    Args:
        data_list (list): Список данных для обработки.
        threshold (float, optional): Пороговое значение. По умолчанию 0.5.
        include_metadata (bool, optional): Включать ли метаданные. По умолчанию False.
        
    Returns:
        list: Обработанные данные.
    """
    result = []
    
    for item in data_list:
        if item['value'] > threshold:
            processed_item = {
                'id': item['id'],
                'processed_value': item['value'] * 2
            }
            
            if include_metadata:
                processed_item['metadata'] = item.get('metadata', {})
                
            result.append(processed_item)
    
    return result
```

**Как мог бы выглядеть код, написанный человеком:**

```python
def process_data(data, thresh=0.5, with_meta=False):
    result = []
    
    for item in data:
        if item['value'] <= thresh:
            continue
            
        proc = {'id': item['id'], 'processed_value': item['value'] * 2}
        
        if with_meta:
            proc['metadata'] = item.get('metadata', {})
            
        result.append(proc)
    
    return result
```

## 6. Предсказуемые имена переменных

Нейросети используют очень предсказуемые, "учебные" имена переменных и функций.

**Пример кода, сгенерированного нейросетью:**

```python
def calculate_average_score(student_scores):
    """Вычисляет средний балл студента."""
    total_score = 0
    number_of_subjects = len(student_scores)
    
    for subject_score in student_scores:
        total_score += subject_score
    
    average_score = total_score / number_of_subjects
    return average_score
```

**Как бы это написал человек:**

```python
def avg_score(scores):
    return sum(scores) / len(scores) if scores else 0
```

## 7. Отсутствие "хаков" и нестандартных подходов

Нейросети редко используют нестандартные приемы или "хаки".

**Пример кода, сгенерированного нейросетью:**

```python
def remove_duplicates(items):
    """Удаляет дубликаты из списка, сохраняя порядок элементов."""
    unique_items = []
    
    for item in items:
        if item not in unique_items:
            unique_items.append(item)
    
    return unique_items
```

**Как бы это написал человек:**

```python
def remove_duplicates(items):
    return list(dict.fromkeys(items))  # Хак с использованием OrderedDict