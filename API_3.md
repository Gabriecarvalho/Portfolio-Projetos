<html>
<body>
 <h1 align="center"> API 3º Semestre - 02/2024</h1>
<h1 align="center"> 
<a href="https://github.com/CODEPLAY-Fatec/API-ADS-3-Sem-Fatec"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://youtan.com.br/">Youtan</a></h2>
 
<img src="./Imagens/logo-youtan.png" height="100" width="230"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto visa resolver o problema da empresa parceira relacionado à dificuldade de registrar avaliações e autoavaliações em equipes grandes e dispersas. A solução proposta pela Youtan foi desenvolver um Dashboard para Feedback e Pesquisa de Clima e Cultura, que permitiu a automação e a aceleração na aplicação das pesquisas no sistema. Isso foi feito por meio de uma plataforma onde o RH pode cadastrar perguntas multidimensionais e categorizar as respostas de líderes, liderados e autoavaliações em painéis visuais para monitorar a evolução individual e coletiva. Essa abordagem ofereceu um acompanhamento contínuo do desenvolvimento da equipe, proporcionando a promoção do bem-estar, a motivação dos colaboradores e a redução dos índices de turnover.
 
 <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
<!-- Figma -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" width="100" height="100" title="Figma" alt="Figma" />

<!-- MySQL -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original-wordmark.svg" width="100" height="100" title="MySQL" alt="MySQL" />

<!-- React -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original-wordmark.svg" width="100" height="100" title="React" alt="React" />

<!-- JavaScript -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" width="100" height="100" title="JavaScript" alt="JavaScript" />

<!-- TypeScript -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="100" height="100" title="TypeScript" alt="TypeScript" />

<!-- Node.js -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg" width="100" height="100" title="Node.js" alt="Node.js" />
</div>
 
    
    
<br>
<ul>
  <li>
    <a href="https://www.figma.com/">Figma</a>: É uma ferramenta de design de interface (UI) e experiência do usuário (UX) baseada em nuvem. Permite a criação de protótipos, wireframes e a colaboração em tempo real.
  </li>
  <li>
    <a href="https://www.mysql.com/">MySQL</a>: É um sistema de gerenciamento de banco de dados (SGBD) relacional, ou seja, que utiliza a linguagem SQL como interface. É amplamente utilizado para armazenar e gerenciar dados de forma estruturada.
  </li>
  <li>
    <a href="https://react.dev/">React</a>: É uma biblioteca JavaScript de código aberto focada na criação de interfaces de usuário (UI). Baseada em componentes, ela facilita o desenvolvimento de aplicações web interativas e dinâmicas (Front-end).
  </li>
  <li>
    <a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">JavaScript</a>: É uma linguagem de programação fundamental para o desenvolvimento web. Permite a implementação de itens complexos, interatividade, animações e atualizações dinâmicas nas páginas.
  </li>
  <li>
    <a href="https://www.typescriptlang.org/">TypeScript</a>: É um superconjunto (superset) de JavaScript criado pela Microsoft que adiciona tipagem estática opcional à linguagem. Isso facilita a detecção de erros durante o desenvolvimento e melhora a manutenção de grandes projetos.
  </li>
  <li>
    <a href="https://nodejs.org/">Node.js</a>: É um ambiente de execução JavaScript construído com o motor V8 do Google Chrome. Ele permite que os desenvolvedores utilizem JavaScript para escrever código no lado do servidor (Back-end), criando aplicações de rede rápidas e escaláveis.
  </li>
</ul>

<h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end e Front-end</h3>
  <p align="justify" style="font-family:roboto;"> Atuei como desenvolvedor neste projeto, com foco inicial na modelagem do banco de dados para otimizar as relações hierárquicas entre equipes, líderes e liderados. Em paralelo, fui responsável por estruturar a arquitetura base do back-end, definindo uma organização de pastas limpa e modular para facilitar a manutenção e escalabilidade do código.

 <details>

<summary>Funções de Autenticação</summary>

<p> Aqui estão algumas funções de autenticação e middleware que eu fiz no backend

<p align="center">
      <img src="./Imagens/login API3.png" alt="auth">
      <img src="./Imagens/middleware API3.png" alt="auth">
      <img src="./Imagens/criar usuario API3.png" alt="auth">
    </p>

</details>

No desenvolvimento do back-end, implementei as regras de negócio para o gerenciamento de equipes. Criei a lógica de alocação de usuários, garantindo restrições importantes de permissão: liderados não têm privilégios para adicionar novos membros, e um usuário não pode ocupar simultaneamente os papéis de líder e liderado no mesmo time. Além disso, estruturei todo o sistema de segurança e acesso da plataforma. Isso incluiu o fluxo de cadastro, o sistema de login com geração e validação de tokens JWT para proteção das rotas, e a funcionalidade de alteração de senha.

<details>

<summary>Funções relacionadas ao time</summary>

<p>Aqui estão algumas funções que eu construi no backend relacionadas ao time</p>

<p align="center">
    <img src="./Imagens/funcao adiciona ao time API3.png" alt="team">
    <img src="./Imagens/funcao adiciona time API3.png" alt="team">
    <img src="./Imagens/outras funçoes time API3.png" alt="team">
    </p>

</details>

Já no front-end, construí a interface de visualização de times do usuário logado, criando uma separação clara e intuitiva entre as equipes que ele lidera e as que ele apenas integra. Também fui responsável pelo desenvolvimento das telas de cadastro e login, realizando a integração completa e o consumo da API com o back-end para ambas as funções. Além disso, implementei um middleware de proteção de rotas, garantindo o controle de acesso e impedindo que usuários não autenticados ou sem permissão acessassem páginas restritas da aplicação.

<details>

<summary>Meu papel no front-end</summary>

<p>Aqui estão algumas partes do frontend que eu fiz como a navbar, e a pagina de times.</p>

<p align="center">
      <img src="./Imagens/navbar funcao API3.png" alt="navbar">
    </p>

</details>

<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>

Durante o desenvolvimento desse projeto de Dashboard para Feedback e Pesquisa de Clima e Cultura de equipes
para a Youtan, pude adquirir diversos aprendizados significativos que contribuíram para o meu crescimento e desenvolvimento como desenvolvedor.

Este projeto foi uma excelente oportunidade para aprofundar minha expertise em desenvolvimento Full-Stack. No back-end, consolidei meus conhecimentos na infraestrutura e organização de projetos em Node.js, focando em uma arquitetura limpa e modular. Também pude implementar do zero um sistema de autenticação seguro com tokens JWT, além de evoluir bastante na modelagem e nos relacionamentos do banco de dados. Já no front-end, mergulhei no ecossistema do React, compreendendo na prática a componentização em uma arquitetura SPA (Single Page Application). Por fim, consegui aprimorar significativamente minhas habilidades de design de interface e usabilidade, garantindo uma navegação muito mais fluida para o usuário.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="270px">Tecnologia/Metodologia</th>
      <th width="85px">Nota</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Figma</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>React</td>
      <td>★★★☆☆</td>
    <td>Entendi</td>
    </tr>	
    <tr>
      <td>Mysql</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Javascript</td>
      <td>★★★☆☆</td>
    <td>Entendi</td>
    </tr>
   <tr>
      <td>Typescript</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>Nodejs</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>GIT</td>
      <td>★★★★★</td>
    <td>Sei fazer com autonimia</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="270px">Habilidade</th>
      <th width="280px">Descrição</th>
    </tr>
    <tr>
      <td>Proatividade</td>
      <td>Colaboração constante com o time e integração entre front-end e back-end.</td>
    </tr>
    <tr>
      <td>Trabalho em equipe</td>
      <td>Precisei aprender a utilizar os conhecimtentos que adquiri sobre java e llm e junta-los no projeto.</td>
    </tr>
    <tr>
      <td>Soluçao de problema</td>
      <td>Atuação na solução de gargalos técnicos e otimizações de performance.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>
 
* [1º Semestre: Agile learn - Plataforma web para aprender sobre metodologia ágil Scrum](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_1.md)
* [2º Semestre: SQL Chat Bot - Aplicação que permite acessar informações de um banco de dados MySQL usando exclusivamente a linguagem natural](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_2.md)
* [3º Semestre: Quantum - Dashboard para Feedback e Pesquisa de Clima e Cultura de equipes](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_3.md)
* [4º Semestre(ADS): FAPG - Sistema Intituitivo para Gestão de Projetos de Pesquisa e Desenvolvimento Tecnológico de uma fundação](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_4_ADS.md)
* [4º Semestre(Banco de dados): Projeto Sistema de Monitoramento e Mobilidade Urbana](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_4.md)
* [5º Semestre: TODO](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_5.md)
* [6º Semestre: TODO](https://github.com/Gabriecarvalho/Portfolio-Projetos/blob/main/API_6.md)

</body>
</html>
