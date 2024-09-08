# 📖 Shelfie
Bem vindo a organização Shelfie! Desenvolvida para o Projeto Integrador I do Intituto Federal do Paraná - Campus Foz do Iguaçu. Aqui nesta organização você pode navegador pelos repositórios e commits feitos durante o desenvolvimento do projeto e ver sua evolução! Temos nas abas de repositórios, a camada de Lógica da API (repositório Shelfie-back-end) e a camada de Aplicação Web (repositório Shelfie-front-end). Neste documento, você terá um resumo de como é o projeto com a documentação técnica e passo a passo de como acessar ele de maneira online e também localmente. Conheça nossa equipe!

<div align="center">
 <h2>🤝 Contribuidores</h2>
 <div display="inline-flex">
    <div align="center">
      <a href="https://github.com/gabrielamarqs" title="gabriela marques">
        <img src="https://avatars.githubusercontent.com/u/106118943?v=4" width="150px;" alt="Foto da Gabriela Marques no GitHub"/><br>
        <sub>
          <b>Gabriela Marques</b>
        </sub>
      </a>
     <p>Responsável pelo Back-end</p>
     <img src="https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/gabrielamarqs" />
     <img src="https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriela-marques-dos-santos-899092161/" />
     <img src="https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white" />
    </div>
    <div align="center">
      <a href="https://github.com/mayspiek" title="mayara spieker">
        <img src="https://avatars.githubusercontent.com/u/79992764?v=4" width="150px;" alt="Foto da Mayara Spieker no Github"/><br>
        <sub>
          <b>Mayara Spieker</b>
        </sub>
      </a>
     <p>Responsável pelo Front-end</p>
     <img src="https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/mayspiek" />
     <img src="https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/mayara-spieker/" />
     <img src="https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white" />
    </div>
</div>
</div>

<div align="center">
<h2>⚗️ Tecnologias</h2>
 <table>
  <td align="center">
   <p>Java</p>
   <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" />    
  </td>
  <td align="center">
    <p>Spring Boot</p>
    <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" /> 
  </td>
  <td align="center">
   <p>ReactJs</p>
   <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" /> 
  </td>
  <td align="center">
   <p>TypeScript</p>
    <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" />
  </td>
  <td align="center">
   <p>PostgreSQL</p>
   <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" />
  </td>
 </table>
</div>

### ✏️ Resumo
 <p align="justify">
  Entusiastas de leitura buscam formas de organizar o andamento de suas leituras de forma a manterem contato e engajamento com outras pessoas de interesses semelhantes. Embora existam diversos sistemas com uma ampla gama de funcionalidades, há uma carência de plataformas que oferecem uma visão centralizada e integrada das atividades de leitura. Este artigo apresenta o desenvolvimento do Shelfie, um Sistema de Gerenciamento e Monitoramento de Leituras, desenvolvido da necessidade dos usuários de poderem acompanhar e monitorar suas leituras diárias, a partir das progressões, do estado das leituras e das avaliações. Através de uma arquitetura de três camadas, desenvolvemos uma aplicação web separando a interface, lógica de negócios e dados. Isso facilita a manutenção para futuras melhorias. O Shelfie atingiu seus principais objetivos, que é oferecer uma interface para o usuário poder monitorar e gerenciar suas leituras a partir das funcionalidades implementadas. O projeto proporcionou importantes aprendizados sobre desenvolvimento de software e design centrado no usuário em aplicações Web. 
 </p>

 ## 🔗 Hospedagem
 A aplicação Web do Shelfie está hospedado em um Bucket AWS e está disponível para toda Web utilizar no seguinte link:
<a target="_blank" href="http://shelfiie-bucket.s3-website.us-east-2.amazonaws.com/">Shelfie</a>. Mas você também pode rodar localmente na sua máquina caso preferir. O tópico seguinte tratará sobre como instalar as dependências e como rodar a aplicação diretamente da sua máquina.

 ## 🛠️ Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

- Você instalou a versão mais recente do node e do npm para o front-end e para o back-end o java 17, o tomcat 10 e a última versão do PostgreSQL.
- Você tenha git e vite instalado na sua máquina. 

### 💻 Instalando Shelfie-FrontEnd

Para instalar o Shelfie-FrontEnd, siga estas etapas:

Linux, macOS e Windows:

```
# clone o repositório
git clone https://github.com/shelfiie/Shelfie-front-end.git
# mova para o diretório da aplicação
cd /Shelfie-front-end
# instale as dependências
npm install
```

### 🚀 Rodando o Shelfie-frontEnd
Para rodar a aplicação do Shelfie localmente é simples, basta você rodar o comando:
```
vite
```

### 💻 Instalando Shelfie-BackEnd

Para instalar o Shelfie-BackEnd, siga estas etapas:

Linux, macOS e Windows:

```
# acesse o PostgreSQL como o usuário postgres
sudo -u postgres psql
# crie o usuário do banco de dados
CREATE USER shelfie WITH PASSWORD 'password';
# crie o banco de dados
CREATE DATABASE db_shelfie;
# conceda todas as permissões ao usuário shelfie para modificar o banco de dados criado
GRANT ALL PRIVILEGES ON DATABASE db_shelfie TO shelfie;


# clone o repositório
git clone https://github.com/shelfiie/Shelfie-back-end
# mova para o diretório da aplicação
cd /Shelfie-back-end
# Compile o projeto sem rodar os testes
mvn package -Dmaven.test.skip=true
```

### 🚀 Rodando o Shelfie-backEnd
Para rodar a API do Shelfie localmente é simples, basta você rodar o comando:
```
java -jar target/shelfie-0.0.1-SNAPSHOT.jar
```

E pronto! Sua aplicação deve rodar normalmente.

### 


 
## Requisitos Funcionais
| Código do Requisito | Descrição | Caso de Uso |
| ------ | ------ | ------ |
| RF 01 | O **Sistema** deve permitir que os usuários se registrem no mesmo, com os seguintes dados: identificador único, login (e-mail), senha, nome, nickname. Ao se registrarem, deverão concordar com o Termo de Política e Privacidade do Sistema. <br><br> Há dois tipos de usuários no Sistema, o usuário tipo **Administrador** e o **Usuário** | UC 01 - Gerenciar **Usuário** |
| RF 02 | O sistema deve permitir que o **Usuário** gerencie seu acesso com os seguintes dados: email e senha. Após uma autenticação bem sucedida desse usuário, o sistema gerará um token JWT (Jason Web Token) com validade de expiração. Esse gerenciamento é essencial para garantir a segurança e o controle de acesso adequado dentro do sistema. | UC 02 - Gerenciar Acesso | 
| RF 03 | O **Leitor** deve ser capaz de gerenciar a sua leitura de livros, indicando o estado do livro, se ele já foi lido, está sendo **lido**, foi **abandonado**, está na lista de **próximas leituras**. Essas informações aparecerão na página inicial do usuário, que será sua estante virtual de maneira filtrada por estado. <br><br> O usuário também poderá desassociar esses livros da sua estante virtual, desabilitando o livro e os dados gerados durante a leitura.  | UC 03 - Gerenciar Monitoramento/Acervo de Livros | 
| RF 04 | O **Leitor** deve ser capaz de anotar o progresso da leitura de cada livro. Na progressão da leitura estará presente a última página que ele leu e um comentário do que estava achando da leitura até o momento. <br><br> A quantidade de páginas lidas que vão ser adicionadas ao paginômetro é o número da página colocada no último registro no progresso da leitura feito pelo **Leitor**. | UC 04 - Gerenciar Progresso do Livro |
| RF 05 | O **Leitor** deve ser capaz de postar uma avaliação dos livros lidos e abandonados, colocando sua opinião do livro completo e/ou motivo que o fez abandoná-lo. Essa avaliação terá um comentário e uma nota que vai de 0 a 5. | UC 05 - Gerenciar Review de Livros |
| RF 06 | O **Leitor** deve ser capaz de curtir ou retirar a curtida da Avaliação de outros Leitores. Essas Avaliações curtidas estarão para sua visualização no Painel de Avaliações. | UC 06 - Gerenciar Curtidas das Reviews |
| RF 07 | O **Leitor** deve ser capaz de reportar reviews de outros Leitores que infringem os Termos de Uso do Sistema. E o **Administrador** deve ser capaz de analisar os reportes solicitados pelos Leitores e definir se a review viola ou não os Termos de Uso do Sistema. | UC 07 - Gerenciar Reporte de Reviews |
| RF 08 | O **Leitor** deve ser capaz de adicionar os livros que estão lendo ou que já foram lidos como favoritos. Caso necessário, ele também poderá retirar o livro dos favoritos. | UC 08 - Gerenciar Livros Favoritos |
| RF 09 | O **Leitor** deve ser capaz de enviar solicitação de amizade para outros usuários, sendo que eles podem aceitar, recusar ou deixar pendente. | UC 09 - Gerenciar Amigos | 
| RF 10 | O **Usuário** deve ser capaz de pesquisar os Livros por** Título, Autor, ISBN** e também, sem filtro algum. Se o livro for encontrado, o sistema primeiramente deverá fornecer informações resumidas como **Capa do livro, Autor(es) e Ano de publicação**. Após a escolha do livro, informações detalhadas sobre o mesmo como deverão ser fornecidas **Descrição, Escritor, Editora, Data de publicação e ISBN 10 e 13**.  | UC 10 - Buscar Dados dos Livros | 
| RF 11 | O **Sistema** deve permitir que **Leitor** receba badges pela quantidade de livros lidos.  | UC 11 - Gerenciar Badges do **Usuário** | 

## Diagrama de Casos de Uso Geral
<p>No diagrama de casos de uso geral, podemos ter um parâmetro geral de todas as funcionalidades que o Shelfie tem e qual o Ator que pode realizá-la.</p>
<img height="600em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/30441ff3-a7ef-4b38-94f4-0e2159dc07a1" />

## Modelo Entidade-Relacionamento
<p>No modelo entidade-relacionamento temos uma visão a nível de banco de dados, como as entidades do nosso sistema se relacionam e quais seus atributos!</p>
<img height="600em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/f5e3fe73-ca22-4e49-b2c1-adc662a90f35" />


## Prototipação - Telas Principais 
<p>As prototipações foram feitas antes da implementação do código para agilizar a parte de estilização do sistema uma vez que essa parte já estava planejada. Tiveram algumas mudanças durante o desenvolvimento, mas o Shelfie continua com a cara das autoras!</p>
<img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/95eca277-3367-4dbe-8dc7-268fa0658dd2" /> <img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/b7ab3d50-9bbe-492b-9ec1-0b7b47f26074" /> 
<img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/ee71fe78-6985-4f99-aa8b-7fc468e04b37 " /> <img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/b668974c-d207-4f65-9d7f-b1bb2de17a05" />

<img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/5a847952-b1ae-40d6-8c8d-ac01b13792c1" /> <img height="350em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/74080664-7214-4f02-897d-16dd6ee474f6" />


