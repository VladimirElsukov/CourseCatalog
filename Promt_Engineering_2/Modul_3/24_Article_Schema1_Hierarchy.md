# Схема 1: «Иерархия компонентов промпта» (вертикальная компоновка)

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

    P --> Z1["ЗАДАЧА"]
    P --> Z2["КОНТЕКСТ"]
    P --> Z3["ОГРАНИЧЕНИЯ"]
    P --> Z4["ФОРМАТ"]

    Z1 --> Z1a["Что нужно сделать"]
    Z1 --> Z1b["Цель промпта"]

    Z2 --> Z2a["Аудитория"]
    Z2 --> Z2b["Данные и факты"]

    Z3 --> Z3a["Объём текста"]
    Z3 --> Z3b["Стиль и тон"]
    Z3 --> Z3c["Ключевые слова"]

    Z4 --> Z4a["Структура ответа"]
    Z4 --> Z4b["Формат (список, таблица)"]

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px,color:#fff
    classDef level1 fill:#81C784,stroke:#2E7D32,stroke-width:4px,color:#fff
    classDef level2 fill:#FFF59D,stroke:#F9A825,stroke-width:4px,color:#e65100

    class P prompt
    class Z1,Z2,Z3,Z4 level1
    class Z1a,Z1b,Z2a,Z2b,Z3a,Z3b,Z3c,Z4a,Z4b level2
```

**Рисунок 1.** «Иерархия компонентов промпта» (hierarchy tree). 1 колонка: ПРОМПТ. 2 колонка: ЗАДАЧА, КОНТЕКСТ, ОГРАНИЧЕНИЯ, ФОРМАТ (в столбик). У каждой свои строки (подкомпоненты). Компактная 1:1, текст полный, цвета и рамки 4px.