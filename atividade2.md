# Atividade 2: Papéis, Responsabilidades e Matriz RACI

## 1. Papel Analisado
* **Papel escolhido:** Desenvolvedor Backend (Backend Developer).

## 2. Diferença entre Responsabilidade e Competência
* **Responsabilidade:** É a obrigação ou o dever que o profissional tem de entregar uma tarefa específica dentro do projeto (por exemplo, o desenvolvedor backend é responsável por criar as rotas de pagamento e garantir que a API funcione).
* **Competência:** São as habilidades, conhecimentos técnicos e comportamentais que a pessoa possui para conseguir executar essa responsabilidade com qualidade (por exemplo, dominar Node.js, saber escrever código limpo, ter boa comunicação e pensar em segurança).

## 3. Competências Técnicas e Comportamentais
* **Técnicas (Hard Skills):** Domínio de linguagens de programação, banco de dados, testes unitários, controle de versão (Git) e padrões de segurança de API.
* **Comportamentais (Soft Skills):** Trabalho em equipe, proatividade para identificar bugs antes que cheguem em produção, atenção aos detalhes e boa comunicação com a equipe de testes (QA).

## 4. Por que a Qualidade é uma Responsabilidade Compartilhada?
* A qualidade não é um problema exclusivo do testador ou do analista de QA. Se o desenvolvedor escreve um código mal estruturado, o analista de testes vai sofrer para testar e o cliente vai ter falhas no sistema. Por isso, desde o PO (Product Owner) que define os requisitos, passando pelos devs que codificam, até o QA que valida, todo mundo tem papel ativo em garantir que o software funcione bem e entregue valor.

## 5. Matriz RACI para o Projeto
*(Legenda: R = Responsável / Accountable, A = Autoridade / A, C = Consultado / Consulted, I = Informado / Informed)*

| Atividades / Processos do Projeto | Product Owner (PO) | Desenvolvedor (Dev) | Analista de QA | Tech Lead |
| :--- | :---: | :---: | :---: | :---: |
| Definição de Requisitos e Critérios de Aceite | **R / A** | C | C | I |
| Desenvolvimento do Código (Funcionalidades) | I | **R / A** | C | C |
| Planejamento e Criação de Casos de Teste | I | C | **R / A** | I |
| Execução de Testes e Relatório de Bugs | I | C | **R / A** | I |
| Homologação e Decisão de Deploy | **R / A** | I | C | C |

## 6. Lacuna Identificada e Práticas de QA Propostas
* **Lacuna identificada:** No início do projeto, a equipe costumava deixar os testes para a última hora, apenas quando o sistema já estava pronto, o que gerava atrasos e retrabalho para corrigir os bugs.
* **Práticas de QA propostas:** Adotar testes unitários obrigatórios feitos pelo próprio desenvolvedor antes de subir o código, além de integrar o analista de QA desde a fase de refinamento dos requisitos para antecipar cenários de erro e evitar falhas estruturais.
