# Financial Model Agent Skill

> Открытый проект [EQ Platform](https://eq.team) — [страница проекта](https://eq.team/open-source/oss-financial-model-skill/)

AI-скилл для создания финансовых моделей бизнеса. Используется в OpenClaw агенте для построения FIM (Financial Independence Model).

## Возможности

- Построение финмоделей для стартапов и малого бизнеса
- Прогнозирование доходов/расходов/прибыли на 1–3 года
- Расчёт unit-экономики (LTV, CAC, маржинальность)
- Оценка точки безубыточности и runway
- Сценарный анализ (база / оптимизм / пессимизм)
- Sensitivity analysis

## Поддерживаемые бизнес-модели

- SaaS / Подписка
- Маркетплейс
- E-commerce
- Услуги / Агентство
- Freemium / Рекламная

## Российская специфика

- Налоговые режимы: УСН, ОСН, НПД, IT-льготы
- Страховые взносы (актуальные коэффициенты 2025–2026)
- Зарплатные бенчмарки IT-рынка
- Эквайринг и платёжные системы

## Установка в OpenClaw

```bash
# Скопировать в workspace скиллов агента
mkdir -p ~/.openclaw/workspaces/finance/skills/financial-model
cp SKILL.md ~/.openclaw/workspaces/finance/skills/financial-model/
```

## Формат вывода

Скилл генерирует два формата одновременно:
- **Markdown** — читаемая версия с таблицами P&L, Cash Flow, Unit-экономика
- **JSON** — машиночитаемая версия для импорта в equity.su
