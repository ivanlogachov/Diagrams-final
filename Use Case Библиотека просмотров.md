@startuml
left to right direction
actor Авториз._пользователь as AP
usecase "История просмотров" as UC1
usecase "Просмотр контента ранее" as UC2
usecase "Смотреть позже" as UC3
usecase "Установка метки ранее" as UC4
usecase "Редактирование списка" as UC5
usecase "Плейлисты" as UC6
usecase "Редактирование списка отобранных плейлистов ранее" as UC7
usecase "Сохранение плейлистов других пользователей ранее" as UC8
usecase "Понравившиеся" as UC9
usecase "Редактирование списка" as UC10
usecase "Установка лайка ранее" as UC11
AP -- UC1
AP -- UC3
AP -- UC6
AP -- UC9
UC2 ..> UC1 : Extend
UC4 ..> UC3 : Extend
UC3 ..> UC5 : Include
UC6 .> UC7 : Include 
UC8 ..> UC6 : Extend
UC9 ..> UC10 : Include
UC11 ..> UC9 : Extend
@enduml