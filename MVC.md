# Ponderada 02: Arquitetura em Esboço do MVC em Sails

## Arquitetura em esboço MVC

&nbsp;&nbsp;&nbsp;&nbsp; O desenvolvimento inicial da arquitetura MVC da aplicação WEB foi produzida a partir do framework Sails.js e segue os seguintes parâmetros:

Model - Camada que comporta os dados principais da aplicação, possui comunicação direta com o banco de dados, responsável por armazenar e recuperar esses dados do próprio banco.

View - Camada com os elementos visuais destinados ao cliente, armazena o código HTML, o CSS e as rotinas JavaScript.

Controller -  Camada intermediária entre as outras, é responsável por fazer a interatividade entre o que é pedido no view e o que é acessado no model.

&nbsp;&nbsp;&nbsp;&nbsp; Dessa forma, foi estruturado o seguinte escopo para as páginas idealizadas do projeto até o momento:

<br>
<div align="center">
<sub>Figura 1 - Tela inicial estudante</sub>
<img src="/assets/01.jpg" width="100%" >
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>
<br>

A tela inicial idealizada para os estudantes foi estruturada a partir da localização dos aspectos visuais (view), como o slider do medidor de felicidade e o carrossel de atividades a fazer, ligando-os ao back-end (controller) que capta as informações, como o valor do medidor de felicidade, as tags escolhidas ou as atividades restantes, armazenadas no banco de dados (model) e permite a visualização desses dados de forma mais intuitiva pelos usuários.

<br>
<div align="center">
<sub>Figura 2 - Tela inicial tutor</sub>
<img src="/assets/02.jpg" width="100%" >
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>
<br>

A tela inicial idealizada para os tutores foi estruturada a partir da localização dos aspectos visuais (view), como a lista do alunos, de grupos e o carrossel de tarefas a fazer, ligando-os ao back-end (controller) que capta as informações armazenadas no banco de dados (model), com o id dos alunos tutorados, seus respectivos grupos, seus nomes, o id do tutor, entre outras informações, e permite a visualização dos dados de forma mais intuitiva pelos usuários.

<br>
<div align="center">
<sub>Figura 3 - Tela de login</sub>
<img src="/assets/03.jpg" width="100%" >
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>
<br>

A tela de login idealizada para o site foi estruturada a partir da localização dos elementos visuais (view) que naturalmente compõem uma tela de login, como a área de digitar o user e senha, e o botão de enviar as informações. Seguindo essa lógica, o back-end (controller) é introduzido para permitir a usabilidade de cada uma dessas funções, que devem também ser ligados a um banco de dados (model) com informações que permitam a funcionalidade do login.

<br>
<div align="center">
<sub>Figura 4 - Tela de perfil</sub>
<img src="/assets/04.jpg" width="100%" >
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>
<br>

A tela de perfil idealizada para o site foi estruturada de forma que tornasse obrigatório o preenchimento dos dados importantes para a utilização da plataforma e desse opção para adição de dados extra. Dessa forma, elementos visuais (view) permitem a intuitividade das funções de cada campo de digitação ou seleção de alternativas - habilidades -, que são controladas pelo back-end (controller) que fornecem uso a esses espaços e os liga ao banco de dados (model), responsável por receber e armazenar os dados preenchidos na página e no login.

<br>
<div align="center">
<sub>Figura 5 - Tela de formulário</sub>
<img src="/assets/05.jpg" width="100%" >
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>
<br>

A tela de formulários idealizada para o site foi estruturada a partir da análise de interfaces pré-existentes dessa categoria. A partir disso, elementos visuais (view) como campos de digitação, de seleção de alternativas e o botão de salvamento são comandados a partir do back-end (controller) que permite a usabilidade de cada uma dessas funções e as conecta ao banco de dados (model), fazendo com que todas as informações coletadas sejam salvas e armazenadas para um uso fuuro.

## Explicação da arquitetura

&nbsp;&nbsp;&nbsp;&nbsp; Os diagramas são montados a partir da divisão de usos que cada um dos elementos (view, model e controller) exercem, contando com subdivisões que permitem o entendimento das funções analisadas, por exemplo: carrossel de atividades no view, funções do carrossel no controller e dados utilizados das atividades no model da arquitetura da tela de login (figura 03). Todos esses elementos estão dentro de um guarda-chuva sistem, que abrange a aplicação web como um todo, conectada a um usuário (user do Chrome) e a um banco de dados (Render).

&nbsp;&nbsp;&nbsp;&nbsp; Ademais, as subvisões de cada um dos elementos view, controller e model são ligadas entre si por meio da arquitetura que possibilita seu uso pleno dentro da aplicação. Seguindo o mesmo exemplo anterior, as funções do carrossel dependem de um banco de dados com informações a serem postas no seu campo, que da mesma forma, dependem do front-end para serem visualizadas pelo usuário na interface do site. Dessa forma, existem conexões entre cada uma das camadas para dipor o funcionamento da aplicação.

&nbsp;&nbsp;&nbsp;&nbsp; Por fim, a arquitetura MVC permite a visualização de um fluxo de itens a serem cumpridos para o desenvolvimento de uma aplicação web. Nela é facilitado o entendimento de cada uma das partes que compõem a criação do site, como elas se relacionam entre si e com o usuário final ou o banco de dados conectado. Também é possível a criação de um backlog completo de atuação para a concretização do projeto, garantindo que nenhuma de suas partes sejam esquecidas. Por se tratar de um site feito para estudantes e tutores, a arquitetura MVC permite a especificação das API's ideais para esse público e estruturação das colunas necessárias para o gerenciamento dos bancos relacionais por meio das ferramentas como o PostgreSQL e o DBeaver.


