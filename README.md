# Обрезка ссылок с помощью Битли

Этот проект позволяет сокращать ссылки с помощью API ВКонтакте и получать статистику по кликам для сокращённых ссылок.

### Как установить

1. Получите ключ к API VK:
   - Зайдите в [ВКонтакте для разработчиков](https://vk.com/dev).
   - Создайте приложение.
   - Получите сервисный токен API VK.
   

2. Создайте файл .env в корне проекта и добавьте ваш токен в следующем формате:
```
VK_ACCESS_TOKEN=replace_with_your_access_token
```

3. Python3 должен быть уже установлен.


4. Используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:

```bash
pip install -r requirements.txt
```
Рекомендуется использовать [virtualenv/venv](https://docs.python.org/3/library/venv.html) для изоляции проекта.

### Как запустить

**Скрипт поддерживает два режима работы:**
1. **Сокращение ссылки.**

Запустите скрипт, указав ссылку, которую нужно сократить. 

Например:
```bash
python main.py https://example.com
```
Результат будет выглядеть следующим образом:
```
Короткая ссылка: https://vk.cc/example
```

2. **Получение статистики по короткой ссылке.**

Укажите короткую ссылку, чтобы узнать количество кликов:
```bash
python main.py https://vk.cc/example
```
Результат:
```
Количество кликов: 123
```
Если что-то пошло не так, вы увидите сообщение об ошибке.

### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).