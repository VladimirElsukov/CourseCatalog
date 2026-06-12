# Mermaid-схема для статьи 6: Чёткая формулировка задачи (распределение по 2-3 рядам)

## Схема 1: Техника 5W1H (3 ряда: Промпт сверху, 3 вопроса в ряд, 3 вопроса в ряд, Результат снизу)

```mermaid
graph TD
    P["ПРОМПТ"] --> W1["WHO: Для кого?"]
    P --> W2["WHAT: Что делать?"]
    P --> W3["WHEN: Когда?"]
    W1 --> W4["WHERE: Где?"]
    W2 --> W5["WHY: Зачем?"]
    W3 --> W6["HOW: Как?"]
    W4 --> R["ЧЁТКАЯ ЗАДАЧА"]
    W5 --> R
    W6 --> R

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef question fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class W1,W2,W3,W4,W5,W6 question
    class R result
```

**Рис. 1.** Техника 5W1H: 6 вопросов в 2 ряда (3+3), Результат снизу.

---

## Схема 2: Правила конкретности (3 ряда: Расплывчатая сверху, 2 правила в ряд, 2 правила в ряд, Чёткая снизу)

```mermaid
graph TD
    P["РАСПЛЫВЧАТАЯ ЗАДАЧА"] --> R1["1. Конкретное действие"]
    P --> R2["2. Измеримые параметры"]
    R1 --> R3["3. Одно действие"]
    R2 --> R4["4. Отсутствие двусмысленности"]
    R3 --> C["ЧЁТКАЯ ЗАДАЧА"]
    R4 --> C

    classDef bad fill:#FFCDD2,stroke:#C62828,stroke-width:4px
    classDef rule fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef good fill:#C8E6C9,stroke:#2E7D32,stroke-width:4px

    class P bad
    class R1,R2,R3,R4 rule
    class C good
```

**Рис. 2.** 4 правила конкретности: 2 ряда (2+2), Результат снизу.

---

## Схема 3: Пример применения 5W1H (3 ряда: Расплывчатая сверху, 3 вопроса в ряд, 3 вопроса в ряд, Чёткая снизу)

```mermaid
graph TD
    R["РАСПЛЫВЧАТАЯ: 'Напиши пост про кофе'"] --> Q1["WHO: IT-специалисты 25-35 лет"]
    R --> Q2["WHAT: продающий пост"]
    R --> Q3["WHEN: не критично"]
    Q1 --> Q4["WHERE: Instagram"]
    Q2 --> Q5["WHY: привлечь внимание"]
    Q3 --> Q6["HOW: 100-120 слов, Hook→Benefit→CTA"]
    Q4 --> C["ЧЁТКАЯ: 'Напиши пост для Instagram (100-120 слов)...'"]
    Q5 --> C
    Q6 --> C

    classDef bad fill:#FFCDD2,stroke:#C62828,stroke-width:4px
    classDef question fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef good fill:#C8E6C9,stroke:#2E7D32,stroke-width:4px

    class R bad
    class Q1,Q2,Q3,Q4,Q5,Q6 question
    class C good
```

**Рис. 3.** Пример: 2 ряда (3+3), Результат снизу.