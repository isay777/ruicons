<div align="center">

<br>

# 🇷🇺 RU Icons

### Иконочный шрифт российских сервисов

[![Версия](https://img.shields.io/badge/версия-1.2-5b6ef5?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0xIDE1aC0ydi02aDJ2NnptMC04aC0yVjdoMnYyeiIvPjwvc3ZnPg==)](CHANGELOG.md)
[![Иконок](https://img.shields.io/badge/иконок-21-a855f7?style=flat-square)](https://ruicons-font.ru/#icons)
[![Лицензия](https://img.shields.io/badge/лицензия-MIT-22c55e?style=flat-square)](LICENSE)
[![Сайт](https://img.shields.io/badge/сайт-ruicons--font.ru-5b6ef5?style=flat-square)](https://ruicons-font.ru/)

<br>

**VK · Яндекс · Авито · Ozon · Wildberries · Rutube · Одноклассники · Max**  
и другие российские платформы — в виде шрифта.  
Подключается одной строкой CSS, работает как Font Awesome.

<br>

[**🌐 Сайт и демо**](https://ruicons-font.ru/) &nbsp;·&nbsp; [**⬇ Скачать v1.2**](https://ruicons-font.ru/download/ruicons-1.2.zip) &nbsp;·&nbsp; [**📋 Список иконок**](#список-иконок)

<br>

</div>

---

## Что это такое

**RU Icons** — бесплатный иконочный шрифт с иконками российских сервисов. Работает так же, как Font Awesome: подключаете один CSS-файл, вставляете `<span>` с нужным Unicode — иконка появляется. Поддерживаются **цветные иконки** через нативный CSS `font-palette` — без SVG, без JS, без зависимостей.

### Почему шрифт, а не SVG?

| | RU Icons (шрифт) | SVG-иконки |
|---|:---:|:---:|
| Подключение | 1 строка CSS | импорт каждого файла |
| Масштабирование | `font-size` | `width` / `height` |
| Цвет | `color` / `font-palette` | `fill` / `stroke` |
| Вес (21 иконка) | ~18 KB woff2 | ~50–150 KB |
| React/Vue | `className="ri"` | импорт компонента |

---

## Быстрый старт

### 1. Скачайте архив

→ [**ruicons-1.2.zip**](https://ruicons-font.ru/download/ruicons-1.2.zip)

В архиве: `ruicons.css` · `ruicons.woff2` · `ruicons.woff` · `ruicons.ttf` · `ruicons.otf`

### 2. Добавьте файлы в проект

```
ваш-проект/
├── fonts/
│   └── ruicons/
│       ├── ruicons.css      ← подключаете этот файл
│       ├── ruicons.woff2
│       ├── ruicons.woff
│       ├── ruicons.ttf
│       └── ruicons.otf
└── index.html
```

### 3. Подключите CSS

```html
<head>
  <link rel="stylesheet" href="fonts/ruicons/ruicons.css">
</head>
```

Или через `@import`:

```css
@import "fonts/ruicons/ruicons.css";
```

### 4. Используйте иконки

```html
<!-- Монохромная иконка VK -->
<span class="ri">&#xf00a;</span>

<!-- Цветная иконка Авито -->
<span class="ri palette0">&#xf002;</span>

<!-- Управление размером -->
<span class="ri" style="font-size: 32px">&#xf00f;</span>
```

---

## Список иконок

| Unicode | Класс | Сервис | Цветной |
|---------|-------|--------|:-------:|
| `\f000` | `icon-alisa` | Алиса (Яндекс) | |
| `\f001` | `icon-avito` | Авито | |
| `\f002` | `icon-avito-cvet` | Авито | 🎨 |
| `\f003` | `icon-dzen` | Дзен | |
| `\f004` | `icon-max` | Max | |
| `\f005` | `icon-odnoklas` | Одноклассники | |
| `\f006` | `icon-ozon` | Ozon | |
| `\f007` | `icon-ozon-cvet` | Ozon | 🎨 |
| `\f008` | `icon-rutube` | Rutube | |
| `\f009` | `icon-rutube-cvet` | Rutube | 🎨 |
| `\f00a` | `icon-vk` | ВКонтакте | |
| `\f00b` | `icon-vkvideo` | VK Видео | |
| `\f00c` | `icon-vkvideo-cvet` | VK Видео | 🎨 |
| `\f00d` | `icon-wb` | Wildberries | |
| `\f00e` | `icon-wb-cvet` | Wildberries | 🎨 |
| `\f00f` | `icon-ya` | Яндекс | |
| `\f010` | `icon-yab` | Яндекс Браузер | |
| `\f011` | `icon-eda-cvet` | Яндекс Еда ✨ | 🎨 |
| `\f012` | `icon-yavideo-cvet` | Яндекс Видео ✨ | 🎨 |
| `\f013` | `icon-yadisk` | Яндекс Диск ✨ | |
| `\f014` | `icon-yamarket-cvet` | Яндекс Маркет ✨ | 🎨 |

✨ — новые в v1.2 · 🎨 — есть цветной вариант

---

## Документация

### Монохромные иконки

Цвет задаётся через CSS-свойство `color` — иконки наследуют цвет родительского элемента:

```html
<span class="ri" style="color: #0788d1; font-size: 24px">&#xf00a;</span>
```

```css
.vk-icon {
  color: #0788d1;   /* фирменный цвет VK */
  font-size: 24px;
}
```

### Цветные иконки (font-palette)

Иконки с суффиксом `-cvet` содержат встроенную цветовую палитру бренда. Добавьте класс `palette0`:

```html
<!-- Цветная иконка Авито -->
<span class="ri palette0">&#xf002;</span>

<!-- Цветная иконка Ozon -->
<span class="ri palette0">&#xf007;</span>
```

### Своя цветовая палитра

Можно переопределить цвета через `@font-palette-values`:

```css
@font-palette-values --custom {
  font-family: "ruicons";
  base-palette: 0;
  override-colors: 0 #ff6600, 1 #ffffff;
}

.my-icon {
  font-family: "ruicons";
  font-palette: --custom;
}
```

### Размеры

Иконки масштабируются как обычный текст — через `font-size`:

```html
<span class="ri" style="font-size: 16px">&#xf00a;</span>
<span class="ri" style="font-size: 32px">&#xf00a;</span>
<span class="ri" style="font-size: 64px">&#xf00a;</span>
<span class="ri" style="font-size: 128px">&#xf00a;</span>
```

### Рядом с текстом

```html
<button>
  <span class="ri" style="vertical-align: middle; margin-right: 6px">&#xf00a;</span>
  Войти через VK
</button>

<a href="#">
  <span class="ri palette0">&#xf002;</span>
  Перейти на Авито
</a>
```

### React

```jsx
import "./fonts/ruicons/ruicons.css";

// Монохромная
function IconVK({ size = 24, color = "inherit" }) {
  return (
    <span
      className="ri"
      style={{ fontSize: size, color }}
      dangerouslySetInnerHTML={{ __html: "&#xf00a;" }}
    />
  );
}

// Цветная
function IconAvito({ size = 24 }) {
  return (
    <span
      className="ri palette0"
      style={{ fontSize: size }}
      dangerouslySetInnerHTML={{ __html: "&#xf002;" }}
    />
  );
}
```

### Vue

```vue
<template>
  <button>
    <span class="ri palette0" style="font-size: 20px">&#xf00a;</span>
    Войти через VK
  </button>
</template>

<style>
@import "@/fonts/ruicons/ruicons.css";
</style>
```

---

## Браузерная поддержка

| Браузер | `font-palette` (цвет) | Монохром |
|---------|:---------------------:|:--------:|
| Chrome / Edge 101+ | ✅ | ✅ |
| Firefox 107+ | ✅ | ✅ |
| Safari 15.4+ | ✅ | ✅ |
| Яндекс Браузер | ✅ | ✅ |
| IE 11 | ❌ | ✅ |

> Монохромные иконки работают во всех современных браузерах. Цветные иконки (`palette0`) требуют поддержки `font-palette` — все актуальные браузеры поддерживают.

---

## Структура репозитория

```
ruicons/
├── index.html        # Сайт-витрина (демо всех иконок, документация, установка)
├── robots.txt        # Директивы для поисковых роботов
├── sitemap.xml       # Карта сайта для Google и Яндекс
├── site.webmanifest  # PWA-манифест
├── .htaccess         # Apache: HTTPS, кэш, CORS, GZIP
├── .gitignore
├── LICENSE           # MIT
├── CHANGELOG.md      # История изменений
└── README.md
```

> **Примечание:** Файлы шрифта (`.woff2`, `.woff`, `.ttf`, `.otf`, `.css`) не хранятся в репозитории — они распространяются через ZIP-архив на сайте.  
> Скачать: [ruicons-font.ru/download/ruicons-1.2.zip](https://ruicons-font.ru/download/ruicons-1.2.zip)

---

## Разработка и вклад

Нашли ошибку? Хотите новую иконку? Открывайте [Issue](https://github.com/ваш-username/ruicons/issues) — рассмотрим в следующем релизе.

При создании Issue укажите:
- Название сервиса и ссылку на официальный логотип
- Нужен монохром, цветной или оба варианта

---

## Лицензия

**MIT** — используйте бесплатно в личных и коммерческих проектах.

> Логотипы VK, Яндекс, Авито, Ozon, Wildberries, Rutube, Одноклассников и других сервисов являются товарными знаками соответствующих компаний. RU Icons не является официальным продуктом этих компаний.

---

<div align="center">

Сделано с ❤️ для русскоязычных разработчиков · [ruicons-font.ru](https://ruicons-font.ru/)

</div>
