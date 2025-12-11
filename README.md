gochat/
├── cmd/
│   └── app/
│       └── main.go        # Точка входа. DI-контейнер, инициализация.
├── internal/
│   ├── config/            # Загрузка конфигурации
│   ├── domain/            # Models, Errors, Interfaces (Contract definitions)
│   │   ├── models.go
│   │   └── errors.go
│   ├── usecase/           # Бизнес-логика (Service layer)
│   ├── repository/        # Реализация интерфейсов хранилища (Postgres, Redis)
│   └── delivery/          # Транспортный слой
│       └── http/          # HTTP Handlers, Routing, Middleware
├── pkg/                   # Общие утилиты (Logger, Validator)
├── migrations/            # SQL миграции
├── docker-compose.yml
├── Makefile
└── go.mod
.golangci.yml