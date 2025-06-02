# Diagrama de Arquitetura

O diagrama de arquitetura é uma representação visual essencial no desenvolvimento de software, funcionando como um guia para estruturar e compreender um sistema. Ele oferece uma visão holística de como os componentes internos interagem entre si e com entidades externas, facilitando a comunicação entre stakeholders, apoiando decisões de design e servindo como referência para implementação e manutenção futura. Ao expor as relações entre as partes do sistema, também ajuda a identificar gargalos potenciais ou desafios de integração.

No diagrama em análise, observamos uma estrutura organizada em **duas camadas fundamentais**: o **frontend (lado do cliente)** e o **backend (servidor)**. No frontend, a aplicação NexJs juntamente com TaliwindCSS para estilização oferece uma interface dinâmica e funcional, concentrando-se em operações **CRUDs** (criação, consulta, atualização e exclusão de dados) e um **Dashboard** para visualização e análise de informações.

No backend, o ambiente **NodeJS** e o framework **ExpressJS** estabelecem as rotas REST que viabilizam a comunicação com o **Supabase**, responsável pelo armazenamento e gestão de dados. Essa camada processa a lógica de negócios para entidades específicas como **Lançamento**, **Foguete** e **Sensor**, gerenciando suas operações CRUDs e configurando a integração com o banco de dados.

A comunicação entre as camadas ocorre exclusivamente via **protocolo HTTP e APIs REST**, garantindo interoperabilidade e controle de fluxo. O frontend solicita ações ao backend, que por sua vez consolida e persiste os dados no Supabase, retornando respostas para atualização da interface do usuário.

Essa arquitetura proporciona uma solução robusta e escalável para monitoramento de foguetes e sensores, onde a separação clara de responsabilidades — interface (frontend), regras de negócio (backend) e armazenamento (Supabase) — otimiza a manutenção e permite adaptações futuras. O uso de tecnologias modernas como ExpressJS e Supabase ainda agiliza o desenvolvimento e assegura a confiabilidade das operações de dados.

![diagrama de estados](imgs/diagrama_Arquitetura.png)
> 🛈 Versão 01 do diagrama de arquitetura

## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|26/05/2025| Modelagem do diagrama de Arquitetura | [Patrícia Silva](https://github.com/Patyhelenaa) e [David Wiliiam](https://github.com/sluucke) |
|`1.1`|01/06/2025| Criação do documento | [Patrícia Silva](https://github.com/Patyhelenaa) |