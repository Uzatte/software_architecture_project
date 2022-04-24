### Описание сценариев исспользования приложения

#### Сценарии исспользования приложения предствавлены ниже:

1. Запись тренировки

**Цель:** Целью данного сценария является фиксация и запись результатов тренировки пользоватля.

**Описание:**
Пользователь открывает меню записи тренировки, выбирает нужный тип тренировки и нажимает **начать**. Система начинает фиксировать показатели тренировки пользователя, исспользуя датчики на его смартфоне, а также датчики других носимых устройств, если такие подключены. После окончания тренировки, данные о ней записываются во временное хранилище на смартфоне пользователя, или на смарт-часах пользователя, если приложение было запущено с них. Далее система пытается выгрузить данные о тренировке с устройства пользователя в базу данных приложения. В случае успеха данные о тренировке попадают в личный профиль пользователя. Если по каким-то причинам данные о тренировке не улалось выгрузить на сервер нашего приложения - попытки выгрузи будут предприниматься далее до достижения успеха. (система будет автоматически пытаться выгрузить данные через следующие интервалы: 1, 5, 10, 30, 60, 400, 3600 минут. Так же будет доступна кнопка принудительной пыпытке выгрузе данных на сервер)

**Схема сценария записи тренировки представлена ниже:**
![Сценарий записи тренироовки](../static/scenario_training_recording.jpeg)