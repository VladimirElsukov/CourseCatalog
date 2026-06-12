# Mermaid-схема для статьи 9: Фреймворк STAR (принцип 2+2 компонента в ряд)

## Схема 1: STAR (вертикальная, 2+2 компонента в ряд)

```mermaid
graph TD
    P["ПРОМПТ"] --> S["S: SITUATION — контекст, предыстория"]
    P --> T["T: TASK — что нужно было сделать"]
    S --> A["A: ACTION — что было сделано, шаги"]
    T --> R["R: RESULT — что получилось, итог"]
    A --> F["ФИНАЛЬНЫЙ ОТВЕТ"]
    R --> F

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef star fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S,T,A,R star
    class F result
```

**Рис. 1.** Фреймворк STAR: вертикальная компоновка (2+2 компонента в ряд) — Промпт сверху, S и T в первом ряду, A и R во втором ряду, Финальный ответ снизу.

---

## Схема 2: STAR (горизонтальная, 2+2 компонента в ряд с огибающими связями)

```mermaid
graph LR
    P["ПРОМПТ"] --> S["S: SITUATION — контекст, предыстория"]
    P --> T["T: TASK — что нужно было сделать"]
    P --> A["A: ACTION — что было сделано, шаги"]
    P --> R["R: RESULT — что получилось, итог"]
    S --> F["ФИНАЛЬНЫЙ ОТВЕТ"]
    T --> F
    A --> F
    R --> F

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef star fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S,T,A,R star
    class F result
```

**Рис. 2.** Фреймворк STAR: горизонтальная компоновка (2+2 компонента в ряд с огибающими связями) — Промпт слева, 4 компонента в 2 ряда (2+2), Финальный ответ справа.

---

## Схема 3: STAR (вертикальная, 3 ряда: Промпт сверху, 2 компонента в ряд, 2 компонента в ряд, Финальный ответ снизу)

```mermaid
graph TD
    P["ПРОМПТ"] --> S["S: SITUATION — контекст, предыстория"]
    P --> T["T: TASK — что нужно было сделать"]
    S --> A["A: ACTION — что было сделано, шаги"]
    T --> R["R: RESULT — что получилось, итог"]
    A --> F["ФИНАЛЬНЫЙ ОТВЕТ"]
    R --> F

    classDef prompt fill:#4FC3F7,stroke:#01579B,stroke-width:4px
    classDef star fill:#81C784,stroke:#2E7D32,stroke-width:4px
    classDef result fill:#FF8A65,stroke:#BF360C,stroke-width:4px

    class P prompt
    class S,T,A,R star
    class F result
```

**Рис. 3.** Фреймворк STAR: 3 ряда (Промпт сверху, 2 компонента в ряд, 2 компонента в ряд, Финальный ответ снизу) — текст полный, компактная 1:1.

---

## Принцип (зафиксирован)

- **Вертикальная** (`graph TD`): **2+2 компонента в ряд** (Промпт сверху, 2 компонента в ряд, 2 компонента в ряд, Результат снизу)
- **Горизонтальная** (`graph LR`): **2+2 компонента в ряд с огибающими связями** (Промпт слева, 4 компонента в 2 ряда, Результат справа)

В следующих статьях — **полный комплект** (текст + визуал) сразу в статье.