# Especificações de Caso de Testes

Os testes de software são fundamentais para assegurar a qualidade e a confiabilidade dos sistemas, atuando como uma barreira crítica contra falhas. Essa prática consiste em executar o programa com o objetivo explícito de identificar erros e verificar se seu comportamento está alinhado aos requisitos especificados. Além de detectar defeitos existentes, os testes ajudam a prevenir problemas futuros, conferindo maior segurança quanto à estabilidade e funcionalidade do produto final.

A especificação de testes formaliza esse processo ao estruturar os cenários de validação em um roteiro claro e sistemático. Ela define as condições de execução, os passos a serem seguidos, as entradas e os resultados esperados para cada caso, servindo como base para avaliar a conformidade com os requisitos do usuário. Para isso, utiliza-se uma tabela de casos de teste, que organiza cada cenário por meio de colunas como ID (identificador único do caso de teste, que permite rastreamento e referência rápida), Objetivo do Teste (descrição clara do que se pretende validar), Pré-condições (estado necessário do sistema antes da execução), Entradas (valores ou ações fornecidos ao sistema), Passos (sequência de ações a serem realizadas), Resultado Esperado (comportamento ou saída que o sistema deve apresentar) e Prioridade (grau de importância do teste, que auxilia na organização da execução). Essa estrutura organizada garante rastreabilidade, cobertura abrangente dos requisitos e validação minuciosa das funcionalidades — elementos essenciais para assegurar a qualidade e a confiabilidade do resultado final.

# Tabela especificação de Casos de Teste - Sofware

| ID   | Objetivo do Teste                        | Pré-condições               | Entrada                            | Passos                                                                 | Resultado Esperado                                     | Prioridade |
|------|------------------------------------------|-----------------------------|------------------------------------|------------------------------------------------------------------------|--------------------------------------------------------|------------|
| CT01 | Verificar inicialização da aplicação     | Sistema instalado           | Nenhuma                            | 1. Iniciar o sistema                                                  | Tela inicial da aplicação é exibida                    | Alta       |
| CT02 | Validar entrada de dados iniciais        | Aplicação iniciada          | Pressão, volume e ângulo           | 1. Inserir dados<br>2. Confirmar entrada                              | Dados são aceitos e armazenados                        | Alta       |
| CT03 | Verificar conexão com servidor embarcado | Dados iniciais inseridos    | Nenhuma                            | 1. Clicar em conectar<br>2. Aguardar resposta                          | Sistema conecta ao servidor e exibe confirmação        | Alta       |
| CT04 | Testar reconexão após falha              | Conexão inicial falhou      | Opção de tentar novamente          | 1. Selecionar “tentar novamente”<br>2. Aguardar reconexão             | Reconexão realizada com sucesso ou tentativa encerrada | Média      |
| CT05 | Validar coleta de dados                  | Conectado ao servidor       | Nenhuma                            | 1. Iniciar coleta<br>2. Aguardar leitura de dados                      | Dados são recebidos com sucesso                        | Alta       |
| CT06 | Testar falha na coleta                   | Conectado ao servidor       | Comunicação interrompida ou erro   | 1. Iniciar coleta<br>2. Simular erro                                  | Sistema detecta falha e informa ao usuário             | Alta       |
| CT07 | Verificar salvamento de dados no banco   | Dados coletados com sucesso | Nenhuma                            | 1. Finalizar coleta<br>2. Aguardar confirmação                         | Dados persistidos corretamente no banco                | Alta       |
| CT08 | Gerar gráficos com dados salvos          | Dados salvos no banco       | Nenhuma                            | 1. Solicitar geração de gráficos                                      | Gráficos são exibidos na tela                          | Alta       |
| CT09 | Visualizar gráficos                      | Gráficos gerados            | Nenhuma                            | 1. Acessar seção de visualização                                      | Gráficos são exibidos de forma clara                   | Alta       |
| CT10 | Exportar dados                           | Dados disponíveis           | Seleção de tipo de exportação      | 1. Escolher “exportar dados”<br>2. Selecionar formato<br>3. Confirmar | Processo de exportação iniciado                        | Média      |
| CT11 | Exportar dados como PDF                  | Dados disponíveis           | Selecionar exportação PDF          | 1. Iniciar exportação<br>2. Selecionar “PDF”<br>3. Confirmar          | Arquivo PDF é gerado corretamente                      | Baixa      |
| CT12 | Exportar dados como CSV                  | Dados disponíveis           | Selecionar exportação CSV          | 1. Iniciar exportação<br>2. Selecionar “CSV”<br>3. Confirmar          | Arquivo CSV é gerado corretamente                      | Baixa      |


## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|28/05/2025| Criação das especificaçÕes de caso de teste para software| [Patrícia Silva](https://github.com/Patyhelenaa) e [Ingrid Alves](https://github.com/alvesingrid) |
|`1.1`|02/06/2025| Criação do documento | [Patrícia Silva](https://github.com/Patyhelenaa) |