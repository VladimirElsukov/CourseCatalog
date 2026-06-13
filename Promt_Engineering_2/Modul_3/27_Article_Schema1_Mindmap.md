# Схема 1: «Структура многоцелевого промпта» (вертикальная компоновка)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "14px",
    "fontFamily": "sans-serif"
  }
}}%%
graph LR
    P["ПРОМПТ"]

    P --> T1["ЗАДАЧА 1"]
    P --> T2["ЗАДАЧА 2"]
    P --> T3["ЗАДАЧА 3"]

    T1 --> T1a["Целевая аудитория"]
    T1 --> T1b["Критерии: возраст, пол, интересы"]

    T2 --> T2a["3 канала продвижения"]
    T2 --> T2b["Обоснование выбора"]

    T3 --> T3a["График на месяц"]
    T3 --> T3b["Даты и форматы"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef task fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef subtask fill:#FFF59D,stroke:#F9A825,stroke-width:4px,color:#e65100

    class P prompt
    class T1,T2,T3 task
    class T1a,T1b,T2a,T2b,T3a,T3b subtask
```

**Рисунок 1.** «Структура многоцелевого промпта» (mind map). 3 ряда: Промпт слева, 3 задачи в столбик (ЗАДАЧА 1, ЗАДАЧА 2, ЗАДАЧА 3), расширения-ветвления справа от каждой задачи. Компактная 1:1, текст полный, цвета и рамки 4px. Расширение в вертикали, поворот на 90 градусов.