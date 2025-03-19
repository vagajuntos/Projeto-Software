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

<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th>ID</th>
      <th>Referência</th>
      <th>Sub ID</th>
      <th>Referência</th>
      <th>Descrição</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Central de Controle</td>
      <td>1.1</td>
      <td>Interface para gerenciamento de frotas de drones</td>
      <td>A central de controle é responsável por atribuir tarefas e pelo controle manual e autônomo dos drones, além da coleta de dados em tempo real.</td>
    </tr>
    <tr>
      <td>1</td>
      <td>Central de Controle</td>
      <td>1.2</td>
      <td>Controle remoto e autônomo dos drones</td>
      <td>A central de controle é responsável por atribuir tarefas e pelo controle manual e autônomo dos drones, além da coleta de dados em tempo real.</td>
    </tr>
    <tr>
      <td>1</td>
      <td>Central de Controle</td>
      <td>1.3</td>
      <td>Dashboard em tempo real com telemetria</td>
      <td>A central de controle é responsável por atribuir tarefas e pelo controle manual e autônomo dos drones, além da coleta de dados em tempo real.</td>
    </tr>
    
---

## **Requisitos Não Funcionais**

1. **Arquitetura Deficiente**  
   - O sistema deve ter baixa latência e não sofrer interrupções de comunicação durante missões críticas.  

2. **Problemas de Segurança**  
   - Implementação de um modelo robusto de autenticação e criptografia para evitar invasões e tomada de controle não autorizada.  
   - O armazenamento de logs de auditoria deve ser imutável e altamente disponível.  

3. **Gerenciamento de Banco de Dados**  
   - O sistema deve garantir a integridade e a sincronização dos dados dos drones em tempo real.  
   - O histórico de missões precisa ser armazenado para auditorias e análise preditiva.  
   - Banco de dados distribuído e replicado para garantir a continuidade da operação.  

4. **Sistemas Operacionais e Concorrência**  
   - Os drones operam em um sistema operacional embarcado que precisa gerenciar múltiplas threads de sensores, navegação e IA.  
   - O sistema deve ser capaz de priorizar processos conforme o status crítico da missão.  

<table>
   <tr>
      <th>Funcionais/Não Funcionais</th>
      <th>Arquitetura deficiente</th>
      <th>Problemas de segurança</th>
      <th>Gerenciamento de banco de dados</th>
      <th>Sistemas operacionais e concorrências</th>
      </tr>
   
   <tr>
      <td>Central de controle</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
   </tr>

   <tr>
      <td>Sistema de navegação</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
   </tr>
      
   <tr>
      <td>Gerenciamento de Comunicaçao</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>     
   </tr>
      
   <tr>  
      <td>Banco de dados e auditoria</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
   </tr>
      
   <tr>   
      <td>Sistema de embarcados e segurança</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
      <td>1</td>
   </tr>
   
</table>

# Diagrama de Atividades

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
