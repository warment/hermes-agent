<p align="center">
  <img src="assets/banner.png" alt="Hermes Agent" width="100%">
</p>

<h1 align="center">☤ Hermes Agent — Русская версия</h1>

<p align="center">
  <b>Форк Hermes Agent с полным русским переводом (~99% интерфейса)</b><br>
  [<b>Русский</b>] · [<a href="README.en.md">English</a>] · [<a href="README.zh-CN.md">中文</a>] · [<a href="README.ur-pk.md">اردو</a>]
</p>

---

## 🇷🇺 Русский перевод

Полная русификация десктопного приложения Hermes Agent — **~99% всех строк интерфейса**:

- Все 38 секций i18n (~3000 строк `ru.ts`): меню, настройки, биллинг, уведомления, горячие клавиши, загрузка, установка, онбординг
- Поля настроек (`ru-constants.ts`)
- Hardcoded-строки компонентов (41 файл): биллинг (проверка, планы, автопополнение), Computer Use, удаление приложения, MoA-пресеты, Quick Entry, пет-оверлей, эмодзи-пикер, star map и др.

### Релизы перевода

| Версия | Ссылка | Описание |
|--------|--------|----------|
| **v2.0.0-ru-locale** | [Релиз](https://github.com/warment/hermes-agent/releases/tag/v2.0.0-ru-locale) | Полная русификация (~99%), 41 файл |
| v1.0.0-ru-locale | [Релиз (архив)](https://github.com/warment/hermes-agent/releases/tag/v1.0.0-ru-locale) | Старая версия (i18n-файлы) |

### Установка перевода

```bash
# Вариант 1: архив из релиза v2.0.0-ru-locale
# 1) Скопируйте файлы из архива в apps/desktop/src (перезапись)
# 2) Соберите приложение:
cd apps/desktop
npm run build && npm run pack
# 3) Установите release/mac-arm64/Hermes.app в /Applications
```

```bash
# Вариант 2: ветка feat/desktop-ru-locale (для разработчиков)
git fetch origin feat/desktop-ru-locale
git checkout feat/desktop-ru-locale
cd apps/desktop && npm run build && npm run pack
```

После запуска: **Settings** → **Appearance** → **Русский**

### PR в апстрим

[#42705 — feat(i18n/desktop): add Russian (ru) locale](https://github.com/NousResearch/hermes-agent/pull/42705)

---

## ☤ О Hermes Agent

Hermes Agent — AI-агент с локальным шлюзом: работает с моделями OpenAI-совместимых API (Nous Portal, OpenRouter и др.), имеет десктопное приложение, TUI и CLI. Документация на английском — [README.en.md](README.en.md).

---

## 📄 Лицензия

MIT License
