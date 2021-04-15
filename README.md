# zelenka-geo-maps

Наборы данных в формате GeoJSON и скрипты для их автоматизации

## Как редактировать зоны

### Через Яндекс.Карты

Для работы потребуется Яндекс.Аккаунт (любой).

1. Переходим в [Конструктор карт Яндекса](https://yandex.ru/map-constructor/)
2. Если не вошли в аккунт, жмём "Войти" в правом верхнем углу
3. Нажимаем кнопку "Импорт" слева
   Если открыта карта, то "Список карт", там "К импорту ->"
4. В окно Импорт загружаем файл зоны (напр., *spb_basezone.geo.json*)
5. Редактируем зону перетаскивая точки
   > ⚠️ Обязательно меняем версию в названии! Принцип описан ниже.
6. Жмём "Сохранить и продолжить"
7. Рядом с "Карта готова" жмём "Экспорт"
8. Выбираем "GEO JSON" и жмём "Скачать"

## Как версионировать

Следуем принципам [semver - семантического версионирования](https://semver.org/lang/ru/)

Версия всегда вида **X.Y.Z**:

- При исправлении небольших ошибок, внесении незаметных/неважных для пользователя изменений, меняем число **Z** (например, с 1.1.2 до 1.1.3).
   *пример:* добавили точек для красоты, или немного сдвинули зону в месте, где нет жилых домов.
- При добавлении нововведений или внесении видимых важных, но не глобальных изменениях, мы меняем число **Y** (например, с 2.9.2 до 2.10.0).
   *пример:* сдвинули зону в одном месте.
- При глобальных изменениях, влияющих на общий пользовательский опыт, мы меняем число **X** (например, с 5.3.19 до 6.0.0).
   *пример:* полностью пересмотрели зону и сильно изменили границы

Каждое обновление может содержать также исправления меньшего порядка. В этом случае учитываем только наибольший значимый номер версии.

# License \ Лицензия

All GeoJSON files are licensed under the [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) (if not explicitly mentioned otherwise)
All other files are licensed under the [ISC License](LICENSE.md) (if not explicitly mentioned otherwise)

Все GeoJSON файлы доступны под лицензией [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) (если не указано иное)
Все остальные файлы доступны под лицензией [ISC](LICENSE.md) (если не указано иное)
