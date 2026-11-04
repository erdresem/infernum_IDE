# Быстрая сборка Infernum IDE через GitHub (без Node.js на ПК)

**На компьютере ничего для сборки устанавливать не нужно.** GitHub сам скачает Node.js, pnpm, Python, Rust и системные компиляторы на своих временных серверах.

1. Скачай и распакуй `infernum-ide-github-build-kit-v0.1.2.zip`.
2. На [github.com/new](https://github.com/new) создай репозиторий `Infernum-IDE`.
3. В репозитории выбери **Add file → Upload files**.
4. Перетащи все файлы из папки `Infernum-IDE`, обязательно включая `.github`.
5. Нажми **Commit changes** в ветку `main`.
6. Открой вкладку **Actions** → **Build Infernum IDE Portable**.
7. Дождись двух зелёных задач и скачай артефакты внизу страницы запуска:
   - `Infernum-IDE-Windows-x64-Portable` — ZIP для Windows.
   - `Infernum-IDE-Linux-x64-Portable` — TAR.GZ для Linux.

Готово. На ПК нужен только браузер. Node.js запускается исключительно внутри GitHub Actions.

Для повторной сборки: **Actions → Build Infernum IDE Portable → Run workflow**.

Подробности — в `README.md`.
