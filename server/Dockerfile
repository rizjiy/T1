# Используем официальный образ Node.js
FROM node:14

# Создаем рабочую директорию
WORKDIR /usr/src/app

# Копируем package.json и package-lock.json
COPY package*.json ./

# Устанавливаем зависимости
RUN npm install

# Копируем все остальные файлы в рабочую директорию
COPY . .

# Открываем порт, который будет использовать приложение
EXPOSE 5000

# Команда для запуска приложения
CMD ["npm", "start"]
