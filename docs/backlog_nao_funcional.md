# Backlog Não-Funcional

O **Backlog Não-Funcional** reúne os requisitos que não dizem respeito diretamente às funcionalidades do sistema, mas que garantem sua qualidade, desempenho, segurança, usabilidade e outros atributos essenciais. Esses requisitos asseguram que o sistema funcione de maneira eficaz, seja confiável, seguro, escalável e mantenha a integridade dos dados e da experiência dos usuários.

## Requisitos

| Requisito | Tipo | Justificativa |
|-----------|------|----------------|
| O sistema deve registrar e armazenar dados de lançamento em até 2 segundos após a coleta | Desempenho | Garante tempo real para análise e resposta dos dados coletados |
| A base de dados deve persistir os dados de cada lançamento com 100% de integridade | Confiabilidade | Evita perda de dados críticos para análise e calibração |
| A interface de análise de dados deve funcionar em desktops e notebooks das equipes | Usabilidade | Permite acesso ao sistema com os dispositivos disponíveis no ambiente escolar |
| O sistema deve proteger contra alterações manuais nos dados armazenados | Segurança | Garante veracidade dos dados para fins de avaliação |
| O software não deve depender de bibliotecas comerciais ou soluções prontas de terceiros | Legalidade | Atende às exigências do projeto pedagógico de autoria própria |
| O sistema deve suportar a entrada de até 3 lançamentos consecutivos por foguete | Escalabilidade | Compatível com a reutilização obrigatória dos foguetes |
| O tempo de carregamento das visualizações não deve ultrapassar 3 segundos com até 3 lançamentos | Desempenho | Mantém fluidez e rapidez na apresentação de dados |
| A plataforma de lançamento deve garantir uma zona segura mínima de 5 metros ao redor | Segurança | Protege a integridade física dos envolvidos no experimento |
| A coleta de dados deve ocorrer com precisão mínima de 0,1 unidade nas variáveis medidas | Precisão Técnica | Garante exatidão nas estimativas de trajetória e calibração do foguete |
| O sistema deve ser documentado e compreensível por todos os membros das engenharias envolvidas | Manutenibilidade | Permite colaboração multidisciplinar e futuras melhorias |
| Os dados de posição e altitude devem ser compatíveis com os sensores integrados ao hardware | Compatibilidade | Garante integração entre software e hardware de medição |
| O código-fonte deve seguir boas práticas de programação e versionamento | Qualidade Técnica | Facilita auditoria, revisão por pares e evita plágios entre grupos |


## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|17/05/2025| Criação do página e adição do backlog não funcional | [Rayene Almeida](https://github.com/rayenealmeida) |
|`1.1`|19/05/2025| Adição do Histórico de Versões| [Rayene Almeida](https://github.com/rayenealmeida) |