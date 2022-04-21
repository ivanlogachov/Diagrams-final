@startuml
left to right direction
actor Авториз._пользователь as AP
actor "Пользователь" as P
usecase "Поиск контента" as UC1
usecase "Ввод запроса" as UC2
usecase "Отображение актуального контента" as UC3
usecase "Выбор типа/тематики контента" as UC4
usecase "Фильмы" as UC5
usecase "Поиск в каталоге фильмов" as UC6
P <|- AP
AP -- UC5
P -- UC1
P -- UC3
UC1 ..> UC2 : Include
UC4 .> UC3 : Extend 
UC5 ..> UC6 : Include
@enduml