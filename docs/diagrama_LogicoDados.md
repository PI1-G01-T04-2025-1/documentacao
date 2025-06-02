# Diagrama Lógico de Dados

O **DLD (Diagrama Lógico de Dados)** é uma etapa fundamental no projeto de bancos de dados, responsável por transformar o modelo conceitual (DER) em uma estrutura técnica preparada para implementação física. Enquanto o DER foca em _"o que"_ o sistema precisa armazenar (entidades, atributos e relacionamentos), o DLD define _"como"_ esses elementos serão organizados no banco de dados, detalhando:
No exemplo gerado com **BrModelo** também, o DLD materializa o DER da seguinte forma:

1. **Estrutura de Tabelas**:
    
    - Tabela `FOGUETE` = colunas: `id` (UUID, chave primária), `nome` (VARCHAR), `peso_ZFW` (NUMERIC).
        
    - Tabela `LANÇAMENTO` = herda todos os atributos do DER + `FOGUETE_id` (UUID, chave estrangeira apontando para `FOGUETE`).
        
    - Tabela `DADOCOLETADO` = vincula-se a `LANÇAMENTO` via `LANCAMENTO_id` (chave estrangeira).
        
2. **Implementação de Relacionamentos**:
    
    - A relação "um foguete realiza múltiplos lançamentos" (1,n) vira a chave estrangeira `FOGUETE_id` na tabela `LANÇAMENTO`.
        
    - A relação "um lançamento gera múltiplos dados" (1,n) transforma-se na chave `LANCAMENTO_id` na tabela `DADOCOLETADO`.


![diagrama Lógico de Dados](imgs/diagrama_logicoDados.jpg)
> 🛈 Versão 01 do DLD

## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|26/05/2025| Modelagem do DLD| [Patrícia Silva](https://github.com/Patyhelenaa),[David Wiliiam](https://github.com/sluucke) e [Ingrid Alves](https://github.com/alvesingrid) |
|`1.1`|02/06/2025| Criação do documento | [Patrícia Silva](https://github.com/Patyhelenaa) |