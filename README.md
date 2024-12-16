# Обрезка ссылок с помощью Битли

Этот проект позволяет сокращать ссылки с помощью API ВКонтакте и получать статистику по кликам для сокращённых ссылок.

### Как установить

1. Получите ключ к API VK:
   - Зайдите в [ВКонтакте для разработчиков](https://vk.com/dev).
   - Создайте приложение.
   - Получите сервисный токен API VK.

2. Создайте файл .env в корне проекта и добавьте ваш токен в следующем формате:
VK_ACCESS_TOKEN=replace_with_your_access_token

3. Python3 должен быть уже установлен.

4. Используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:

```bash
pip install -r requirements.txt
```
Рекомендуется использовать [virtualenv/venv](https://docs.python.org/3/library/venv.html) для изоляции проекта.

### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).