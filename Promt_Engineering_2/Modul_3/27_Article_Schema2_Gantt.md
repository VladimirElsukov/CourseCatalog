# Схема 2: «Порядок выполнения задач» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМПТ"]

    P --> T1["ЗАДАЧА 1"]
    T1 --> T2["ЗАДАЧА 2"]
    T2 --> T3["ЗАДАЧА 3"]
    T3 --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef task fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P prompt
    class T1,T2,T3 task
    class R result
```

**Рисунок 2.** «Порядок выполнения задач» (Gantt chart). 3 ряда: Промпт сверху, 3 задачи в столбик (последовательно), Результат снизу. Компактная 1:1, текст полный, цвета и рамки 4px. Расширение в вертикали, а не в горизонтали.