# Текущий годовой план (до изменений 27.10)

> Копия текста плана из README [репозитория курса](https://github.com/TIlzziter/p58-course-2026) на 28.10.2026. Код, лабы и материалы — только там. Источник правды — README курса; предложения по изменениям — в [2026-10-27-plan-update.md](2026-10-27-plan-update.md).

## Проект 58 · 9 класс · 2026–2027

Годовой курс школьной ИТ-программы «Проект 58» для 9 класса (8 учеников, 14–15 лет).
За год команда с распределёнными ролями проектирует, пишет, тестирует, разворачивает и сопровождает
**сайт с мультиплеерными браузерными играми, которые открываются из Telegram-ботов как Mini Apps**.
Бэкенд на Python. ИИ-агент работает как участник команды: правила в `AGENTS.md`, spec-first,
ревью агентом и человеком, измеримая оценка его работы.

* 29 учебных недель: 26.10.2026 – 30.05.2027, зимние каникулы ~25.12–10.01.
* Т1 — недели 1–5, Т2 — недели 6–16, Т3 — недели 17–29.
* Каждая неделя: **лекция** (`l01`) и **семинар** (`l02`), по 3 академических часа. Всего 58 уроков + вводный урок 00.
* Стек: Python 3.12, FastAPI, aiogram 3, WebSocket, PostgreSQL + SQLAlchemy 2 + Alembic, Redis, Docker, Nginx,
  GitHub Actions, pytest; клиент игр — HTML/CSS/JS и `<canvas>`.
* Роли: аналитика, бэкенд и боты, фронтенд, тестирование, DevOps, дизайн, R&D (по желанию).

Источник тем и последовательности — план занятий «Проект 58: план занятий на 2026–2027».
Сводка — в [`tools/syllabus.py`](https://github.com/TIlzziter/p58-course-2026/blob/main/tools/syllabus.py); из него генерируются таблица ниже и README уроков.

## Расписание

<!-- schedule -->
| Нед. | Даты | Урок | Тема | Лабораторная | Контест |
|---|---|---|---|---|---|
| 1 | 26.10–01.11 | [01 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w01-l01-kickoff/README.md) | Кикофф: игры из Telegram, роли, Git-процесс |  |  |
| 1 | 26.10–01.11 | [02 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w01-l02-team-setup/README.md) | Семинар: идея, подкоманды, монорепо, доска задач, AGENTS.md | [lab01](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w01-l02-team-setup/labs/lab01-git-flow/README.md) |  |
| 2 | 02.11–08.11 | [03 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w02-l01-spec-first/README.md) | Spec-first: user story, критерии приёмки, протокол; архитектура бот → Mini App → FastAPI |  |  |
| 2 | 02.11–08.11 | [04 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w02-l02-bot-and-api/README.md) | Семинар: спека игры 1, бот на aiogram 3 с кнопкой WebApp, каркас FastAPI | [lab02](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w02-l02-bot-and-api/labs/lab02-api-by-spec/README.md) | [c01](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c01-python-git-specs/sheet.pdf) |
| 3 | 09.11–15.11 | [05 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w03-l01-mini-apps/README.md) | Telegram Mini Apps: initData и HMAC; HTML/CSS/JS и canvas | [lab03](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w03-l01-mini-apps/labs/lab03-init-data/README.md) |  |
| 3 | 09.11–15.11 | [06 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w03-l02-game-logic/README.md) | Семинар: логика «4 в ряд» на сервере, pytest, отрисовка на canvas | [lab04](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w03-l02-game-logic/labs/lab04-connect-four/README.md) |  |
| 4 | 16.11–22.11 | [07 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w04-l01-docker-nginx/README.md) | Docker и docker compose; Nginx как reverse proxy, домен, HTTPS |  |  |
| 4 | 16.11–22.11 | [08 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w04-l02-deploy-mvp/README.md) | Семинар: деплой MVP на VPS, чек-лист DevOps, репетиция демо | [lab05](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w04-l02-deploy-mvp/labs/lab05-docker-review/README.md) | [c02](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c02-grids-games-signatures/sheet.pdf) |
| 5 | 23.11–29.11 | [09 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w05-l01-review-t1/README.md) | Повторение к срезу Т1, ретро триместра |  |  |
| 5 | 23.11–29.11 | [10 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w05-l02-demo-t1/README.md) | Демо Т1 для родителей и администрации; срез Т1 |  |  |
| 6 | 30.11–06.12 | [11 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w06-l01-websocket-asyncio/README.md) | WebSocket в FastAPI, asyncio; комнаты и протокол сообщений |  |  |
| 6 | 30.11–06.12 | [12 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w06-l02-multiplayer-rooms/README.md) | Семинар: мультиплеер игры 1, комната на 2 игрока, сервер — источник истины | [lab06](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w06-l02-multiplayer-rooms/labs/lab06-ws-rooms/README.md) | [c03](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c03-asyncio-protocols/sheet.pdf) |
| 7 | 07.12–13.12 | [13 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w07-l01-postgres-sqlalchemy/README.md) | PostgreSQL вместо SQLite: SQLAlchemy 2 (async), миграции Alembic |  |  |
| 7 | 07.12–13.12 | [14 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w07-l02-db-rating/README.md) | Семинар: таблицы игроков, матчей и рейтинга; история партий | [lab07](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w07-l02-db-rating/labs/lab07-sqlalchemy-rating/README.md) |  |
| 8 | 14.12–20.12 | [15 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w08-l01-redis/README.md) | Redis: сессии, комнаты, TTL, pub/sub; несколько копий приложения |  |  |
| 8 | 14.12–20.12 | [16 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w08-l02-lobby-matchmaking/README.md) | Семинар: лобби, очередь матчмейкинга, приглашение другу ссылкой из бота | [lab08](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w08-l02-lobby-matchmaking/labs/lab08-redis-matchmaking/README.md) | [c04](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c04-databases-cache/sheet.pdf) |
| 9 | 21.12–24.12 | [17 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w09-l01-ci-github-actions/README.md) | CI в GitHub Actions: ruff, pytest, сборка образа | [lab09](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w09-l01-ci-github-actions/labs/lab09-ci-pipeline/README.md) |  |
| 9 | 21.12–24.12 | [18 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w09-l02-pr-review-retro/README.md) | Семинар: CI на каждый PR, кейсы PROD, ревью агент + человек, ретро полугодия |  |  |
| — | 25.12–10.01 | — | **Зимние каникулы** (ориентировочно); по желанию — QuestHub | — | — |
| 10 | 11.01–17.01 | [19 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w10-l01-cd-deploy/README.md) | CD: автодеплой на VPS после merge, секреты, staging и prod | [lab10](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w10-l01-cd-deploy/labs/lab10-secret-scanner/README.md) |  |
| 10 | 11.01–17.01 | [20 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w10-l02-deploy-pipeline/README.md) | Семинар: пайплайн деплоя, правила про секреты в AGENTS.md |  | [c05](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c05-pipelines-secrets/sheet.pdf) |
| 11 | 18.01–24.01 | [21 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w11-l01-game-algorithms/README.md) | Алгоритмы игры 2: игровой цикл, конечный автомат, честный рандом, коллизии | [lab11](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w11-l01-game-algorithms/labs/lab11-snake-engine/README.md) |  |
| 11 | 18.01–24.01 | [22 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w11-l02-game2-spec/README.md) | Семинар: спека и серверная логика игры 2, тесты по таблице правил |  |  |
| 12 | 25.01–31.01 | [23 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w12-l01-game-frontend/README.md) | Фронтенд игр: requestAnimationFrame, интерполяция, тема Telegram, мобильная вёрстка; Pyodide |  |  |
| 12 | 25.01–31.01 | [24 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w12-l02-game2-client/README.md) | Семинар: клиент игры 2, UI-кит, R&D-прототип на Pyodide | [lab12](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w12-l02-game2-client/labs/lab12-interpolation/README.md) | [c06](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c06-game-loop-random/sheet.pdf) |
| 13 | 01.02–07.02 | [25 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w13-l01-testing/README.md) | Тестирование: pytest-asyncio, тесты WebSocket, тестовая БД, смоук e2e | [lab13](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w13-l01-testing/labs/lab13-mutation-tests/README.md) |  |
| 13 | 01.02–07.02 | [26 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w13-l02-qa-plan/README.md) | Семинар: QA-план, баг-трекинг, тесты в CI, метрики работы агента |  |  |
| 14 | 08.02–14.02 | [27 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w14-l01-monitoring/README.md) | Мониторинг и логи: структурированные логи, healthcheck, метрики, алерты в Telegram | [lab14](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w14-l01-monitoring/labs/lab14-logs-alerts/README.md) |  |
| 14 | 08.02–14.02 | [28 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w14-l02-incident-drill/README.md) | Семинар: дашборд и алерты; учение «сайт упал» |  | [c07](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c07-tests-logs/sheet.pdf) |
| 15 | 15.02–21.02 | [29 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w15-l01-security/README.md) | Безопасность и ответственность: античит, rate limit, данные пользователей, prompt injection | [lab15](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w15-l01-security/labs/lab15-anticheat-ratelimit/README.md) |  |
| 15 | 15.02–21.02 | [30 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w15-l02-security-audit/README.md) | Семинар: аудит безопасности, feature freeze |  |  |
| 16 | 22.02–28.02 | [31 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w16-l01-review-t2/README.md) | Повторение к срезу Т2, ретро триместра |  |  |
| 16 | 22.02–28.02 | [32 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w16-l02-demo-t2/README.md) | Демо Т2 и срез Т2 |  | [c08](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c08-security/sheet.pdf) |
| 17 | 01.03–07.03 | [33 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w17-l01-llm-in-product/README.md) | LLM в продукте: API модели, промпты, ограничения, модерация | [lab16](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w17-l01-llm-in-product/labs/lab16-llm-evals/README.md) |  |
| 17 | 01.03–07.03 | [34 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w17-l02-extension-spec/README.md) | Семинар: выбор расширения и его спека, набор evals |  |  |
| 18 | 08.03–14.03 | [35 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w18-l01-hackathon-format/README.md) | Формат хакатона: шаблон проекта, роли под таймер, питч |  |  |
| 18 | 08.03–14.03 | [36 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w18-l02-project-template/README.md) | Семинар: шаблон «FastAPI + бот + Docker» за одну сессию |  | [c09](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c09-texts-prompts-templates/sheet.pdf) |
| 19 | 15.03–21.03 | [37 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w19-l01-mini-hackathon-1/README.md) | Мини-хакатон, сессия 1: идея, спека, каркас |  |  |
| 19 | 15.03–21.03 | [38 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w19-l02-mini-hackathon-2/README.md) | Мини-хакатон, сессия 2: доделка, питч, жюри |  |  |
| 20 | 22.03–28.03 | [39 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w20-l01-data-analysis/README.md) | Анализ данных: pandas, SQL-аналитика, графики | [lab17](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w20-l01-data-analysis/labs/lab17-game-analytics/README.md) |  |
| 20 | 22.03–28.03 | [40 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w20-l02-game-metrics/README.md) | Семинар: аналитика игровых событий — удержание, длина партий, баланс |  | [c10](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c10-data-metrics/sheet.pdf) |
| 21 | 29.03–04.04 | [41 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w21-l01-game-ai/README.md) | Алгоритмы ИИ-соперника: минимакс, эвристики, Монте-Карло | [lab18](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w21-l01-game-ai/labs/lab18-minimax/README.md) |  |
| 21 | 29.03–04.04 | [42 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w21-l02-ai-opponent/README.md) | Семинар: бот-соперник в одной из игр, турнир решений |  |  |
| 22 | 05.04–11.04 | [43 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w22-l01-load-scaling/README.md) | Нагрузка и масштабирование: locust, реплики за Nginx, Redis pub/sub, индексы | [lab19](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w22-l01-load-scaling/labs/lab19-load-report/README.md) |  |
| 22 | 05.04–11.04 | [44 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w22-l02-load-test/README.md) | Семинар: нагрузочный тест и оптимизация |  | [c11](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c11-game-trees/sheet.pdf) |
| 23 | 12.04–18.04 | [45 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w23-l01-hackathon-window/README.md) | Окно внешнего хакатона: подготовка и участие |  |  |
| 23 | 12.04–18.04 | [46 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w23-l02-hackathon-retro/README.md) | Семинар: ретро хакатона, буфер, опционально QuestHub |  |  |
| 24 | 19.04–25.04 | [47 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w24-l01-extension-cycle/README.md) | Расширение продукта: полный цикл spec-first |  |  |
| 24 | 19.04–25.04 | [48 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w24-l02-extension-impl/README.md) | Семинар: реализация расширения по мартовской спеке |  | [c12](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c12-load-scale/sheet.pdf) |
| 25 | 26.04–02.05 | [49 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w25-l01-ux-accessibility/README.md) | UX: юзабилити-тесты, доступность |  |  |
| 25 | 26.04–02.05 | [50 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w25-l02-usability-tests/README.md) | Семинар: тесты на одноклассниках, правки интерфейса |  |  |
| 26 | 03.05–09.05 | [51 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w26-l01-backups-runbook/README.md) | Надёжность: бэкапы PostgreSQL, восстановление, runbook | [lab20](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w26-l01-backups-runbook/labs/lab20-backups/README.md) |  |
| 26 | 03.05–09.05 | [52 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w26-l02-restore-drill/README.md) | Семинар: учение по восстановлению; feature freeze |  | [c13](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c13-reliability-time/sheet.pdf) |
| 27 | 10.05–16.05 | [53 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w27-l01-docs-portfolio/README.md) | Документация и портфолио: README, архитектура, видео-демо |  |  |
| 27 | 10.05–16.05 | [54 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w27-l02-stabilization/README.md) | Семинар: стабилизация, багфиксы, release candidate |  |  |
| 28 | 17.05–23.05 | [55 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w28-l01-pitch/README.md) | Публичное выступление и питч |  |  |
| 28 | 17.05–23.05 | [56 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w28-l02-rehearsal/README.md) | Семинар: генеральный прогон финального демо |  | [c14](https://github.com/TIlzziter/p58-course-2026/blob/main/contests/c14-season-final/sheet.pdf) |
| 29 | 24.05–30.05 | [57 · Лекция](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w29-l01-final-review/README.md) | Итоговое повторение |  |  |
| 29 | 24.05–30.05 | [58 · Семинар](https://github.com/TIlzziter/p58-course-2026/blob/main/lessons/w29-l02-final-demo/README.md) | Финальный демо-день, срез Т3, ретро года |  |  |
<!-- /schedule -->

