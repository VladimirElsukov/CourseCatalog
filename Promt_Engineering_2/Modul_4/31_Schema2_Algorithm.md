# Схема 2: «Алгоритм выбора лучшего варианта» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "13px",
    "fontFamily": "sans-serif"
  }
}}%%
graph TD
    P["ПРОМПТ"]

    P --> G["ГЕНЕРАЦИЯ ВЕТВЕЙ"]
    G --> E["ОЦЕНКА"]
    E --> S["ВЫБОР"]

    S --> R["РЕЗУЛЬТАТ"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef step fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px,color:#fff

    class P prompt
    class G,E,S step
    class R result
```

**Рисунок 2.** «Алгоритм выбора лучшего варианта» (flowchart). **3 ряда**: Промпт сверху, 3 этапа в столбик (ГЕНЕРАЦИЯ ВЕТВЕЙ, ОЦЕНКА, ВЫБОР), Результат снизу. Компактная 1:1, текст полный, цвета и рамки 4px. Вертикальная компоновка.