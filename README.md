# Vue 3 + Vite + Tailwind CSS + DaisyUI

Сучасний веб-додаток, створений з використанням Vue 3, Vite, Tailwind CSS та DaisyUI.

## 🚀 Технології

- **Vue 3** - Прогресивний JavaScript фреймворк для створення користувацьких інтерфейсів
- **Vite** - Швидкий інструмент збірки для сучасних веб-додатків
- **Tailwind CSS** - Утилітарний CSS фреймворк для швидкої розробки
- **DaisyUI** - Компонентна бібліотека для Tailwind CSS

## 📋 Вимоги

- Node.js (версія 18.3 або вище)
- npm або yarn

## 🛠️ Встановлення

1. Клонуйте репозиторій:
```bash
git clone https://github.com/yourusername/learn-vite-vue-tailwind.git
cd learn-vite-vue-tailwind
```

2. Встановіть залежності:
```bash
npm install
# або
yarn
```

3. Запустіть проект в режимі розробки:
```bash
npm run dev
# або
yarn dev
```

4. Відкрийте браузер за адресою [http://localhost:5174](http://localhost:5174)

## 📁 Структура проекту

```
learn-vite-vue-tailwind/
├── public/              # Статичні файли
├── src/                 # Вихідний код
│   ├── assets/          # Зображення, шрифти тощо
│   ├── components/      # Vue компоненти
│   │   └── TheHeader.vue # Компонент хедера
│   ├── App.vue          # Головний компонент
│   ├── main.js          # Точка входу
│   └── style.css        # Глобальні стилі
├── index.html           # HTML шаблон
├── package.json         # Залежності та скрипти
├── postcss.config.js    # Конфігурація PostCSS
├── tailwind.config.js   # Конфігурація Tailwind CSS
└── vite.config.js       # Конфігурація Vite
```

## 🧩 Компоненти

### TheHeader.vue

Адаптивний хедер з логотипом, навігацією та кнопками дій. Підтримує мобільне меню з кнопкою-гамбургером.

### App.vue

Головний компонент додатку з прикладом лічильника, що демонструє реактивність Vue 3.

## 🎨 Стилізація

Проект використовує комбінацію Tailwind CSS та DaisyUI для стилізації:

- **Tailwind CSS** - для базових стилів та утиліт
- **DaisyUI** - для готових компонентів (navbar, menu, btn, card тощо)

## 📦 Збірка для продакшену

Для створення оптимізованої збірки для продакшену:

```bash
npm run build
# або
yarn build
```

Збірка буде створена в директорії `dist/`.

## 📝 Ліцензія

MIT

## 👥 Автори

- Гук Максим - [@GukMaksim](https://github.com/GukMaksim)

---

Створено з ❤️ за допомогою Vue 3, Vite, Tailwind CSS та DaisyUI
