# Схема 2: «Алгоритм создания цепочки» (горизонтальная компоновка)

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

    P --> S1["АНАЛИЗ ЗАДАЧИ"]
    P --> S2["РАЗБИЕНИЕ НА ЭТАПЫ"]
    P --> S3["ФОРМУЛИРОВКА ПРОМПТОВ"]
    P --> S4["ТЕСТИРОВАНИЕ"]
    P --> S5["ОПТИМИЗАЦИЯ"]

    S1 --> R["РЕЗУЛЬТАТ"]
    S2 --> R
    S3 --> R
    S4 --> R
    S5 --> R

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P prompt
    class S1,S2,S3,S4,S5 step
    class R result
```

**Рисунок 2.** «Алгоритм создания цепочки» (flowchart). 3 ряда: Промпт слева, 5 этапов в столбик (АНАЛИЗ ЗАДАЧИ, РАЗБИЕНИЕ НА ЭТАПЫ, ФОРМУЛИРОВКА ПРОМПТОВ, ТЕСТИРОВАНИЕ, ОПТИМИЗАЦИЯ), Результат справа. Компактная 1:1, текст полный, цвета и рамки 4px. Расширение слева направо, не длинная по горизонтали.