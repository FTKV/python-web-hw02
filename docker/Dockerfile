# Docker-команда FROM вказує базовий образ контейнера
# Наш базовий образ - це Linux з попередньо встановленим python-3.10
FROM python:3.11

# Встановимо змінну середовища
ENV APP_HOME /app/bot_assistant

# Встановимо робочу директорію всередині контейнера
WORKDIR $APP_HOME

# Скопіюємо інші файли в робочу директорію контейнера
COPY . .

RUN pip install .
# RUN useradd -ms /bin/bash user
# USER user
# WORKDIR /home/user

# Запустимо наш застосунок всередині контейнера
ENTRYPOINT ["bot-assistant"]