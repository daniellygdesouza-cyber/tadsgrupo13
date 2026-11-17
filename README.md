## Integrantes do grupo

* Cristiane Ferreira (FênixxTec)
* Danielly Gomes de Souza (
daniellygdesouza-cyber)
* Helvia Monteiro Olmeda (HelviaMonteiro)
* Marinara de Jesus Rosa (marinararosajr)
* Polyanna Michele do Nascimento (polymichele)
* Rodrigo Martins de Almeida (xNumber01)

# 🎬 Cinem@Fã - Quiz de Filmes e Séries

O *Cinem@Fã* é uma aplicação web interativa de perguntas e respostas focada no entretenimento de fãs de series, cinema e televisão. O sistema permite aos utilizadores testarem os seus conhecimentos em diversas franquias famosas, acumularem pontos e competirem num ranking geral.

Este projeto foi desenvolvido como requisito académico pela *Equipe 13* do curso de *TADS 2026 - Centro Universitário SENAC*.

---

### Execução Local 

Para rodar os ficheiros localmente na sua máquina, o projeto não exige instalações complexas:

1. Faça o download deste repositório clicando no botão verde *Code* > *Download ZIP* no topo da página.
2. Extraia o ficheiro ZIP no seu computador.
3. Abra a pasta extraída e dê um duplo clique no ficheiro index.html.
4. A aplicação abrirá diretamente no seu navegador padrão.

---

## 🚀 Funcionalidades

*   *Autenticação de Utilizadores:* Sistema de registo e login utilizando E-mail e Palavra-passe.
*   *Persistência de Dados Local:* Utilização da API localStorage do navegador para guardar perfis de utilizadores, histórico de quizzes concluídos e pontuações, sem necessidade de uma base de dados externa.
*   *Dinâmica de Quizzes:* 
    *   6 categorias de entretenimento disponíveis.
    *   Sorteio dinâmico de 10 perguntas aleatórias a partir de um banco de 30 questões por tema (garantindo que cada jogada seja única).
    *   Bloqueio de repetição: cada utilizador só pode responder a cada tema uma única vez.
*   *Feedback Visual e Imediato:* Barra de progresso interativa, validação de respostas em tempo real (correto/incorreto) e transições suaves de interface (fade-in).
*   *Gamificação:* Tabela de Classificação (Ranking Top 5) atualizada automaticamente com base na pontuação total dos utilizadores.
*   *Conformidade Legal:* Aviso de conformidade com a LGPD (Lei Geral de Proteção de Dados - Lei 13.709/18).

## 📚 Categorias Disponíveis

1.  🌊 Percy Jackson
2.  🟢 Chaves
3.  🎠 Carrossel
4.  🪄 Harry Potter
5.  ⚔️ Demon Slayer
6.  🩺 Grey's Anatomy

---

## 💻 Tecnologias e Padrões Utilizados

O projeto foi construído utilizando as bases do desenvolvimento Web Standards (Front-end):

*   *HTML5:* Semântica e estruturação lógica de componentes.
*   *CSS3:* Estilização responsiva (Mobile-First), utilização de CSS Variables (:root), Flexbox e CSS Grid Layout.
*   *JavaScript (Vanilla JS):* Manipulação de DOM, gestão de estado da aplicação, arrays/objetos, e persistência com localStorage.
*   *Design:* Interface baseada em "Cards" (Modo Escuro / Dark Theme) e tipografia moderna (Google Fonts: Poppins).

-----

## 🛠️ Estrutura do Projeto

```text
📦 cinemafa
 ┣ 📂 css
 ┃ ┗ 📜 style.css       # Estilos globais e responsividade da aplicação
 ┣ 📂 js
 ┃ ┣ 📜 app.js          # Lógica principal, manipulação de DOM e rotas virtuais
 ┃ ┗ 📜 data.js         # Banco de dados estático (Perguntas, Alternativas e Respostas)
 ┣ 📜 index.html        # Estrutura principal da página (Single Page Application)
 ┣ 📜 db.json           # Representação JSON da estrutura de dados da aplicação
 ┗ 📜 README.md         # Documentação do projeto
 }


***********************************************************************************
Documentação



Foco na Jornada-Chave: Em uma Prova de Conceito, o objetivo não é construir toda a infraestrutura definitiva de servidores, mas sim validar a experiência principal do usuário — no caso do Cinem@Fã, o fluxo de jogar o quiz de filmes e séries, registrar respostas e exibir a pontuação ou os parceiros (como CinemaShow e Loja Do Fã).  



&#x20;Validação Rápida: Usar local Storage e arquivos JSON simula o comportamento de um banco de dados (como o Node.js/SQLite planejado para a versão final) sem travar o desenvolvimento com configurações complexas de back-end neste momento. Isso permite colocar o protótipo funcional nas mãos dos usuários rapidamente.   



Coleta de Feedbacks Reais: Como o sistema já roda de forma tangível no navegador, você consegue testar a usabilidade, o layout responsivo e a lógica do quiz para coletar métricas e feedbacks reais antes de escalar o banco de dados.   





\---------------------------------------------------------------------------------------------------------------------------------------------------

###### ***Como defender essa escolha na apresentação:***

###### 

###### ***Se precisar justificar para a banca ou para o professor por que usou local Storage/JSON em vez de um banco relacional agora, basta argumentar que***

###### &#x20;***a arquitetura foi desenhada para validar a jornada principal (MVP/PoC) com baixo acoplamento, garantindo que a camada de dados em JSON possa ser*** 

###### ***facilmente migrada para uma API Node.js + SQLite na próxima fase de evolução do produto, sem precisar refazer a interface.***

**---------------------------------------------------------------------------------------------------------------------------------------------------**



**Banco de Dados (Simulado / Armazenamento Local): O localStorage junto com a estrutura JSON não é um Sistema Gerenciador de Banco de Dados (SGBD)**

&#x20;**tradicional (como SQLite, MySQL ou PostgreSQL), mas funciona como uma camada de persistência de dados no navegador. Na documentação técnica, o termo mais preciso e bem-visto pelos professores é "Persistência de Dados Local (Web Storage API / JSON)" ou "Simulação de Banco de Dados NoSQL em formato JSON".**



**Front-end (Sim): É tudo o que roda diretamente no navegador do usuário — sua estrutura em HTML5, a estilização responsiva em CSS3 e toda a regra de negócio e interatividade do quiz em JavaScript.**



&#x20;**Cinem@Fã — Protótipo Funcional (PoC)**



**> Projeto Integrador — Curso de Análise e Desenvolvimento de Sistemas (ADS) | Equipe 13**



**Sobre esta Entrega (Prova de Conceito)**



**Esta versão representa a \*\*Segunda Etapa: Implantação de Prova de Conceito (PoC)\*\* do Cinem@Fã, uma aplicação web e mobile responsiva de quiz interativo sobre filmes e séries.** 



**O objetivo técnico desta entrega é transformar a ideação em um \*\*produto tangível e funcional\*\*, validando a jornada principal do usuário (seleção de categorias, resposta às perguntas, cálculo de pontuação e exibição de parceiros) para coleta rápida de feedbacks reais antes da escalabilidade da infraestrutura.**



**####################################################################################################################################
PoC - Cris    FênixTech

-> MATERIAL A SER EDITADO.. REEESTRUTURADO E ASSOCIADO AO README JA ADICIONADO <-


**Arquitetura e Tecnologias Utilizadas**

Para viabilizar a construção rápida do protótipo funcional com foco na experiência do usuário, o sistema foi estruturado com arquitetura \*\*Client-Side (Front-end)\*\* e persistência local:**



Front-end (Interface e Lógica):

HTML5: Estruturação semântica das telas e acessibilidade.

CSS3:\*\* Estilização, identidade visual e design responsivo (Mobile-First).

JavaScript (padrão: ES6+) Manipulação do DOM, controle de fluxo do quiz, validação de respostas, temporizador/pontuação e integração com o armazenamento local.(Local Storage)


Persistência de Dados (Simulação de Banco de Dados):

 JSON \& `local Storage` (Web Storage API):\*\* Utilizados para armazenar a base de perguntas, respostas, histórico de pontuações e preferências do usuário diretamente no navegador.** 

Back-end:

 Não aplicável nesta etapa (PoC).
Toda a regra de negócio é executada no lado do cliente (\*client-side\*), eliminando a dependência de servidor para validação inicial da jornada.(Apresentamos aqui apenas um  protótipo)**

Evolução Arquitetural (Próximos Passos)

A camada de dados foi modelada em formato JSON visando o baixo acoplamento. Nas próximas etapas de evolução do produto, o sistema estará preparado para integrar:
1. Back-end: API RESTful desenvolvida em Node.js.**
2. Banco de Dados Relacional:\*\* Migração da persistência local para \*\*SQLite\*\* (ou SGBD equivalente), permitindo ranking global, autenticação de usuários e painel administrativo dinâmico.**

Como Executar o Projeto
Como o projeto não depende de servidor back-end nesta fase:
1. Clone este repositório ou baixe os arquivos.**
2. Abra o arquivo `index.html` diretamente em qualquer navegador moderno (Chrome, Edge, Firefox) ou utilize a extensão \*Live Server\* no VS Code.

Estrutura dos Arquivos:
cinemafa-poc

├── index.html              # Tela inicial (seleção de categorias e aviso LGPD)**

├── quiz.html               # Tela principal do jogo**

├── ranking.html            # Tela de pontuação/resultados e parceiros**

├── README.md               # Documentação técnica do projeto**

├── css/

│   ├── style.css           # Estilos globais e identidade visual**

│   └── responsive.css      # Regras específicas para mobile** 

├── js/

│   ├── app.js              # Lógica principal do quiz e manipulação do DOM**

│   └── storage.js          # Funções de leitura/gravação no local Storage**

├── data/

│   └── perguntas.json      # Base inicial de perguntas de filmes e séries**

└── assets/

├── img/                # Logos do Cinem@Fã, CinemaShow e Loja Do Fã**

└── icons/              # Ícones da interface**


-> MATERIAL A SAER EDITADO
**************************************************************
