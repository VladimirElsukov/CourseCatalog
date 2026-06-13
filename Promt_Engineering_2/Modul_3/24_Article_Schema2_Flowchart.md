# Схема 2: «Алгоритм расстановки приоритетов» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "13px",
    "fontFamily": "sans-serif"
  }
}}%%
graph LR
    P["ПРОМПТ"]

    P --> Q1{"Тип задачи?"}
    P --> Q2{"Конфликт\nприоритетов?"}
    P --> Q3{"Нужно\nвыбрать\nприоритет?"}

    Q1 -->|Официальный документ| A1["Приоритет 1: Тон (официальный)"]
    Q1 -->|Маркетинговый текст| A2["Приоритет 1: Тон (дружелюбный)"]
    Q1 -->|Технический текст| A3["Приоритет 1: Точность (факты, данные)"]
    Q1 -->|Креативный текст| A4["Приоритет 1: Тон (поэтический)"]

    Q2 -->|Да| A5["Выбери\nболее\nвысокий\nприоритет"]
    Q2 -->|Нет| A6["Соблюдай\nвсе\nприоритеты"]

    Q3 -->|Да| A7["Приоритет 1\nкритически\nважен"]
    Q3 -->|Нет| A8["Приоритет 5\nопционален"]

    A1 --> R["РЕЗУЛЬТАТ"]
    A2 --> R
    A3 --> R
    A4 --> R
    A5 --> R
    A6 --> R
    A7 --> R
    A8 --> R

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef question fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef action fill:#FFF59D,stroke:#F9A825,stroke-width:4px,color:#e65100
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P prompt
    class Q1,Q2,Q3 question
    class A1,A2,A3,A4,A5,A6,A7,A8 action
    class R result
```

**Рисунок 2.** «Алгоритм расстановки приоритетов» (flowchart). 1 колонка: ПРОМПТ. 2 колонка: вопросы и действия (в столбик). У каждой свои строки. Компактная 1:1, текст полный, цвета и рамки 4px.