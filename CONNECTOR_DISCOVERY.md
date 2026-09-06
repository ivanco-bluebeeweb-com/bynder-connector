# Bynder Connector — Discovery

**Vendor:** Bynder (https://bynder.com)  
**API Base URL:** `https://api.bynder.com/api/v4`  
**Authentication:** OAuth 2.0 Bearer Token / Permanent Token

## Архитектура API
- **Ключевые сущности:** медиа-активы (/media), коллекции (/collections), мета-свойства и теги (/metaproperties), процесс загрузки (/media/upload)
- **Формат обмена данными:** JSON / HTTPS REST.
- **Обработка ошибок:** Стандартные HTTP-коды (400, 401, 403, 404, 429, 500) с типизацией ответа.
- **Тестовая точка проверки подключения:** `GET /api/v4/media`.
