```mermaid
---
title: Diagrama de Casos de Uso - Projeto de Drone
---

actor Operador
actor Sistema_de_Monitoramento
actor Usuario_Final
actor Drone

Operao_Autenticar_Usuario --> Operador
Operao_Atribuir_Tarefa --> Operador
Operao_Executar_Tarefa --> Drone
Operao_Detectar_Ameaca --> Drone
Operao_Desviar_de_Ameaca --> Drone
Operao_Trocar_Dados --> Drone --> Sistema_de_Monitoramento
Operao_Retornar_Ponto_Base --> Drone
Operao_Abortar_Missao --> Operador

rectangle Casos_de_Uso {
    Operao_Autenticar_Usuario[Autenticar Usurio]
    Operao_Atribuir_Tarefa[Atribuir Tarefa ao Drone]
    Operao_Executar_Tarefa[Executar Tarefa]
    Operao_Detectar_Ameaca[Detectar Ameaa]
    Operao_Desviar_de_Ameaca[Desviar de Ameaa]
    Operao_Trocar_Dados[Trocar Dados com o Sistema]
    Operao_Retornar_Ponto_Base[Retornar ao Ponto Base]
    Operao_Abortar_Missao[Abortar Misso]
}

note right of Sistema_de_Monitoramento
    Recebe dados do drone durante a misso.
end note

note left of Usuario_Final
    Utiliza os resamenteultados das misses.
end note
