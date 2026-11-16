Практическая работа по отработке BIOS/UEFI в Lenovo BIOS Simulator Center

  Задача 1. Навигация по основным разделам
Цель: Запомнить структуру меню UEFI.
Задание: Последовательно откройте разделы Main, Config, Security, Startup, Restart. Выпишите, какая информация отображается в Main (серийный номер, версия UEFI, тип CPU).
<img width="889" height="638" alt="image" src="https://github.com/user-attachments/assets/858bfec8-e68b-46a8-9fc0-c028eb812b15" />
 
 Задача 2. Смена порядка загрузки
Цель: Научиться менять приоритет загрузочных устройств.
Задание: Перейдите в Startup → Boot. Сделайте USB первым, NVMe — вторым. Запомните клавишу сохранения (F10).
<img width="404" height="263" alt="image" src="https://github.com/user-attachments/assets/02946e9e-b005-4c54-ae64-4b354e3af20e" />

  Задача 3. Включение/выключение Secure Boot
Цель: Понять назначение Secure Boot.
Задание: Перейдите в Security → Secure Boot. Проверьте статус, переключите на противоположный, верните обратно. Отметьте, требуется ли перезагрузка.
Выполнено: При отключении перезагрузка потребуется, но на эмуляторе это не требуется
  
  Задача 4. Установка пароля супервизора
Цель: Отработать установку пароля администратора UEFI.
Задание: Перейдите в Security → Password → Supervisor Password. Установите пароль Test1234. Попробуйте изменить любую настройку — должен появиться запрос пароля. Затем сбросьте пароль.
<img width="823" height="276" alt="image" src="https://github.com/user-attachments/assets/e375fe57-bfe2-4405-8ef1-8b5b7106515d" />
Выполнено: Запрос будет запрашиваться, но на эмуляторе это не работает

  Задача 5. Сброс на заводские настройки
Цель: Научиться возвращать UEFI к исходному состоянию.
Задание: Перейдите в Restart → Load Factory Defaults (или F9). Подтвердите сброс. Проверьте, что настройки из задач 2–4 сброшены.
<img width="816" height="182" alt="image" src="https://github.com/user-attachments/assets/40469e37-a3e9-4c86-a889-b837403910e2" />

  Задача 6. Управление встроенными устройствами
Цель: Отработать управление периферией на низком уровне.
Задание: Перейдите в Config → USB. Найдите USB BIOS Support или Always On USB. Отключите, затем включите обратно. Запишите точный путь.
Выполнено: При переключении USB BIOS Support или Always On USB пользоваться usb устройствами будет невозможно

  Задача 7. Режим работы SATA/NVMe
Цель: Понять разницу между режимами контроллера.
Задание: Перейдите в Config → Storage → SATA Controller Mode (или NVMe Mode). Посмотрите варианты (AHCI / RAID / Intel RST), переключите и верните обратно. Обратите внимание на предупреждения.
Выполнено: в эмуляторе Storage отсутствует
<img width="405" height="486" alt="image" src="https://github.com/user-attachments/assets/2e333767-680c-4fd1-ba29-2eac06969328" />

  Задача 8. Временное меню загрузки (эмуляция F12)
Цель: Научиться использовать Boot Menu без изменения постоянных настроек.
Задание: Найдите опцию Startup → Boot Mode или эмуляцию F12 Boot Menu. Активируйте, затем вернитесь в главное меню.

  Задача 9. Просмотр системных логов
Цель: Научиться диагностировать проблемы через UEFI.
Задание: Перейдите в Main → System Summary (или Config → Diagnostics). Найдите раздел с логами POST/событий. Просмотрите их, найдите Clear Event Log (если есть) и очистите.
Выполнено: Также как и storage отсутвует в эмуляторе 

  Задача 10. Полный сценарий: подготовка к переустановке ОС
Цель: Закрепить все навыки в одном практическом задании.
Задание (последовательно):

Сбросить настройки на Factory Defaults (1 мин).
Включить Secure Boot (1 мин).
Установить Supervisor Password (2 мин).
Поставить USB первым в порядке загрузки (2 мин).
Сохранить и выйти (F10) (1 мин).
Снова войти, проверить настройки, сбросить пароль и вернуть порядок загрузки (2 мин).
<img width="826" height="194" alt="image" src="https://github.com/user-attachments/assets/d7f5c28c-e283-47ac-9223-c261531e1095" />
<img width="816" height="269" alt="image" src="https://github.com/user-attachments/assets/6e4c8d97-671a-4930-ab83-dcccf522ac44" />
<img width="579" height="54" alt="image" src="https://github.com/user-attachments/assets/4ecb4d13-b5d1-4f86-8cf1-eaf569df2063" />
<img width="351" height="221" alt="image" src="https://github.com/user-attachments/assets/1ad02120-0e4c-4fee-82bc-8e79d45d7eb0" />
<img width="604" height="167" alt="image" src="https://github.com/user-attachments/assets/cc6ed274-c761-4d20-82ad-79f7ae120eba" />





