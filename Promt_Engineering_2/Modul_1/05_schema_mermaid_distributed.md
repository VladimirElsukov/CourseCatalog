# Mermaid-схема (распределение узлов по 2-3 рядам, полный текст, компактная 1:1)

## Схема: 2 ряда (Промпт сверху, 4 компонента в ряд, Результат снизу)

```mermaid
graph TD
    P["ПРОМПТ"] --> T["ЗАДАЧА: Напиши продающий текст"]
    P --> C["КОНТЕКСТ: Аудитория CTO, продукт AI"]
    P --> L["ОГРАНИЧЕНИЯ: max 250 слов, без эмодзи"]
    P --> F["ФОРМАТ: 4 блока Hook→Проблема→Решение→CTA"]
    T --> R["РЕЗУЛЬТАТ"]
    C --> R
    L --> R
    F --> R

    classDef task fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef ctx fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef lim fill:#FFB74D,stroke:#E65100,stroke-width:4px
    classDef fmt fill:#CE93D8,stroke:#6A1B9A,stroke-width:4px
    classDef res fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class T task
    class C ctx
    class L lim
    class F fmt
    class R res
```

**Характеристики:**
- **2 ряда**: Промпт сверху, 4 компонента в ряд, Результат снизу
- **Текст полный** (как в статье)
- **Компактная 1:1** — не растягивается по горизонтали
- **Цвета** по вашему коду
- **Рамки 4px**

---

## Схема: 3 ряда (Промпт сверху, 2 компонента в ряд, 2 компонента в ряд, Результат снизу)

```mermaid
graph TD
    P["ПРОМПТ"] --> T["ЗАДАЧА: Напиши продающий текст"]
    P --> C["КОНТЕКСТ: Аудитория CTO, продукт AI"]
    T --> L["ОГРАНИЧЕНИЯ: max 250 слов, без эмодзи"]
    C --> F["ФОРМАТ: 4 блока Hook→Проблема→Решение→CTA"]
    L --> R["РЕЗУЛЬТАТ"]
    F --> R

    classDef task fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef ctx fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef lim fill:#FFB74D,stroke:#E65100,stroke-width:4px
    classDef fmt fill:#CE93D8,stroke:#6A1B9A,stroke-width:4px
    classDef res fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class T task
    class C ctx
    class L lim
    class F fmt
    class R res
```

**Характеристики:**
- **3 ряда**: Промпт сверху, 2 компонента в ряд, 2 компонента в ряд, Результат снизу
- **Текст полный**
- **Компактная 1:1**
- **Цвета** и **рамки 4px**

---

## Схема: 3 ряда с огибающими связями (Промпт слева, 4 компонента в 2 ряда, Результат справа)

```mermaid
graph LR
    P["ПРОМПТ"] --> T["ЗАДАЧА: Напиши продающий текст"]
    P --> C["КОНТЕКСТ: Аудитория CTO, продукт AI"]
    P --> L["ОГРАНИЧЕНИЯ: max 250 слов, без эмодзи"]
    P --> F["ФОРМАТ: 4 блока Hook→Проблема→Решение→CTA"]
    T --> R["РЕЗУЛЬТАТ"]
    C --> R
    L --> R
    F --> R

    classDef task fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef ctx fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef lim fill:#FFB74D,stroke:#E65100,stroke-width:4px
    classDef fmt fill:#CE93D8,stroke:#6A1B9A,stroke-width:4px
    classDef res fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class T task
    class C ctx
    class L lim
    class F fmt
    class R res
```

**Характеристики:**
- **3 ряда**: Промпт слева, 4 компонента в 2 ряда (2+2), Результат справа
- **Текст полный**
- **Компактная 1:1** (горизонтальная компоновка `graph LR`)
- **Цвета** и **рамки 4px**
- **Связи огибают** и приходят к нужным блокам

---

## Рекомендация

**Лучший вариант для статьи 5:** **Схема 3 ряда с огибающими связями** (`graph LR`):

- Промпт слева
- 4 компонента в 2 ряда (2+2)
- Результат справа
- Текст полный
- Компактная 1:1
- Цвета и рамки 4px

Это соответствует вашему требованию: «распределял правильно узлы пусть в 2 3 ряда просто связи огибали и приходили к нужному блоку».