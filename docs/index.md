<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*&lt;Sistema Falcão Sombrio para Drones&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Alexandre Eiji Tomimura Carvalho
* João Pedro Pioltini de Oliveira
* Luiz Eduardo Bacha dos Santos
* Matheus Veiga Bacetic Joaquim

# Descrição do Projeto

O **Sistema Falcão Sombrio** é um projeto para a reformulação da arquitetura de software dos drones bélicos autônomos da **Securus Dynamics**, visando melhorar sua eficiência, segurança e operação remota.

O sistema enfrentará desafios em **sistemas operacionais** (concorrência, segurança e tempo real) e **banco de dados** (distribuição, replicação e auditoria), garantindo comunicação segura e controle inteligente da frota de drones.

A **Consultoria Cyber Bullet System (Turma 4G)** foi contratada para modelar o novo sistema utilizando UML, cobrindo requisitos, diagramas e documentação técnica, conforme um planejamento estruturado em fases.

---

# Análise de Requisitos Funcionais e Não-Funcionais

## **Requisitos Funcionais**

<table>
    <tr>
        <th>ID</th>
        <th>Referência</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>1</td>
        <td><strong>Central de Controle</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>1.1</td>
        <td>- Interface para gerenciamento de frotas de drones.</td>
        <td>Uma interface que permite gerenciar a frota de drones, proporcionando uma visualização e controle.</td>
    </tr>
    <tr>
        <td>1.2</td>
        <td>- Controle remoto e autônomo dos drones.</td>
        <td>Permite controlar os drones manualmente e de forma autônoma, oferecendo flexibilidade nas operações.</td>
    </tr>
    <tr>
        <td>1.3</td>
        <td>- Dashboard em tempo real com telemetria.</td>
        <td>Um painel que exibe dados de telemetria dos drones em tempo real, garantindo todas as informações importantes.</td>
    </tr>
    <tr>
        <td>2</td>
        <td><strong>Sistema de Navegação Inteligente</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>2.1</td>
        <td>- Sensoriamento do ambiente via LIDAR, câmeras e GPS.</td>
        <td>Utiliza LIDAR, câmeras e GPS para coletar dados do ambiente e orientar os drones de maneira precisa.</td>
    </tr>
    <tr>
        <td>2.2</td>
        <td>- Detecção e evasão de ameaças em tempo real.</td>
        <td>Detecta ameaças e realiza manobras evasivas em tempo real para evitar colisões e outros perigos, mantendo a segurança dos drones.</td>
    </tr>
    <tr>
        <td>2.3</td>
        <td>- Operação autônoma baseada em redes neurais.</td>
        <td>Utiliza inteligência artificial baseada em redes neurais para operar os drones de forma autônoma.</td>
    </tr>
    <tr>
        <td>3</td>
        <td><strong>Gerenciamento de Comunicação</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>3.1</td>
        <td>- Protocolos para comunicação segura e em tempo real com os drones.</td>
        <td>Protocolos que garantem comunicação segura e em tempo real entre os drones e a central de controle.</td>
    </tr>
    <tr>
        <td>3.2</td>
        <td>- Mecanismos de fallback para evitar perda de conexão.</td>
        <td>Estratégias para manter a comunicação estável e evitar a perda de conexão com a central.</td>
    </tr>
    <tr>
        <td>4</td>
        <td><strong>Banco de Dados e Auditoria</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>4.1</td>
        <td>- Logs de missões realizadas e eventos críticos.</td>
        <td>Registro detalhado das missões e eventos críticos ocorridos durante a operação dos drones, para consulta e análise futura.</td>
    </tr>
    <tr>
        <td>4.2</td>
        <td>- Criptografia de ponta e assinaturas digitais.</td>
        <td>Utilização de criptografia avançada e assinaturas digitais para garantir que os dados sejam seguros e autênticos.</td>
    </tr>
    <tr>
        <td>4.3</td>
        <td>- Banco de dados NoSQL distribuído para dados em tempo real.</td>
        <td>Sistema de banco de dados distribuído que permite atualizações e acessos em tempo real, garantindo mais eficiência.</td>
    </tr>
    <tr>
        <td>5</td>
        <td><strong>Sistemas Embarcados e Segurança</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>5.1</td>
        <td>- Autenticação de operadores via biometria e autenticação multifator.</td>
        <td>Autenticação dos operadores utilizando biometria e múltiplos fatores de segurança, para garantir que apenas pessoas autorizadas tenham acesso.</td>
    </tr>
    <tr>
        <td>5.2</td>
        <td>- Monitoramento de processos do SO embarcado para evitar falhas.</td>
        <td>Monitoramento dos processos do sistema operacional dos drones, para prever e evitar falhas, garantindo uma operação estável.</td>
    </tr>
</table>

---

## **Requisitos Não Funcionais**

<table>
    <tr>
        <th>ID</th>
        <th>Referência</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>1</td>
        <td><strong>Arquitetura Deficiente</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>1.1</td>
        <td>- O sistema deve ter baixa latência e não sofrer interrupções de comunicação durante missões críticas.</td>
        <td>O sistema deve garantir comunicação contínua e rápida durante missões críticas, evitando qualquer tipo de atraso ou interrupção.</td>
    </tr>
    <tr>
        <td>2</td>
        <td><strong>Problemas de Segurança</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>2.1</td>
        <td>- Implementação de um modelo robusto de autenticação e criptografia para evitar invasões e tomada de controle não autorizada.</td>
        <td>Deve ser implementado um modelo de segurança robusto que inclui autenticação forte e criptografia para proteger contra acessos não autorizados.</td>
    </tr>
    <tr>
        <td>2.2</td>
        <td>- O armazenamento de logs de auditoria deve ser imutável e altamente disponível.</td>
        <td>Os logs de auditoria devem ser armazenados de forma que não possam ser alterados e devem estar disponíveis a qualquer momento para consulta.</td>
    </tr>
    <tr>
        <td>3</td>
        <td><strong>Gerenciamento de Banco de Dados</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>3.1</td>
        <td>- O sistema deve garantir a integridade e a sincronização dos dados dos drones em tempo real.</td>
        <td>O sistema deve assegurar que os dados dos drones sejam precisos e sincronizados em tempo real para uma operação eficiente.</td>
    </tr>
    <tr>
        <td>3.2</td>
        <td>- O histórico de missões precisa ser armazenado para auditorias e análise preditiva.</td>
        <td>O histórico das missões dos drones deve ser registrado para fins de auditoria e para realizar análises preditivas.</td>
    </tr>
    <tr>
        <td>3.3</td>
        <td>- Banco de dados distribuído e replicado para garantir a continuidade da operação.</td>
        <td>Deve ser utilizado um banco de dados distribuído e replicado para assegurar a continuidade das operações mesmo em caso de falhas.</td>
    </tr>
    <tr>
        <td>4</td>
        <td><strong>Sistemas Operacionais e Concorrência</strong></td>
        <td></td>
    </tr>
    <tr>
        <td>4.1</td>
        <td>- Os drones operam em um sistema operacional embarcado que precisa gerenciar múltiplas threads de sensores, navegação e IA.</td>
        <td>O sistema operacional dos drones deve ser capaz de gerenciar várias threads simultâneas para sensores, navegação e inteligência artificial.</td>
    </tr>
    <tr>
        <td>4.2</td>
        <td>- O sistema deve ser capaz de priorizar processos conforme o status crítico da missão.</td>
        <td>O sistema deve ter a capacidade de priorizar processos dependendo da criticidade de cada missão, garantindo que tarefas essenciais tenham prioridade.</td>
    </tr>
</table>

# Diagrama de Atividades
<table>
    <tr>
        <td><img src="src/diagrama.jpg" width="500" height="600"></td>
    </tr>
</table>
*&lt;Diagrama para visualizer as pessoas das áreas de negócios e de desenvolvimento de uma organização para entender o processo e comportamento.&gt;*

# Diagrama de Casos de Uso

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

# Diagrama de Sequência

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
