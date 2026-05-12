<html>
<body>
 <h1 align="center"> API 4º Semestre - 01/2025</h1>
<h1 align="center"> 
<a href="https://github.com/CODEPLAY-Fatec/API-ADS-4-Sem-Fatec"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>
</h1>
 
 <h2> Parceiro Acadêmico: <a href="https://fapg.org.br/">FAPG</a></h2>
 
<img src="./Imagens/logofpag.png" height="100" width="230"/>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> O projeto visa resolver o desafio enfrentado pela FAPG relacionado à complexidade e dificuldade no gerenciamento de seus projetos. A solução proposta foi desenvolver um sistema web intuitivo para a gestão integrada de projetos e de suas respectivas atividades, que permitiu a simplificação e a otimização de todo esse processo. Isso foi feito por meio de uma plataforma centralizada onde é possível organizar o fluxo de trabalho, registrar as tarefas e facilitar a visualização clara do andamento de cada etapa. Essa abordagem ofereceu um acompanhamento dinâmico das operações, proporcionando a garantia de eficiência na execução e a total transparência para todos os partícipes envolvidos.
 
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

<!-- Next.js -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg" width="100" height="100" title="Next.js" alt="Next.js" />

<!-- Prisma -->
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/prisma/prisma-original.svg" width="100" height="100" title="Prisma" alt="Prisma" />
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
  <li>
    <a href="https://nextjs.org/">Next.js</a>: É um framework React poderoso e flexível que permite a criação de aplicações web de alto desempenho. Ele oferece recursos nativos como renderização do lado do servidor (SSR), geração de sites estáticos (SSG) e criação simplificada de rotas de API.
  </li>
  <li>
    <a href="https://www.prisma.io/">Prisma</a>: É um ORM (Object-Relational Mapper) moderno para Node.js e TypeScript. Ele facilita o acesso, a modelagem e a migração do banco de dados, permitindo que os desenvolvedores escrevam consultas de forma intuitiva, segura e com forte tipagem.
  </li>
</ul>
<h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end e Front-end</h3>
  <p align="justify" style="font-family:roboto;"> Atuei como desenvolvedor Full-Stack neste projeto, iniciando minhas contribuições pela modelagem do banco de dados para garantir uma estrutura de dados sólida, eficiente e escalável para a aplicação.

 <details>

<summary>Modelagem do banco com Prisma</summary>

<p> Aqui estão algumas funções de autenticação e middleware que eu fiz no backend

```javascript

generator client {
  provider = "prisma-client-js"
}

datasource db {
  provider = "mysql"
  url      = env("DATABASE_URL")
}

model institutions {
  id       Int        @id @default(autoincrement())
  name     String     @unique(map: "name") @db.VarChar(255)
  projects projects[]
}

model projects {
  id              Int              @id @default(autoincrement())
  name            String           @db.Text
  description     String?          @db.Text
  subject         String?          @db.VarChar(255)
  institution     String?          @db.VarChar(255)
  creator         Int
  status          projects_status?
  start           DateTime?        @db.DateTime(0)
  finish          DateTime?        @db.DateTime(0)
  projectMember   projectMember[]
  projectsubjects projectSubjects? @relation(fields: [subject], references: [name], onUpdate: NoAction, map: "projects_ibfk_1")
  institutions    institutions?    @relation(fields: [institution], references: [name], onUpdate: NoAction, map: "projects_ibfk_2")
  users           users            @relation(fields: [creator], references: [id], onDelete: Cascade, onUpdate: NoAction, map: "projects_ibfk_3")
  tasks           tasks[]

  @@index([creator], map: "creator")
  @@index([institution], map: "institution")
  @@index([subject], map: "subject")
}

/// This model or at least one of its fields has comments in the database, and requires an additional setup for migrations: Read more: https://pris.ly/d/database-comments
model tasks {
  id           Int             @id @default(autoincrement())
  projectId    Int
  taskUser     Int?
  title        String          @db.Text
  description  String?         @db.Text
  priority     tasks_priority?
  timeEstimate Int?
  start        DateTime?       @db.DateTime(0)
  finish       DateTime?       @db.DateTime(0)
  createdAt    DateTime        @default(now()) @db.DateTime(0)
  finishedAt   DateTime?       @db.DateTime(0)
  lastUpdated  DateTime?       @db.DateTime(0)
  status       tasks_status
  projects     projects        @relation(fields: [projectId], references: [id], onDelete: Cascade, onUpdate: NoAction, map: "tasks_ibfk_1")
  users        users?          @relation(fields: [taskUser], references: [id], onUpdate: NoAction, map: "tasks_ibfk_2")

  @@index([projectId], map: "projectId")
  @@index([taskUser], map: "taskUser")
}

model users {
  id            Int             @id @default(autoincrement())
  name          String          @db.Text
  email         String          @db.Text
  phoneNumber   String?         @db.Text
  password      String          @db.Text
  projectMember projectMember[]
  projects      projects[]
  tasks         tasks[]
  userPicture   userPicture?
}

model projectMember {
  projectId Int
  userId    Int
  users     users    @relation(fields: [userId], references: [id], onDelete: Cascade, onUpdate: NoAction, map: "projectMember_ibfk_1")
  projects  projects @relation(fields: [projectId], references: [id], onDelete: Cascade, onUpdate: NoAction, map: "projectMember_ibfk_2")

  @@id([projectId, userId])
  @@index([userId], map: "userId")
}

model projectSubjects {
  id       Int        @id @default(autoincrement())
  name     String     @unique(map: "name") @db.VarChar(255)
  projects projects[]
}

model userPicture {
  userId Int   @id
  file   Bytes @db.Blob
  users  users @relation(fields: [userId], references: [id], onDelete: Cascade, onUpdate: NoAction, map: "userPicture_ibfk_1")
}

model PictureDefault {
  id   Int   @id @default(autoincrement())
  file Bytes @db.Blob
}


enum tasks_priority {
  Baixa
  Media @map("Média")
  Alta
}

enum projects_status {
  Fechado
  Em_andamento @map("Em andamento")
  Concluido    @map("Concluído")
}

enum tasks_status {
  Fechado
  Em_andamento @map("Em andamento")
  Concluido    @map("Concluído")
}


```

</details>

No back-end, fui responsável pela implementação do fluxo de cadastro e por estruturar o sistema de autenticação segura utilizando tokens JWT. Além da parte de segurança, também desenvolvi a lógica de negócio e as rotas de API voltadas para a gestão de tarefas e acompanhamento dos projetos.

<details>

<summary>Funções relacionadas as Tarefas</summary>

<p>Segue um exemplo de uma funçao que eu fiz para criar tarefas</p>

```javascript

export const createTaskService = async (
  task: Task,
  projectId: number,
  userId: number,
) => {
  const IsMember = inTheProject(projectId, userId);
  if (!IsMember) {
    throw new Error(
      "Usuário não tem permissão para criar tarefas neste projeto.",
    );
  }
  const projectFinish = await prisma.projects.findFirst({  //essa parte gigante é para fazer as verificaçoes de data
    where: {
      id: projectId,
    },
    select: {
      finish: true,
    }
  });

  const projectStart = await prisma.projects.findFirst({
    where: {
      id: projectId,
    },
    select: {
      start: true,
    }
  });

  const ProjectFinish = new Date(projectFinish?.finish!);
  const TaskStart = new Date(task.start!);
  const TaskFinish = new Date(task.finish!);
  const ProjectStart = new Date(projectStart?.start!);


  if (TaskStart < ProjectStart) {
    throw new Error("Data de início da tarefa não pode ser antes da data de início do projeto.");
  }
  if (TaskFinish < TaskStart) {
    throw new Error("Data de início da tarefa não pode ser depois que a data de fim.");
  }
  if (TaskFinish > ProjectFinish) {
    throw new Error("Data de fim da tarefa não pode ser depois que a data de fim do projeto.");
  }
  if (ProjectFinish < TaskStart) {
    throw new Error("Data de início da tarefa não pode ser maior que a data de fim do projeto.");
  }

  const createTask = prisma.tasks.create({
    data: {
      title: task.title,
      description: task.description || null,
      start: task.start,
      finish: task.finish,
      finishedAt: task.status == "Concluido" ? new Date() : null,
      priority: task.priority,
      status: task.status,
      projectId: projectId,
      timeEstimate: task.timeEstimate || null,
      taskUser: task.taskUser || null,
    },
  });
  return createTask;
};



```

</details>

No front-end, desenvolvi a página de perfil do usuário. Criei um painel centralizado onde o usuário pode visualizar rapidamente informações essenciais sobre os seus projetos e identificar as tarefas mais urgentes. Nesta mesma interface, integrei a funcionalidade de gerenciamento de conta, permitindo que o usuário altere sua senha de forma simples e segura.

<details>

<summary>Meu papel no front-end</summary>

<p>Aqui esta um exemplo de uma pagina Profile que eu fiz</p>

```javascript

"use client";

import { Activities } from "@/created-components/Activities";
import { ChangePassword } from "@/created-components/ChangePassword";
import Navbar from "@/created-components/Navbar";
import { ProfileForm } from "@/created-components/ProfileForm";
import { ProfilePicture } from "@/created-components/ProfilePicture";
import { useEffect, useState } from "react";
import toast from "react-hot-toast";
import axios from "axios";
import { useRouter } from "next/navigation";

type UserProfile = {
  name: string;
  email: string;
  phone: string;
}

export default function UserProfilePage() {
  const router = useRouter();
  const [userData, setUserData] = useState({
    id: 0,
    name: "",
    email: "",
    phone: "",
  });
  const [profilePicture, setProfilePicture] = useState("");
  const [avatarRefreshKey, setAvatarRefreshKey] = useState(0);

  const [isSaving] = useState(false);
  const [isChangingPassword, setIsChangingPassword] = useState(false);

  useEffect(() => {
    const fetchUserData = async () => {
      try {
        const userInfo = await axios.get("/api/me", { withCredentials: true });
        setUserData({
          id: userInfo.data.id,
          name: userInfo.data.name,
          email: userInfo.data.email,
          phone: userInfo.data.phone,
        });

        try {
          const fotoData = await axios.get("/api/foto", { withCredentials: true });
          setProfilePicture(`data:image/png;base64,${fotoData.data.base64}`);
        } catch {
          console.log("No profile picture found, UserAvatar will display initials");
        }
      } catch (error) {
        console.error("Erro ao buscar dados do usuário:", error);
      }
    };

    fetchUserData();
  }, []);

  const updateProfile = async (userData: UserProfile) => {
    try {
      const response = await axios.patch("/api/users", userData, { withCredentials: true });
      if (response.status === 201) {
        toast.success("Perfil atualizado com sucesso!", { duration: 1500 });
      } else {
        toast.error("Erro ao atualizar perfil", { duration: 2000 });
      }
    }
    catch (error) {
      console.error("Erro ao atualizar perfil:", error);
      toast.error("Erro ao atualizar perfil", { duration: 1500 });
    }

  }

  const handlePhotoUpload = async (file: File) => {
    const formData = new FormData();
    formData.append("imagem", file);

    try {
      const response = await fetch("/api/foto", {
        method: "POST",
        body: formData,
      });

      if (!response.ok) throw new Error("Erro ao enviar imagem");

      toast.success("Foto enviada com sucesso!", { duration: 2000 });

      // Refresh profile picture
      try {
        const imagemResponse = await fetch("/api/foto");
        const imagemData = await imagemResponse.json();
        setProfilePicture(`data:image/png;base64,${imagemData.base64}`);

        const newRefreshKey = avatarRefreshKey + 1;
        setAvatarRefreshKey(newRefreshKey);

        localStorage.setItem('avatarRefreshKey', newRefreshKey.toString());
        window.dispatchEvent(new Event('storage'));

      } catch (error) {
        console.error("Erro ao atualizar a foto após upload:", error);
      }
    } catch (error) {
      console.error("Erro ao enviar a foto:", error);
      toast.error("Erro ao enviar a foto", { duration: 2000 });
    }
  };

  return (
    <div className="min-h-screen flex flex-col bg-transparent">
      <Navbar />
      <div className="flex-1 flex items-center justify-center pt-16 px-4 pb-8">
        <div className="w-full max-w-4xl relative">
          <button
            onClick={() => router.push("/projetos")}
            className="absolute left-0 md:left-4 text-3xl text-gray-700 hover:text-gray-900 top-[5px] md:top-[15px]"
          >
            &#60;
          </button>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
            <div className="md:col-span-1 flex flex-col items-center justify-center">
              <ProfilePicture
                profilePicture={profilePicture}
                onPhotoUpload={handlePhotoUpload}
                name={userData.name}
                email={userData.email}
                userId={userData.id}
                refreshKey={avatarRefreshKey}
              />
            </div>
            <div className="md:col-span-2">
              {isChangingPassword ? (
                <ChangePassword onBack={() => setIsChangingPassword(false)} />
              ) : (
                <ProfileForm
                  userData={userData}
                  onChange={(field, value) => setUserData((prev) => ({ ...prev, [field]: value }))}
                  onSave={() => updateProfile(userData)}
                  isSaving={isSaving}
                  onChangePassword={() => setIsChangingPassword(true)}
                />
              )}
            </div>
          </div>

          <Activities />
        </div>
      </div>
    </div>
  );
}

```

</details>

<h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>

Durante o desenvolvimento desse projeto de Sistema Intituitivo para Gestão de Projetos de Pesquisa e Desenvolvimento Tecnológico de uma fundação
para a FAPG, pude adquirir diversos aprendizados significativos que contribuíram para o meu crescimento e desenvolvimento como desenvolvedor.

Este projeto foi uma excelente oportunidade para elevar o meu nível técnico. Na camada de dados, pude aprofundar minha visão sobre modelagem e tive a minha primeira experiência prática utilizando o Prisma ORM para otimizar as consultas ao banco. No front-end, consolidei minha base em React: mergulhei a fundo no gerenciamento de estados, no uso avançado do useEffect e na compreensão real sobre o ciclo de vida dos componentes. Além de todo esse aprendizado novo, a construção do sistema me permitiu fortalecer e aplicar com mais maturidade os conhecimentos que eu já possuía no ecossistema Node.js.

  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="270px">Tecnologia/Metodologia</th>
      <th width="85px">Nota</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Figma</td>
      <td>★★★★★</td>
    <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>React</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
    </tr>	
    <tr>
      <td>Mysql</td>
      <td>★★★★★</td>
    <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>Javascript</td>
      <td>★★★★☆</td>
    <td>Sei fazer com ajuda</td>
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
    <tr>
      <td>NextJS</td>
      <td>★★★☆☆</td>
    <td>Entendi</td>
    </tr>
    <tr>
      <td>Prisma</td>
      <td>★★★★</td>
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
  <td>Responsividade</td>
  <td>Desenvolvi interfaces responsivas, garantindo uma experiência consistente em diferentes dispositivos e tamanhos de tela.</td>
</tr>
   <tr>
  <td>Acessibilidade</td>
  <td>Adotei práticas de desenvolvimento acessível, garantindo que as aplicações sejam utilizáveis por todas as pessoas, independentemente de suas habilidades.</td>
</tr>
<tr>
  <td>Otimização de Desempenho</td>
  <td>Otimizei o desempenho das aplicações, implementando práticas como lazy loading e minimização de recursos.</td>
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
