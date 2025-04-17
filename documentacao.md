# Documentação para Criação de Página com GitHub Pages

Esta documentação foi elaborada para que qualquer pessoa, mesmo sem conhecimento prévio, consiga criar, configurar e publicar sua própria página utilizando o modelo do projeto [si-unifeb/si-unifeb.github.io](https://github.com/si-unifeb/si-unifeb.github.io). Ela explica o que é o GitHub Pages, quais são os pré-requisitos, como estruturar o repositório, editar os conteúdos e publicar seu site com facilidade. Siga os passos abaixo para obter uma compreensão detalhada de cada etapa.

---

## 1. Visão Geral

**O que é GitHub Pages?**

GitHub Pages é um serviço gratuito do GitHub que permite hospedar sites estáticos diretamente a partir de um repositório. Você pode criar desde páginas pessoais e portfólios até sites institucionais sem necessidade de um servidor próprio. O serviço interpreta arquivos HTML, CSS, JavaScript e Markdown, facilitando a personalização do seu conteúdo.

**Objetivo desta documentação:**  
Orientar o usuário a partir do zero a criar seu próprio site por meio do GitHub Pages, usando como base o projeto “si-unifeb.github.io”. Ao final, você saberá como criar, customizar e publicar seu site.

---

## 2. Pré-Requisitos

Antes de começar, verifique se você possui o seguinte:

- **Conta no GitHub:**  
  Se ainda não tiver, [crie sua conta](https://github.com/join).

- **Conhecimentos básicos de Markdown:**  
  O conteúdo do site é escrito em Markdown (arquivos `.md`), mas não é necessário ser um expert. Para aprender os conceitos básicos, consulte o [Guia Rápido de Markdown](https://www.markdownguide.org/basic-syntax/).


- **Um editor de texto:**  
  Você pode utilizar o editor da interface web do GitHub ou editores de código fonte locais como Visual Studio Code, Sublime Text, etc.

- **Conhecimentos básicos de Git (opcional):**  
  Embora seja possível editar via interface web do GitHub, conhecimentos básicos sobre Git facilitarão o versionamento e as atualizações. Alternativamente, você pode utilizar o [GitHub Desktop](https://desktop.github.com/), um programa que roda em computadores x64 e possui uma interface de fácil entendimento, permitindo utilizar o versionamento sem a necessidade de digitar comandos.


---

## 3. Estrutura do Projeto

O repositório modelo “si-unifeb.github.io” possui uma estrutura simples e organizada, que serve como ponto de partida para a criação do seu site. A seguir, você encontrará uma descrição detalhada dos principais arquivos e pastas:

- **README.md:**  
  Este arquivo contém informações gerais sobre o projeto, orientações iniciais e pode incluir parte desta documentação. Ele é o primeiro contato do usuário com o seu repositório, sendo importante para entender o propósito e as instruções básicas do site.

- **index_pt.md e index_en.md:**  
  São as páginas iniciais do site, respectivamente em português e em inglês.  

- **Pastas temáticas (ex.: `colaboradores`, `discentes`, `docentes`):**  
  Diretórios criados para organizar conteúdos ou seções específicas do site. Cada pasta pode conter arquivos Markdown, imagens ou outros recursos relacionados a um tema específico. Por exemplo:  
  - **colaboradores:** Armazenam informações e perfis sobre os colaboradores do projeto.  
  - **discentes:** Inclui informações referentes aos alunos ou discentes.  
  - **docentes:** Contém informações referentes aos professores ou docentes.
  
  Você pode criar novas pastas, renomeá-las ou reorganizá-las de acordo com a necessidade do seu projeto, garantindo uma navegação mais intuitiva e organizada para os visitantes.

- **Outros arquivos (imagens, etc.):**  
  Embora muitos projetos incluam arquivos CSS ou scripts para personalizar o visual e adicionar funcionalidades dinâmicas, **neste projeto o foco é a utilização de arquivos Markdown para o conteúdo**.  
  No entanto, você pode incluir imagens para enriquecer o conteúdo visual do seu site. Geralmente, as imagens podem ser organizadas em pastas específicas (por exemplo, `imagens/`) e inseridas nos arquivos Markdown usando a sintaxe:
  ```markdown
  ![Descrição da imagem](imagens/sua-imagem.jpg)

Esta organização modular facilita tanto a manutenção quanto a expansão do site. Com uma estrutura bem definida, você pode facilmente localizar e editar os conteúdos específicos de cada seção, além de adicionar novos recursos sem comprometer a organização geral do projeto.


---

## 4. Como Criar sua Própria Página a Partir deste Projeto

Esta seção explica detalhadamente como criar o repositório, clonar para sua máquina local, copiar o conteúdo do projeto modelo, personalizar o site e publicá-lo no GitHub Pages.

### 4.1. Criando um Novo Repositório no GitHub

Para publicar seu site no GitHub Pages, é necessário criar um repositório seguindo o padrão específico. Siga os passos abaixo:

1. **Acesse o GitHub:**  
   - Vá para [https://github.com](https://github.com) e faça login na sua conta.

2. **Inicie a criação de um novo repositório:**  
   - No canto superior direito de qualquer página, clique no ícone **"+"** e selecione **"New repository"**.  
   ![Criar novo repositório no GitHub](https://docs.github.com/assets/images/help/repository/repo-create.png)

3. **Nomeie o repositório corretamente:**  
   - No campo **"Repository name"**, insira o nome no formato:
     ```
     seu-usuario.github.io
     ```
     Substitua `seu-usuario` pelo seu nome de usuário no GitHub. Por exemplo, se seu nome de usuário for `joaocarlos`, o repositório deverá ser `joaocarlos.github.io`.

     > **Importante:** Se o seu nome de usuário contiver letras maiúsculas, converta-as para minúsculas no nome do repositório, conforme recomendado pela [documentação oficial do GitHub Pages](https://docs.github.com/pt/pages/getting-started-with-github-pages/creating-a-github-pages-site).

4. **Adicione uma descrição (opcional):**  
   - No campo **"Description"**, você pode adicionar uma breve descrição sobre o propósito do repositório.

5. **Defina a visibilidade do repositório:**  
   - Selecione **"Public"** para tornar o repositório visível a todos. O GitHub Pages funciona com repositórios públicos.

6. **Inicialize o repositório com um README:**  
   - Marque a opção **"Initialize this repository with a README"** para adicionar um arquivo `README.md` inicial.

7. **Crie o repositório:**  
   - Clique no botão **"Create repository"** para finalizar a criação.

Após esses passos, seu repositório estará pronto e disponível em `https://seu-usuario.github.io`.

---

### 4.1.1. Clonando o Repositório Criado para sua Máquina Local

Para começar a editar e adicionar o conteúdo do projeto modelo, é necessário clonar o repositório que você acabou de criar para o seu computador. Utilize o GitHub Desktop conforme as instruções abaixo:

1. **Abra o GitHub Desktop:**  
   Caso ainda não o possua, baixe e instale o [GitHub Desktop](https://desktop.github.com/).

2. **Clone seu repositório:**  
   - No GitHub Desktop, vá em **File > Clone repository**.
   ![Clonar Repositório](https://docs.github.com/assets/cb-10969/mw-1440/images/help/desktop/clone-file-menu-windows.webp)  
   - Na aba **URL**, insira a URL do seu repositório. Por exemplo, se seu nome de usuário for `seu-usuario`, a URL será:
     ```
     https://github.com/seu-usuario/seu-usuario.github.io
     ```
     ![Inserir a URL](https://docs.github.com/assets/cb-57764/mw-1440/images/help/desktop/clone-a-repository-url-tab-name-input.webp)
   - Escolha uma pasta local onde o repositório será clonado e clique em **Clone**.
   ![Escolher o local](https://docs.github.com/assets/cb-58144/mw-1440/images/help/desktop/clone-choose-button-url-windows.webp)

3. **Verifique o repositório no GitHub Desktop:**  
   - Após a clonagem, seu repositório aparecerá no menu suspenso **"Current Repository"** (canto superior esquerdo do GitHub Desktop).  
   - Caso ele não apareça automaticamente, vá em **File > Add Local Repository...**, clique em **Choose...**, navegue até a pasta onde o repositório foi clonado, selecione-a e clique em **Add Repository**.
   ![Adicionar Repositório Local](https://docs.github.com/assets/cb-10757/mw-1440/images/help/desktop/add-local-repository-windows.webp)
   ![Escolher local](https://docs.github.com/assets/cb-53845/mw-1440/images/help/desktop/add-repo-choose-button-mac.webp)

Essa etapa garante que você tenha uma cópia local do repositório para trabalhar nos arquivos do seu site, podendo sincronizar as alterações com o repositório remoto.

---

### 4.2. Copiando o Conteúdo do Projeto Modelo

Agora que o seu repositório local está configurado, é hora de adicionar o conteúdo do projeto modelo. Existem duas maneiras principais de fazer isso:

#### Opção 1: Usando o GitHub Desktop (Recomendado para Iniciantes)

1. **Clone o repositório modelo:**  
   - Abra o GitHub Desktop.  
   - Vá em **File > Clone repository**.   
   - Na aba **URL**, insira a URL do repositório modelo (por exemplo, `https://github.com/si-unifeb/si-unifeb.github.io`).  
   - Escolha uma pasta local para clonar e clique em **Clone**.  

2. **Copie os arquivos do repositório modelo para o seu repositório local:**  
   - Após o clone, abra a pasta do repositório modelo em seu computador e copie todos os arquivos e pastas.

3. **Abra o seu repositório no GitHub Desktop:**  
   - No GitHub Desktop, clique no menu suspenso **"Current Repository"** no canto superior esquerdo e selecione o seu repositório (aquele que você clonou anteriormente, ou seja, o seu repositório recém-criado).  
   - Se o repositório não estiver listado, utilize **File > Add Local Repository...** para adicioná-lo (veja a seção anterior).

4. **Cole os arquivos copiados:**  
   - No explorador de arquivos do seu sistema, cole os arquivos copiados do repositório modelo na pasta do seu repositório local.

5. **Confirme e envie as alterações:**  
   - No GitHub Desktop, as alterações serão listadas.  
   - Adicione uma mensagem de commit (por exemplo, "Adicionando conteúdo do projeto modelo") e clique em **Commit to main**.  
   - Clique em **Push origin** para enviar as alterações para o repositório remoto.

#### Opção 2: Usando a Interface Web do GitHub

1. **Acesse o repositório modelo:**  
   - Vá para o repositório modelo no GitHub (por exemplo, `https://github.com/si-unifeb/si-unifeb.github.io`).

2. **Baixe o conteúdo:**  
   - Clique no botão **Code** e depois em **Download ZIP**.
   ![Dowload ZIP](https://sites.northwestern.edu/researchcomputing/files/2021/05/github.png)  
   - Extraia o conteúdo do arquivo ZIP em seu computador.

3. **Acesse seu repositório:**  
   - Entre no seu repositório recém-criado no GitHub.

4. **Adicione os arquivos:**  
   - Clique em **Add file > Upload files**.
   ![Adicionar Arquivos](https://docs.github.com/assets/cb-54037/mw-1440/images/help/repository/upload-files-button.webp)  
   - Arraste e solte os arquivos extraídos ou clique em **choose your files** para selecioná-los.  
   - Após adicionar os arquivos, clique em **Commit changes** para finalizar.

> **Nota:** Se o seu repositório já possuir um arquivo `README.md` criado automaticamente, você pode optar por substituí-lo ou mantê-lo, conforme sua preferência.

---
## 📚 Documentação de Implementação Detalhada
Para ver como cada página e componente foi construído, acesse:
➡️ [docs/detalhamento.md](docs/detalhamento.md)

