# Инструкция по использованию RPA для автоматического инвайта в Discord каналы.

#### Требования для корректной работы: ```Google Таблица с настройками каналов.```

---
1. **Настроить каналы в Google Таблице. Указать названия каналов и инвайт ссылки.**

<img width="575" height="123" alt="изображение" src="https://github.com/user-attachments/assets/5bf87921-25bc-423c-b800-bd28cbbf5c9c" />

---
2. **В интерфейсе AdsPower выберите профили, на которых будет осуществляться автоматизация. (Можно скопировать разом все из таблицы и просто вставить в строку)**

<img width="1279" height="510" alt="изображение" src="https://github.com/user-attachments/assets/eafce50e-bb08-45d5-b92e-a5fb5f3bdd09" />

---
3. **Запустите процесс RPA, связанный с инвайтами в Discord: в меню RPA выберите нужный процесс.**

<img width="812" height="91" alt="изображение" src="https://github.com/user-attachments/assets/62d8f7a6-4085-4e4b-b7df-ebe50db7c9db" />

---
4. **Нажмите кнопку запуска и дождитесь выполнения. Посмотреть ход процесса можно в журнале задач («Task Log») AdsPower.**

<img width="783" height="541" alt="изображение" src="https://github.com/user-attachments/assets/efbc8dc7-7a8f-45d9-9b35-b1d9d0a77cd7" />

---
**Посмотреть логи на предмет успешного или ошибочного выполнения RPA можно в каталоге:** ```~/.config/adspower_global/cwd_global/source/data```

<img width="873" height="587" alt="изображение" src="https://github.com/user-attachments/assets/1b716e42-419e-44ff-bde8-5137f5bfc795" />

---
# Статусы:
**invite_<название_канала>_status-<номер_задачи>.txt** - ```В текстовом файле указан номер профиля и рядом true (успешный) или false (неудачный) вход в канал.```

**invite_<номер_профиля>_discord_not_login-<номер_задачи>.txt** - ```Discord аккаунт не авторизован.```

**invite_<номер_профиля>_server_limit-<номер_задачи>.txt** - ```Максимальный лимит каналов в Discord, вступить не удалось.```
