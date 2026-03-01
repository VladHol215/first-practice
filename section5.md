```mermaid
useCaseDiagram
    actor "Клієнт" as C
    actor "Процесинговий центр" as P
    actor "Підтримка" as S

    package "Система Онлайн-Банкінгу" {
        usecase "Авторизація" as UC1
        usecase "Переказ коштів" as UC2
        usecase "Керування лімітами" as UC3
        usecase "Аналітика витрат" as UC4
        usecase "Чат з підтримкою" as UC5
    }

    C --> UC1
    C --> UC2
    C --> UC3
    C --> UC4
    C --> UC5
    UC2 --> P
    UC5 --> S
    ```