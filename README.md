# dominicusin/.github — инфраструктура экосистемы

Репозиторий служит двум целям:

1. **Reusable workflows** для всех систем экосистемы (`dominicusin/.github/.github/workflows/*@main`).
2. **Profile README и архив** материалов (в т.ч. математические результаты AlphaEvolve ниже).

Организационные шаблоны issue/PR живут в репозиториях `surypus/.github` и `neoallunity/.github` — GitHub применяет их только на уровне организации.

## Доступные workflows

| Workflow | Назначение |
|---|---|
| `haskell-ci.yml` | GHC 9.6.5 + cabal build/test |
| `python-ci.yml` | ruff + mypy + pytest |
| `js-site-ci.yml` | Node 24, npm ci + build |
| `docs-ci.yml` | mkdocs strict build |
| `mirror-gitlab.yml` | opt-in зеркало в GitLab |

Подключение:

```yaml
jobs:
  ci:
    uses: dominicusin/.github/.github/workflows/python-ci.yml@main
    with:
      python-version: '3.11'
      test-path: tests
```

Информация о системах, статусах и метриках: [`dominicusin/portfolio`](https://github.com/dominicusin/portfolio).

---

# Mathematical Results - AlphaEvolve

Этот репозиторий содержит математические результаты проекта AlphaEvolve от Google DeepMind.

## Описание

Репозиторий включает Jupyter-ноутбук с математическими результатами и исследованиями, полученными с помощью системы AlphaEvolve.

## Файлы

- `mathematical_results.ipynb` - Jupyter-ноутбук с математическими результатами
- `LICENSE` - Лицензия MIT
- `profile/` - Директория с профилем

## Использование

Ноутбук можно открыть в Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dominicusin/.github/blob/main/mathematical_results.ipynb)

## Лицензия

- Программное обеспечение распространяется под лицензией Apache License, Version 2.0
- Остальные материалы распространяются под лицензией Creative Commons Attribution 4.0 International (CC-BY)

Подробнее см. [LICENSE](LICENSE)

## Авторство

Copyright 2024-2025 Google DeepMind Technologies Limited

Это не официальный продукт Google.
