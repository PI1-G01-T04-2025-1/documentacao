# Dicionário de Dados 

Um dicionário de dados (também conhecido como repositório de metadados) é a espinha dorsal documental de qualquer sistema de banco de dados. Ele funciona como um catálogo centralizado que descreve detalhadamente a estrutura, o significado e as regras dos dados armazenados. Em essência, é uma "enciclopédia" que responde:

- O que cada elemento representa (ex: peso_ZFW = peso do foguete sem combustível);

- Como ele se relaciona com outros dados (ex: FOGUETE_id vincula lançamentos a um foguete específico);

- Quais restrições aplicam-se (ex: campos obrigatórios, tipos de dados como UUID ou NUMERIC(10,2)).

# Dicionário de Dados - Projeto Oásis

## Entidade: FOGUETE  
*Descrição*: Contém informações dos foguetes utilizados nos lançamentos.  

| Atributo  | Propriedades do Atributo       | Tipo de Dado | Tamanho | Descrição                          |
|-----------|--------------------------------|--------------|---------|------------------------------------|
| id        | Chave primária, obrigatório    | UUID         | \-      | Identificador do foguete          |
| nome      | Obrigatório                    | VARCHAR      | \-      | Nome do foguete                   |
| peso_ZFW  | Obrigatório                    | NUMERIC      | 10,2    | Peso do foguete sem água (Zero Fuel Weight) |

---

## Entidade: LANCAMENTO  
*Descrição*: Contém os dados relacionados aos lançamentos de foguetes com água.  

| Atributo           | Propriedades do Atributo              | Tipo de Dado | Tamanho | Descrição                                |
|--------------------|---------------------------------------|--------------|---------|------------------------------------------|
| id                 | Chave primária, obrigatório           | UUID         | 11      | Identificador do lançamento             |
| data_hora          | Obrigatório                           | DATE         | \-      | Data e hora do lançamento               |
| angulo_inicial     | Obrigatório                           | REAL         | 2       | Ângulo inicial do lançamento            |
| nivel_agua         | Obrigatório                           | NUMERIC      | 300     | Nível de água no momento do lançamento  |
| pressao_inicial    | Obrigatório                           | REAL         | 4       | Pressão inicial no lançamento           |
| massa_foguete_total| Obrigatório                           | NUMERIC      | 10,2    | Massa total do foguete                  |
| FOGUETE_id         | Chave estrangeira, obrigatório        | UUID         | \-      | ID do foguete utilizado no lançamento   |

---

## Entidade: DADOCOLETADO  
*Descrição*: Contém os dados registrados durante o lançamento de um foguete.  

| Atributo      | Propriedades do Atributo       | Tipo de Dado | Tamanho | Descrição                                      |
|---------------|--------------------------------|--------------|---------|------------------------------------------------|
| id            | Chave primária, obrigatório    | UUID         | \-      | Identificador do dado coletado                |
| LANCAMENTO_id | Chave estrangeira, obrigatório | UUID         | \-      | ID do lançamento ao qual os dados pertencem   |
| posicoes      | Obrigatório                    | REAL         | \-      | Posição registrada durante o voo              |
| velocidade    | Obrigatório                    | REAL         | \-      | Velocidade registrada durante o voo           |
| tempo         | Obrigatório                    | REAL         | \-      | Tempo registrado correspondente aos dados     |

## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|26/05/2025| Criação do Dicionário de Dados | [Patrícia Silva](https://github.com/Patyhelenaa), [David Wiliiam](https://github.com/sluucke) e [Ingrid Alves](https://github.com/alvesingrid) |
|`1.1`|02/06/2025| Criação do documento | [Patrícia Silva](https://github.com/Patyhelenaa) |