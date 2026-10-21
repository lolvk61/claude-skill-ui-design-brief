# ui-design-brief

[Русский](#русский) · [English](#english)

---

## Русский

Скилл для [Claude Code](https://claude.com/claude-code), который не даёт сразу
верстать шаблонный «нейро-дизайн». Перед тем как делать новый интерфейс, Claude
коротко расспрашивает о дизайне, показывает 2–3 эскиза на выбор и только потом
делает.

### Что делает

- **Новый интерфейс** (сайт, приложение, дашборд, игровое меню, окно мода):
  3–4 вопроса кнопками с конкретными вариантами (палитры с hex-кодами, реальные
  референсы, плотность, содержание), затем 2–3 заметно разных эскиза. Выбранное
  направление записывается в `DESIGN.md` или CSS-переменные, а перед сдачей
  результат проверяется по скриншоту.
- **«На твой вкус», «без вопросов»:** стиль выбирается по жанру продукта,
  называется одной строкой, в конце предлагается его сменить.
- **«По-быстрому», «ничего лишнего»:** без брифа, в аккуратном стандартном виде
  фреймворка.
- **Мелкие правки готового интерфейса:** скилл не вмешивается.

Анти-список: градиенты, неон и свечение; сетки одинаковых карточек и шаблонный
лендинг; пустота, заглушки и пустые слоганы. Цвет со смыслом (статусы, серии
на графиках, категории) при этом разрешён.

### Установка

Склонируй репозиторий в папку скиллов Claude Code:

```bash
git clone https://github.com/lolvk61/claude-skill-ui-design-brief.git ~/.claude/skills/ui-design-brief
```

На Windows это `%USERPROFILE%\.claude\skills\ui-design-brief`. Скилл подхватится
в новой сессии и сработает сам, когда понадобится новый интерфейс.

### Тесты

В `evals/evals.json` лежат пять тестовых запросов (сайт кофейни, десктопное
приложение, мелкая правка, дашборд «без вопросов», быстрый таймер), а в
`evals/files/` входной файл для теста с правкой.

### Лицензия

[MIT](LICENSE)

---

## English

A [Claude Code](https://claude.com/claude-code) skill that stops Claude from
jumping straight into generic, AI-looking UI. Before building a new interface,
Claude runs a short design brief, shows 2–3 sketches to choose from, and only
then builds.

The skill text is written in Russian; Claude follows it regardless of the
language you talk to it in.

### What it does

- **New UI** (website, app, dashboard, game menu, mod settings window):
  3–4 quick multiple-choice questions with concrete options (hex palettes, real
  references, density, content source), then 2–3 genuinely different sketches.
  The chosen direction is recorded in `DESIGN.md` or CSS variables, and the
  result is checked on screenshots before hand-off.
- **"Your call" / "no questions":** picks a style that fits the product's
  genre, names it in one line, and offers to change it at the end.
- **"Quick and simple" / "nothing extra":** skips the brief and uses the tidy
  stock look of the framework.
- **Small fixes to an existing UI:** the skill stays out of the way.

Anti-patterns it avoids: gradients, neon and glow; grids of identical cards and
template landing pages; empty filler, placeholders and hollow slogans. Colour
that carries meaning (statuses, chart series, categories) is explicitly allowed.

### Install

Clone into your Claude Code skills folder:

```bash
git clone https://github.com/lolvk61/claude-skill-ui-design-brief.git ~/.claude/skills/ui-design-brief
```

On Windows that is `%USERPROFILE%\.claude\skills\ui-design-brief`. The skill is
picked up in a new session and triggers on its own whenever a new UI is needed.

### Evals

`evals/evals.json` holds five test prompts (coffee-shop site, desktop app,
small fix, "no questions" dashboard, quick timer); `evals/files/` has the input
file for the small-fix case.

### License

[MIT](LICENSE)
