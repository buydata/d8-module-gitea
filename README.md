# Модуль Gitea для Deckhouse

Этот модуль разворачивает Gitea в кластере Kubernetes с использованием Deckhouse.

## Параметры

- `enabled`: Включить/выключить развертывание Gitea.
- `serviceName`: Название сервиса.
- `deploymentName`: Название деплоймента.
- `image`: Настройки образа Gitea.
- `resources`: Ресурсы для подов.
- `servicePort`: Порт, на котором будет доступен Gitea.
- `containerPort`: Внутренний порт контейнера.
- `postgres`: Настройки PostgreSQL.
- `persistence`: Настройки persistent volume.
- `configMap`: Конфигурационный файл Gitea.

## Пример использования

```yaml
gitea:
  enabled: true
  postgres:
    password: mysecretpassword
```