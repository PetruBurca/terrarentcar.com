# 🎨 UI Components Structure

Организованная структура UI компонентов для лучшей навигации и поддержки.

## 📁 Структура папок

### 📝 **forms/** - Формы и валидация

- `checkbox.tsx` - Флажок
- `form.tsx` - Форма с валидацией
- `radio-group.tsx` - Группа радиокнопок

### 🔤 **inputs/** - Поля ввода

- `input.tsx` - Текстовое поле
- `textarea.tsx` - Многострочное поле
- `select.tsx` - Выпадающий список
- `slider.tsx` - Слайдер
- `switch.tsx` - Переключатель
- `time-picker.tsx` - Выбор времени
- `time-picker-wheel.tsx` - Барабанный выбор времени
- `input-otp.tsx` - OTP поле

### 🏗️ **layout/** - Структура и компоновка

- `card.tsx` - Карточка
- `separator.tsx` - Разделитель
- `sidebar.tsx` - Боковая панель
- `sheet.tsx` - Выдвижная панель
- `drawer.tsx` - Выдвижной ящик
- `scroll-area.tsx` - Область прокрутки
- `resizable.tsx` - Изменяемый размер
- `aspect-ratio.tsx` - Соотношение сторон

### 🧭 **navigation/** - Навигация

- `breadcrumb.tsx` - Хлебные крошки
- `navigation-menu.tsx` - Навигационное меню
- `menubar.tsx` - Панель меню
- `tabs.tsx` - Вкладки
- `pagination.tsx` - Пагинация
- `accordion.tsx` - Аккордеон
- `collapsible.tsx` - Сворачиваемый блок

### 🔔 **feedback/** - Уведомления и статусы

- `toast.tsx` - Всплывающие уведомления
- `toaster.tsx` - Контейнер уведомлений
- `sonner.tsx` - Альтернативные уведомления
- `alert.tsx` - Предупреждения
- `alert-dialog.tsx` - Диалог предупреждения
- `progress.tsx` - Прогресс-бар
- `skeleton.tsx` - Скелетон загрузки
- `badge.tsx` - Значки

### 📊 **data-display/** - Отображение данных

- `table.tsx` - Таблица
- `chart.tsx` - Графики
- `calendar.tsx` - Календарь
- `avatar.tsx` - Аватар

### 🎭 **overlays/** - Модальные окна и всплывающие элементы

- `dialog.tsx` - Диалоговое окно
- `popover.tsx` - Всплывающее окно
- `tooltip.tsx` - Подсказка
- `hover-card.tsx` - Карточка при наведении
- `dropdown-menu.tsx` - Выпадающее меню
- `context-menu.tsx` - Контекстное меню
- `command.tsx` - Командная палитра

### 📱 **media/** - Медиа компоненты

- `carousel.tsx` - Карусель

### 🔧 **utils/** - Утилиты и базовые компоненты

- `button.tsx` - Кнопка
- `label.tsx` - Метка
- `toggle.tsx` - Переключатель
- `toggle-group.tsx` - Группа переключателей
- `use-toast.ts` - Хук уведомлений

## 🚀 Как использовать

### Импорт из главного index

```typescript
import { Button, Input, Dialog } from "@/components/ui";
```

### Импорт из конкретной категории

```typescript
import { Button } from "@/components/ui/utils/button";
import { Input } from "@/components/ui/inputs/input";
import { Dialog } from "@/components/ui/overlays/dialog";
```

### Импорт всей категории

```typescript
import * as Forms from "@/components/ui/forms";
import * as Layout from "@/components/ui/layout";
```

## ✅ Преимущества новой структуры

1. **Логическая группировка** - Компоненты сгруппированы по функциональности
2. **Лучшая навигация** - Легко найти нужный компонент
3. **Масштабируемость** - Простое добавление новых компонентов
4. **Обратная совместимость** - Все старые импорты работают через главный index
5. **Четкая документация** - Понятное разделение ответственности

## 🔄 Миграция

Все существующие импорты продолжают работать благодаря главному `index.ts`:

```typescript
// ✅ Это продолжает работать
import { Button } from "@/components/ui";

// ✅ Это тоже работает
import { Button } from "@/components/ui/utils/button";
```
