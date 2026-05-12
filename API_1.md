<html>
<body>
 <h1 align="center"> API 1º Semestre - 02/2020</h1>
<h1 align="center"> 
<a href="https://github.com/Grupo-1-2020-PI-FATEC-ADS/SOS-EDUCA"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://fatecsjc-prd.azurewebsites.net/">FATEC São José dos Campos - Prof. Jessen Vidal</a></h2>
 
<img src="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/images/fatecsjc_400x192.png" height="100" width="230"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto consiste na criação de um site de comércio eletrônico (E-commerce) voltado para materiais didáticos. O objetivo principal foi facilitar o acesso e fornecer recursos de qualidade para professores e alunos, com o intuito de apoiar seus estudos e aprimorar o processo de aprendizagem. O site oferece uma ampla variedade de materiais didáticos, abrangendo diversas disciplinas e níveis educacionais. Isso inclui livros, apostilas, e-books, vídeos educativos, planos de aula, jogos educativos, entre outros recursos relevantes para auxiliar tanto os educadores quanto os estudantes.
Uma das principais características do site foi a facilidade de navegação e busca, permitindo que os usuários encontrem rapidamente o conteúdo desejado. Além disso, fornecer recursos de filtragem e classificação, permitindo que os usuários refinem suas pesquisas com base em critérios específicos, como disciplina, nível de ensino, autor, editora, entre outros.
 
 <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
 
 <div style="display: inline_block"><br> 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mysql/mysql-original-wordmark.svg" width="100"    height="100" />	 
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/html5/html5-original-wordmark.svg" width="100"    height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/css3/css3-original-wordmark.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/php/php-plain.svg" width="100" height="100" />
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/javascript/javascript-original.svg" width="100"    height="100" />	
 <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/trello/trello-plain-wordmark.svg" width="100" height="100" />
</div>
 
	
	
<br>
 
  <ul>
  <li><a href="https://www.mysql.com/">MySQL</a>: É um sistema de gerenciamento de banco de dados (SGBD) relacional, ou seja, que utiliza a linguagem SQL como interface. Lançado sobre a licença GPL, possui como desenvolvedor a Oracle Corporation.</p></li>
  </li>	  
  <li><a href="https://html.spec.whatwg.org/multipage/">HTML</a>: É uma linguagem de marcação utilizada para estruturar e organizar o conteúdo das páginas da web. Com suas tags e elementos, permite a criação de textos, imagens, links e formulários, fornecendo a base fundamental para a construção de sites. É complementado por outras tecnologias como CSS e JavaScript para estilização e interatividade.</p></li>
  </li>
   <li><a href="https://www.w3.org/Style/CSS/Overview.en.html">CSS</a>: É uma linguagem de estilo utilizada para definir a apresentação e o layout visual das páginas da web.</p></li>
  </li>
   <li><a href="https://www.php.net/">PHP</a>: É uma linguagem de programação server-side amplamente utilizada para desenvolvimento web. Com sua sintaxe simples e poderosa, permite a criação de sites dinâmicos, interativos e conectados a bancos de dados, possibilitando a construção de aplicativos web robustos.</p></li>
  </li>
   <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">JavaScript</a>: É uma linguagem de programação versátil e poderosa, utilizada para adicionar interatividade, funcionalidades dinâmicas e comportamentos aos sites.</p></li>
  </li>
  <li><a href="https://trello.com/">Trello</a>: É uma ferramenta de gerenciamento de projetos baseada em quadros virtuais que permite organizar tarefas e colaborar em equipes de forma visual e intuitiva.</p></li>
  </li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end e Front-end</h3>
  <p align="justify" style="font-family:roboto;"> Como desenvolvedor nesse projeto, minhas atribuições foram essenciais para a implementação das interfaces do usuário e para garantir uma experiência de usuário fluida e amigável.

Minha contribuição, utilizando PHP, permitiu a implementação da funcionalidade de autenticação de usuários, a persistência de dados por meio de variáveis de sessão e o reaproveitamento de código com a inclusão de arquivos PHP. Essas contribuições foram essenciais para o bom funcionamento e segurança do sistema de login do cliente no projeto.

<details>
	
<summary>Código em PHP - Manipulação dos dados</summary>
 
> Inicialização de sessão: Com a linha "?php session_start(); ?", iniciei uma sessão PHP. Isso permite que armazene e acesse variáveis de sessão, que podem ser usadas para manter dados específicos do usuário entre as requisições.

> Utilizei o PHP para manipular os dados submetidos no formulário de login. O formulário é enviado para o arquivo "autenticando_clientes.php" através do atributo action no elemento "form".
	
```php
 
<?php session_start(); ?>
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <?php include('cabecalho.php');?>
	<title>Login do cliente</title>
</head>
<body>
  <?php include('navbar.php');?>
  <?php (include("progresso.php"))(1);?>
 
  <div class="container">
	<!-- Main Content -->
	<div class="container-fluid">
		<div class="row main-content bg-success text-center">
			<div class="col-md-4 text-center company__info">
				<span class="company__logo"><h2><img src="images/sos.gif" alt="" width="120px" height="120px"></span></h2></img>
			</div>
			<div class="col-md-8 col-xs-12 col-sm-12 login_form ">
				<div class="container-fluid">
					<div class="row">
						<h2>Log In</h2>
					</div>
					<div class="row">
						<form control="" class="form-group" action="autenticando_clientes.php" method="POST">
							<div class="row">
								<input type="text" id="username" class="form__input" name="usuario" value="<?php echo @$_SESSION['usuario']?>"  placeholder="Digite seu Email">
							</div>
							<div class="row">
								<!-- <span class="fa fa-lock"></span> -->
								<input type="password" id="password" class="form__input" name="senha" <?= @$_SESSION['senha'] ? 'autofocus' : '' ?>  maxlength="8" placeholder="Digite sua senha">
							</div>
							<div class="row">
								<input type="submit" value="Login" class="btn2">
							</div>
						</form>
					</div>
				</div>
			</div>
		</div>
  </div>
</div>
</body>
  <?php include('rodape.php');?> 
</body>
</html>

```

</details>  

Realizei a validação do e-mail e senha fornecidos. Verifiquei se ambos os campos foram preenchidos, garantindo que o usuário tenha fornecido as informações necessárias para efetuar o login. Após a validação, utilizei a função fetch para fazer uma chamada assíncrona para o back-end, utilizando o método POST. Enviei os dados do login em formato JSON, incluindo o e-mail e a senha. No back-end, em um arquivo PHP chamado "login.php", os dados recebidos foram processados e a autenticação do usuário foi verificada. A resposta do back-end foi tratada utilizando os métodos then e catch. Em caso de sucesso, os dados retornados pelo back-end foram processados e tratados de acordo. Em caso de erro, qualquer exceção ou falha na chamada foi capturada e tratada adequadamente.

<details>
	
<summary>Código em JavaScript - Validação do Formulário de Login</summary>
 
```javascript

document.getElementById("loginForm").addEventListener("submit", function(event) {
  event.preventDefault();
  var email = document.getElementById("email").value;
  var password = document.getElementById("password").value;
  
  // Realizar validação do email e senha
  if (email && password) {
    // Fazer chamada assíncrona para o back-end em PHP
    fetch("login.php", {
      method: "POST",
      body: JSON.stringify({ email: email, password: password }),
      headers: {
        "Content-Type": "application/json"
      }
    })
    .then(response => response.json())
    .then(data => {
      // Tratar a resposta do back-end
    })
    .catch(error => {
      // Tratar erros
    });
  }
});

```

</details>  
 
Criação e Estilização de Interfaces:
desenvolvi as interfaces do usuário utilizando HTML, CSS e Bootstrap, seguindo as diretrizes de design fornecidas pelo Figma como referência.
Ajudei a criar um layout responsivo que se adaptasse a diferentes dispositivos e tamanhos de tela. Isso permitiu que os usuários acessassem o site de qualquer dispositivo, como computadores, tablets e smartphones, proporcionando uma experiência consistente.
Ao utilizar o Bootstrap, aproveitei os componentes e classes pré-definidos para criar rapidamente interfaces consistentes, economizando tempo e esforço.

<details>
	
<summary>Código em CSS - Estilização do formulário de Login</summary>
	
```css

  .wrapper {
    display: flex;
    align-items: center;
    flex-direction: column; 
    justify-content: center;
    width: 100%;
    min-height: 100%;
    padding: 20px;
  }
  
  #formContent {
    -webkit-border-radius: 10px 10px 10px 10px;
    border-radius: 10px 10px 10px 10px;
    background: #fff;
    padding: 30px;
    width: 90%;
    max-width: 450px;
    position: relative;
    padding: 0px;
    -webkit-box-shadow: 0 30px 60px 0 rgba(0,0,0,0.3);
    box-shadow: 0 30px 60px 0 rgba(0,0,0,0.3);
    text-align: center;
  }
  
  #formFooter {
    background-color: #f6f6f6;
    border-top: 1px solid #dce8f1;
    padding: 25px;
    text-align: center;
    -webkit-border-radius: 0 0 10px 10px;
    border-radius: 0 0 10px 10px;
  }

```
 
</details> 
  
  <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

  <h1 align="center"> <img src = "https://github.com/Grupo-1-2020-PI-FATEC-ADS/SOS-EDUCA/blob/master/Imagens%20Geral/videosprint3.gif"/></h1>
 
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  
Tive a oportunidade de aprofundar meus conhecimentos em desenvolvimento web, especialmente em relação à criação de um site de comércio eletrônico completo. Isso envolveu o domínio de tecnologias como HTML, CSS e JavaScript, além de frameworks e bibliotecas relevantes para a implementação de recursos de navegação, busca e filtragem. Além disso, tive a chance de trabalhar com bancos de dados, uma vez que o projeto envolvia a gestão e organização de um amplo catálogo de materiais didáticos. Nesse contexto, o aprendizado e a aplicação do MySQL foram fundamentais para entender e implementar a estrutura de dados necessária para armazenar e recuperar as informações relevantes.

Outro aspecto importante foi o foco na usabilidade e experiência do usuário. Ao implementar recursos de busca e filtragem avançados, tive que considerar a facilidade de navegação e o fornecimento de informações relevantes de forma eficiente, contribuindo para a satisfação dos usuários e tornando o site mais atraente. Além disso, o desenvolvimento desse projeto permitiu que eu aprimorasse minhas habilidades de trabalho em equipe, uma vez que a criação de um site de comércio eletrônico envolve diferentes etapas e requer colaboração com os integrantes da equipe.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="270px">Tecnologia/Metodologia</th>
      <th width="85px">Nota</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Ágil Scrum</td>
      <td>★★☆☆☆</td>
	<td>Já ouvi falar</td>
    </tr>
    <tr>
      <td>MySQL</td>
      <td>★★★☆☆</td>
	<td>Entendi</td>
    </tr>	
    <tr>
      <td>HTML</td>
      <td>★★★★☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>★★★★☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>PHP</td>
      <td>★★★☆☆</td>
	<td>Sei fazer com ajuda</td>
    </tr>
   <tr>
      <td>JavaScript</td>
      <td>★★☆☆☆</td>
	<td>Já ouvi falar</td>
    </tr>
    <tr>
      <td>GIT</td>
      <td>★★★☆☆</td>
	<td>Sei fazer com ajuda</td>
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
      <td>Precisei estudar bastante sobre desenvolvimento web.</td>
    </tr>
    <tr>
      <td>Conhecimento</td>
      <td>Precisei aprender a utilizar e aplicar o Scrum no projeto.</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Precisei me comunicar sobre a evolução das minhas tarefas.</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>Precisei organizar a documentação e código no GitHub.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>
 
   <p align="justify" style="font-family:roboto;"><li> 1º Semestre: SOS EDUCA - Site de Vendas de Materiais Didáticos</li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_2.md">2º Semestre: GSW - Dashboard para acompanhamentos dos projetos, através de diferentes fontes de dados.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_3.md">3° Semestre: PromoAll - Ecommerce com um motor de regras para promoções aplicadas no momento da compra.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_4.md">4° Semestre: Subiter - Aplicação Web para sincronização dos dados administrativos, financeiros e operacionais.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_5.md">5º Semestre: Tech Ninjas - Automatização de transferência de arquivos entre nuvens.</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/BryanRibeiro/Portfolio-Projetos/blob/main/API_6.md">6º Semestre: Tech Vision - Sistema de Informação Geográfica de dados públicos do ProAgro.</a></li></p>
  
</body>
</html>