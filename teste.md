---
title: Diagrama de Casos de Uso - Projeto de Drone
---

actor Operador
actor Sistema_de_Monitoramento
actor Usuario_Final
actor Drone

Operador --> Operao_Autenticar_Usuario
Operador --> Operao_Atribuir_Tarefa
Operador --> Operao_Abortar_Missao
Drone --> Operao_Executar_Tarefa
Drone --> Operao_Detectar_Ameaca
Drone --> Operao_Desviar_de_Ameaca
Drone --> Operao_Trocar_Dados
Drone --> Operao_Retornar_Ponto_Base
Sistema_de_Monitoramento --> Operao_Trocar_Dados

rectangle Casos_de_Uso {
    Operao_Autenticar_Usuario[Autenticar Usuário]
    Operao_Atribuir_Tarefa[Atribuir Tarefa ao Drone]
    Operao_Executar_Tarefa[Executar Tarefa]
    Operao_Detectar_Ameaca[Detectar Ameaça]
    Operao_Desviar_de_Ameaca[Desviar de Ameaça]
    Operao_Trocar_Dados[Trocar Dados com o Sistema]
    Operao_Retornar_Ponto_Base[Retornar ao Ponto Base]
    Operao_Abortar_Missao[Abortar Missão]
}

note right of Sistema_de_Monitoramento
    Recebe dados do drone durante a missão.
end note

note left of Usuario_Final
    Utiliza os resultados das missões.
end note
