---
title: Diagrama de Casos de Uso - Projeto de Drone
---

actor Operador
actor Sistema_de_Monitoramento
actor Usuario_Final
actor Drone

Operador --> (Autenticar Usuário)
Operador --> (Atribuir Tarefa ao Drone)
Operador --> (Abortar Missão)
Drone --> (Executar Tarefa)
Drone --> (Detectar Ameaça)
Drone --> (Desviar de Ameaça)
Drone --> (Trocar Dados com o Sistema)
Drone --> (Retornar ao Ponto Base)
Sistema_de_Monitoramento --> (Trocar Dados com o Sistema)

rectangle Casos_de_Uso {
    (Autenticar Usuário)
    (Atribuir Tarefa ao Drone)
    (Executar Tarefa)
    (Detectar Ameaça)
    (Desviar de Ameaça)
    (Trocar Dados com o Sistema)
    (Retornar ao Ponto Base)
    (Abortar Missão)
}

note right of Sistema_de_Monitoramento
    Recebe dados do drone durante a missão.
end note

note left of Usuario_Final
    Utiliza os resultados das missões.
end note
