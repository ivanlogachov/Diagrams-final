@startuml
left to right direction
actor Пользователь as P
usecase "Авторизация" as UC1
usecase "Ввести номер телефона/эл.почту" as UC2
usecase "Ввести пароль" as UC3
usecase "Регистрация" as UC4
usecase "Заполнить форму данных" as UC5
usecase "Придумать пароль" as UC6
usecase "Согласиться с условиями политики сервиса" as UC7
usecase "Подтверждение телефонного номера/эл.почты" as UC8
P -- UC1
P -- UC4
UC1 ..> UC2 : Include
UC1 ..> UC3 : Include 
UC4 ..> UC5 : Include
UC4 ..> UC6 : Include
UC4 ..> UC7 : Include
UC4 ..> UC8 : Include
@enduml