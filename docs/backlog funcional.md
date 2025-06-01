# Backlog Funcional

O backlog funcional é uma lista organizada de funcionalidades que um sistema deve implementar para atender às necessidades dos usuários. Ele serve como um guia para o desenvolvimento do software, definindo o que precisa ser feito, por que e para quem.

O backlog funcional do projeto Oásis segue o formato de histórias de usuário, representando os requisitos funcionais sob a perspectiva do usuário final. Elas seguem um formato padrão:

“Eu, como [tipo de usuário], quero [ação] para [benefício].”

Esse formato ajudará a equipe de software a entender quem vai usar a funcionalidade, o que a pessoa deseja fazer e por que tal funcionalidade é importante.

Os requisitos funcionas foram classificados utilizando o MoSCoW, técnica utilizada para definir a prioridade de cada funcionalidade no backlog.

<br>

<table>
  <thead>
    <tr>
      <th>Épico</th>
      <th>Feature</th>
      <th>ID</th>
      <th>História de Usuário</th>
      <th>MoSCoW</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3">E01<br>Coleta de Telemetria</td>
      <td>F01<br>Conexão ao servidor embarcado</td>
      <td>US01</td>
      <td>Eu, como operador, quero conectar o software ao servidor embarcado no foguete para iniciar a leitura dos dados de voo.</td>
      <td>Must</td>
    </tr>
    <tr>
      <td>F02<br>Requisição de dados JSON</td>
      <td>US02</td>
      <td>Eu, como operador, quero requisitar os dados do voo em formato JSON para processá-los no sistema.</td>
      <td>Must</td>
    </tr>
    <tr>
      <td>F03<br>Persistência dos dados</td>
      <td>US03</td>
      <td>Eu, como operador, quero salvar os dados coletados em um banco de dados para uso posterior e comparação entre lançamentos.</td>
      <td>Must</td>
    </tr>
    <tr>
      <td rowspan="3">E02<br>Análise de Voo</td>
      <td>F04<br>Visualização gráfica</td>
      <td>US04</td>
      <td>Eu, como operador, quero visualizar gráficos de aceleração e velocidade para analisar a trajetória do foguete.</td>
      <td>Must</td>
    </tr>
    <tr>
      <td>F05<br>Indicadores de desempenho</td>
      <td>US05</td>
      <td>Eu, como operador, quero ver a altura máxima, tempo de voo e distância final para verificar se os requisitos de alcance foram atendidos.</td>
      <td>Should</td>
    </tr>
    <tr>
      <td>F06<br>Análise comparativa</td>
      <td>US06</td>
      <td>Eu, como operador, quero comparar os dados entre os três lançamentos para calibrar o foguete com base nos resultados.</td>
      <td>Could</td>
    </tr>
    <tr>
      <td rowspan="3">E03<br>Interface com o Usuário</td>
      <td>F07<br>Dashboard interativo</td>
      <td>US07</td>
      <td>Eu, como operador, quero navegar entre as telas de conexão, gráficos e análise para usar o sistema com facilidade.</td>
      <td>Should</td>
    </tr>
    <tr>
      <td>F08<br>Exportação dos dados</td>
      <td>US08</td>
      <td>Eu, como operador, quero exportar os dados dos lançamentos em CSV para realizar análises externas.</td>
      <td>Could</td>
    </tr>
    <tr>
      <td>F09<br>Exportar relatório em PDF</td>
      <td>US09</td>
      <td>Eu, como operador, quero exportar os gráficos e dados em formato .PDF para documentar o desempenho do foguete.</td>
      <td>Could</td>
    </tr>
    <tr>
      <td rowspan="1">E04<br>Calibração de Trajetória</td>
      <td>F10<br>Ajuste por parâmetros</td>
      <td>US10</td>
      <td>Eu, como operador, quero visualizar os dados de entrada como pressão, volume e ângulo para entender seu impacto no desempenho.</td>
      <td>Should</td>
    </tr>
  </tbody>
</table>


## Histórico de versões

| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|17/05/2025| Criação do documento de backlog funcional | [Carlos Rodrigues](https://github.com/Carlos-kadu) |    |    |
|`1.1`|01/06/2025| Adição do histórico de versões e ajuste na US04 | [Carlos Rodrigues](https://github.com/Carlos-kadu) |    |    |