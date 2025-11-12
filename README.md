# Courses Project

## Установка и запуск

```bash
# Клонирование репозитория
git clone https://github.com/XanderWhite/courses.git .
git checkout -b xander origin/xander

# Backend (Laravel)
cd backend/
composer install
# Настроить .env файл

# Frontend (React)
cd frontend/
npm install

# Запуск
cd frontend/
npm start

cd backend/
php artisan serve

# Добавить секретные ключи
https://github.com/XanderWhite/courses
Settings → Secrets and variables → Actions → New repository secret

cat C:\Users\Xande\.ssh\projects_deploy
HOSTING_SSH_KEY = результат пред. команды

# Данные ssh
HOSTING_HOST = 77.222.40.85
HOSTING_USER = xanderbel2
REACT_APP_API_URL = https://xanderwhite.ru/projects/courses/public

# Создаем ветки
git checkout -b hosting
git push origin hosting

# Создать файл и добавить настройки для автодеплоя
.github/workflows/deploy.yml

git add .github/workflows/deploy.yml
git commit -m "Add deploy workflow"
git push origin hosting