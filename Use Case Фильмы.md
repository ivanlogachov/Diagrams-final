@startuml
left to right direction
actor Авториз._пользователь as AP
actor "Платежная_сист" as PS
usecase "Просмотр списка покупок" as UC2
usecase "Просмотр каталога" as UC1
usecase "Приобретение фильма" as UC3
usecase "Взять на прокат" as UC4
usecase "Купить" as UC5
AP -- UC1
AP - UC2
PS - UC3
UC1 ..> UC3 : Include
UC4 ..> UC3 : Extend 
UC5 ..> UC3 : Extend
@enduml