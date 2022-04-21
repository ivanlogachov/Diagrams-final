@startuml
left to right direction
actor Пользователь as P
actor Авториз._пользователь as AP
usecase "Просмотр контента" as UC1
usecase "Управление просмотром" as UC2
usecase "Настройки просмотра" as UC3
P <|- AP
P -- UC1
UC2 ..> UC1 : Extend
UC3 ..> UC1 : Extend
@enduml