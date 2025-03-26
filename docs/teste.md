# Diagrama de Caso de Uso – Projeto Drone

```mermaid
%% Diagrama de Caso de Uso para o Projeto Drone
%% Atores: Piloto e Estação de Controle
%% Casos de Uso: Iniciar Missão, Cancelar Missão, Verificar Status, Decolar, Navegar, Realizar Tarefas (como Capturar Imagens e Realizar Inspeção),
%% Monitorar Bateria, Monitorar Status em Tempo Real e Enviar Comandos.

usecaseDiagram
    actor Piloto
    actor "Estação de Controle" as Estacao

    Piloto --> (Iniciar Missão)
    Piloto --> (Cancelar Missão)
    
    (Iniciar Missão) --> (Verificar Status do Drone)
    (Iniciar Missão) --> (Decolar)
    (Iniciar Missão) --> (Navegar)
    (Iniciar Missão) --> (Realizar Tarefas)
    
    (Realizar Tarefas) --> (Capturar Imagens)
    (Realizar Tarefas) --> (Realizar Inspeção)
    
    (Navegar) --> (Monitorar Bateria)
    
    Estacao --> (Monitorar Status em Tempo Real)
    Estacao --> (Enviar Comandos)
