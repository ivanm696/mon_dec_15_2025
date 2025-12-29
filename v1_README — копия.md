# grok-android

Простой каркас Android-проекта и конфигурация CI / GitHub Pages для репозитория grok-android-1.0.88-release.00.

Содержимое репозитория
- Android-модуль `app/` (Kotlin, минимальный Hello World)
- Файлы сборки Gradle (Kotlin DSL)
- CI workflow для сборки, тестов и lint
- GitHub Pages: простая страница из `docs/`

Как собирать локально
1. Установите JDK 17 и Android SDK.
2. Запустите сборку Gradle в корне репозитория:

```bash
./gradlew assembleDebug
```

CI
- Файл: `.github/workflows/android-ci.yml` — собирает проект, запускает тесты и lint.

Публикация сайта
- Файл: `.github/workflows/pages.yml` — деплойит содержимое `docs/` на GitHub Pages.

Лицензия
Проект поставляется под лицензией MIT (см. LICENSE).

Контакты
- Владелец: @ivan327