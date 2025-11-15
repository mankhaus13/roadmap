# Git Workflow для roadmap

## Для студентов

### Вариант 1: Fork (рекомендуется)
Студент получает свою копию и может синхронизироваться с обновлениями.

**Шаг 1: Fork репозитория**
1. Зайди на https://github.com/savinmikhail/roadmap
2. Нажми кнопку "Fork" вверху справа
3. Теперь у тебя есть своя копия!

**Шаг 2: Клонируй свой fork**
```bash
git clone https://github.com/ТвойUsername/roadmap.git
cd roadmap
```

**Шаг 3: Добавь upstream (связь с оригиналом)**
```bash
git remote add upstream https://github.com/savinmikhail/roadmap.git
```

**Шаг 4: Работай и сохраняй прогресс**
```bash
# После того как выполнил задачи
git add .
git commit -m "Progress: completed stage 1.3"
git push origin main
```

**Шаг 5: Получай обновления от ментора**
Когда ментор обновил roadmap:
```bash
git fetch upstream
git merge upstream/main
# Или если хочешь перезаписать свои изменения:
# git reset --hard upstream/main
```

---

### Вариант 2: Template (проще, но без синхронизации)
Если не хочешь возиться с Git.

**В GitHub**:
1. Зайди на https://github.com/savinmikhail/roadmap
2. Нажми "Use this template" → "Create a new repository"
3. Назови свой репо (например, "my-roadmap")
4. Clone и работай

**Минус**: не получится автоматически подтягивать обновления от ментора.
