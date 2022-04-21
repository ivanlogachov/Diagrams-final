@startuml
left to right direction
actor "Пользователь" as P
actor "Авторизированный пользователь" as AP
actor "Платежная система" as PS
usecase "Регистрация" as UC1
usecase "Поиск контента (Навигатор)" as UC2
usecase "Просмотр контента" as UC3
usecase "Проигрыватель" as UC4
usecase "Shorts" as UC5
usecase "Управление поступающим контентом" as UC6
usecase "Другие возможности" as UC7
usecase "Спорт" as UC8
usecase "Трансляции" as UC9
usecase "Видеоигры" as UC10
usecase "Фильмы" as UC11
usecase "Приобретение" as UC12
usecase "Просмотр каталога" as UC13
usecase "Навигатор" as UC14
usecase "Подписки" as UC15
usecase "Оформлении подписок ранее" as UC16
usecase "Библиотека просмотров" as UC17
usecase "Просмотр контента ранее" as UC18
usecase "Управление профелем (Настройка)" as UC19
P <|- AP
P -- UC1
P -- UC2
P -- UC3
AP -- UC6
AP -- UC19
PS -- UC12
UC3 .> UC4 : Include
UC3 ..> UC5 : Include
UC6 ..> UC7 : Include
UC6 ..> UC8 : Include
UC6 ..> UC9 : Include
UC6 ..> UC10 : Include
UC6 ..> UC11 : Include
UC11 ..> UC12 : Include
UC13 ..> UC12 : Extend
UC6 ..> UC14 : Include
UC6 ..> UC15 : Include
UC6 ..> UC17 : Include
UC16 ..> UC15 : Extend
UC18 ..> UC17 : Extend
@enduml