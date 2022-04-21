@startuml
left to right direction
actor Авториз._пользователь as AP
usecase "Управление подписками" as UC1
usecase "Мониторинг интерисующего контента" as UC2
usecase "Отмена подписки" as UC3
usecase "Оформление подписки" as UC4
usecase "Оформление подписок ранее" as UC5
usecase "Поиск/ просмотр каталога подписок" as UC6
AP - UC2
AP - UC1
UC1 ..> UC3 : Include
UC1 ..> UC4 : Include 
UC5 ..> UC2 : Extend
UC6 ..> UC4 : Extend
@enduml