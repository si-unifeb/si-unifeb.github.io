# Detalhamento da Implementação para Iniciantes

Este documento mostra, passo a passo, como cada arquivo Markdown do projeto **si-unifeb.github.io** está estruturado e organizado. Aqui você vai entender como usamos **badges do Shields.io** para navegação, a disposição dos arquivos e pastas, e os elementos de rodapé — tudo em Markdown simples, sem templates personalizados.

> **Importante:** Se você só precisa criar, clonar e publicar seu site, consulte o **documentação.md**. Este guia detalha cada página e componente.

---

## Sumário

1. [Formato das Páginas](#formato-das-paginas)
2. [Uso de Badges do Shields.io](#uso-de-badges-do-shieldsio)
3. [Estrutura de Navegação](#estrutura-de-navegacao)
4. [Organização de Pastas e Páginas Temáticas](#organizacao-de-pastas-e-paginas-tematicas)
5. [Descrição Detalhada de Cada Página](#descricao-detalhada-de-cada-pagina)
6. [Como Criar Novas Páginas](#como-criar-novas-paginas)

---

## 1. Formato das Páginas

- **Arquivos Markdown**: cada página é um arquivo `.md` que começa com badges para navegação e um título principal (`# Título`).
- **Cabeçalhos**: use `#` para título, `##` para seções e `###` para subseções.
- **Imagens e links**: insira badges com:
  ```markdown
  [![Texto Alternativo](URL-da-badge)](URL-de-destino)
  ```

---

## 2. Uso de Badges do Shields.io

- **Shields.io** é uma plataforma digital que gera imagens personalizadas via URL.

### 2.1. Badge Estática Básica
- **Exemplo de Badge Estática**:
  ```
  https://img.shields.io/static/v1?label=&message=MENU&color=%23009BD5&style=for-the-badge
  ```
- **Parâmetros**:
  - `label`: texto à esquerda (pode ficar vazio).
  - `message`: texto principal.
  - `color`: cor de fundo (hex com `%23`).
  - `style`: estilo (`for-the-badge`, `flat`).
- **Markdown**:
  ```markdown
  [![MENU](https://img.shields.io/static/v1?label=&message=MENU&color=%23009BD5&style=for-the-badge)](/menu.md)
  ```
  - **Exibição:**
    
    [![MENU](https://img.shields.io/static/v1?label=&message=MENU&color=%23009BD5&style=for-the-badge)]()

### 2.2. Badge com ícone (logo)

- Você também pode criar badges com ícones de plataformas como Instagram, GitHub, LinkedIn, e-mail, entre outros. Isso é possível usando os parâmetros ```logo``` e ```logoColor```.

- Exemplo de Badge com ícone:
  ```markdown
  [![Instagram](https://img.shields.io/badge/Instagram-8A2BE2?logo=instagram&logoColor=white&style=for-the-badge)](https://instagram.com)
  ```
  - **Exibição:**

    [![Instagram](https://img.shields.io/badge/Instagram-8A2BE2?logo=instagram&logoColor=white&style=for-the-badge)]()

- **Explicando os parâmetros usados:**

  - ```Badge text``` (antes do ```?```) : define o texto da badge. Neste caso: ```Instagram```.

  - ```color``` : cor de fundo em hexadecimal. No exemplo acima ```8A2BE2``` - **Roxo Escuro.**

  - ```logo``` : nome do ícone (nesse caso ```instagram```).

  - ```logoColor``` : cor do ícone (geralmente ```white``` para contraste).

  - ```style``` : mesmo que nos outros exemplos.

    > **Importante:** Para descobrir quais logos estão disponíveis no Shields.io, consulte a biblioteca de ícones utilizada pela plataforma, disponível no GitHub na pasta ```icons``` . Confira [aqui](https://github.com/simple-icons/simple-icons)

---

## 3. Estrutura de Navegação

Em todas as páginas, temos badges no topo que linkam para:

| Seção                 | Arquivo                              |
|-----------------------|--------------------------------------|
| Página Inicial PT               | `index.md`                        |
| Página Inicial EN               | `indexen.md`                        |
| Docentes PT           | `docentes/docentes_pt.md`            |
| Docentes EN           | `docentes/docentes_en.md`            |
| Discentes PT          | `discentes/discentes_pt.md`          |
| Discentes EN          | `discentes/discentes_en.md`          |
| Colaboradores PT      | `colaboradores/inicial.md`           |
| Colaboradores EN      | `collaborators/initial.md`           |
| Colaboradores 2025 PT         | `colaboradores/2025/colaboradores.md`|
| Colaboradores 2025 EN         | `collaborators/2025/collaborators.md`|

---

## 4. Organização de Pastas e Páginas Temáticas

```text
/ (raiz)
├── index.md
├── indexen.md
├── docentes/
│   ├── docentes_pt.md
│   └── docentes_en.md
├── discentes/
│   ├── discentes_pt.md
│   └── discentes_en.md
├── colaboradores/
│   ├── inicial.md
│   └── 2025/
│       └── colaboradores.md
├── collaborators/
│   ├── initial.md
│   └── 2025/
│       └── collaborators.md
├── README.md
└── docs/
    ├── detalhamento_implementacao.md
    └── guia_publicacao.md

```

---

## 5. Descrição Detalhada de Cada Página

### 5.1. `index.md`
- **Propósito**: Página inicial em Português.
- **Badge no topo**: Link para a página em Inglês.
  ```markdown
  [![ESTA PÁGINA EM INGLÊS](https://img.shields.io/static/v1?label=&message=ESTA+P%C3%81GINA+EM+INGL%C3%8AS&color=%23009BD5&style=for-the-badge)](/indexen.md)
  ```
  - **Exibição:**

    [![ESTA PÁGINA EM INGLÊS](https://img.shields.io/static/v1?label=&message=ESTA+P%C3%81GINA+EM+INGL%C3%8AS&color=%23009BD5&style=for-the-badge)]()

- **Título**: `# Sobre` com Badges que redirecionam para os seguintes meios de contato: Curso de Sistemas de Informação(SI) da Unifeb, Whatsapp da Unifeb e Instagram de SI.
  ```markdown
  [![Sistemas de Informação UNIFEB](https://img.shields.io/badge/Sistemas%20de%20Informa%C3%A7%C3%A3o_UNIFEB-302683?logo=htmlacademy)](https://vestibular.unifeb.edu.br/curso.php?id=28) [![Contato UNIFEB](https://img.shields.io/badge/Contato_UNIFEB-25D366?logo=whatsapp&logoColor=white)](https://wa.me/551733216411) [![Instagram Sistemas de Informação UNIFEB](https://img.shields.io/badge/Instagram_Sistemas_de_Informação_UNIFEB-8A2BE2?logo=instagram)](https://www.instagram.com/siunifeb/)
  ```

  - **Exibição:**

    [![Sistemas de Informação UNIFEB](https://img.shields.io/badge/Sistemas%20de%20Informa%C3%A7%C3%A3o_UNIFEB-302683?logo=htmlacademy)]() [![Contato UNIFEB](https://img.shields.io/badge/Contato_UNIFEB-25D366?logo=whatsapp&logoColor=white)]() [![Instagram Sistemas de Informação UNIFEB](https://img.shields.io/badge/Instagram_Sistemas_de_Informação_UNIFEB-8A2BE2?logo=instagram)]()

- **Menu:** Badges com links para subseções: Docentes, Discentes.
  ```markdown
  [![DOCENTES](https://img.shields.io/static/v1?label=&message=DOCENTES&color=%23009BD5&style=for-the-badge)](/docentes/docentes_pt.md) 

  [![DISCENTES](https://img.shields.io/static/v1?label=&message=DISCENTES&color=%23009BD5&style=for-the-badge)](/discentes/discentes_pt.md)
  ```
  - **Exibição:**

    [![DOCENTES](https://img.shields.io/static/v1?label=&message=DOCENTES&color=%23009BD5&style=for-the-badge)]() 

    [![DISCENTES](https://img.shields.io/static/v1?label=&message=DISCENTES&color=%23009BD5&style=for-the-badge)]()

- **Código Fonte:** Badges que redirecionam para o repositório do projeto no GitHub, mostram a quantidade de estrelas e de forks.
  ```markdown
  [![CyberChase - si-unifeb.github.io](https://img.shields.io/static/v1?label=CyberChase&message=si-unifeb.github.io&color=black&logo=github)](https://github.com/si-unifeb/si-unifeb.github.io "Ir para o Repositório") [![stars - si-unifeb.github.io](https://img.shields.io/github/stars/si-unifeb/si-unifeb.github.io?style=social)](https://github.com/si-unifeb/si-unifeb.github.io) [![forks - unifeb.github.io](https://img.shields.io/github/forks/si-unifeb/si-unifeb.github.io?style=social)](https://github.com/si-unifeb/si-unifeb.github.io)
  ```
  - **Exibição:**

    [![CyberChase - si-unifeb.github.io](https://img.shields.io/static/v1?label=CyberChase&message=si-unifeb.github.io&color=black&logo=github)]() [![stars - si-unifeb.github.io](https://img.shields.io/github/stars/si-unifeb/si-unifeb.github.io?style=social)]() [![forks - unifeb.github.io](https://img.shields.io/github/forks/si-unifeb/si-unifeb.github.io?style=social)]()   

- **Alunos Colaboradores:** Link para a página inicial de colaboradores.
  ```markdown
  [![COLABORADORES](https://img.shields.io/static/v1?label=&message=COLABORADORES&color=%23009BD5&style=for-the-badge)](/colaboradores/inicial.md)
  ```
  - **Exibição:**

    [![COLABORADORES](https://img.shields.io/static/v1?label=&message=COLABORADORES&color=%23009BD5&style=for-the-badge)]()

- **Orientador:** Badges com link para o perfil no GitHub e indicação do número de seguidores.
  ```markdown
  [![Miguel dos Santos Martins](https://img.shields.io/badge/Miguel%20dos%20Santos%20Martins-302683?&color=gray&logo=github)](https://github.com/omiguelsma "Ir para o perfil GitHub") [![Seguidores](https://img.shields.io/github/followers/omiguelsma)](https://github.com/omiguelsma)
  ``` 
  - **Exibição:**

    [![Miguel dos Santos Martins](https://img.shields.io/badge/Miguel%20dos%20Santos%20Martins-302683?&color=gray&logo=github)]() [![Seguidores](https://img.shields.io/github/followers/omiguelsma)]()

- **Template Web**: Badge para o link do Template usado para a criação desse projeto.
  ```markdown
  [![omiguelsma - omiguelsma.github.io](https://img.shields.io/static/v1?label=omiguelsma&message=omiguelsma.github.io&color=blue&logo=github)](https://github.com/omiguelsma/omiguelsma.github.io)
  ```
  - **Exibição:**

    [![omiguelsma - omiguelsma.github.io](https://img.shields.io/static/v1?label=omiguelsma&message=omiguelsma.github.io&color=blue&logo=github)](https://github.com/omiguelsma/omiguelsma.github.io)

### 5.2. `index_en.md`
- **Propósito**: Página inicial em Inglês.
- **Badge no topo**: Link para a página em Português
  ```markdown
  [![THIS PAGE IN PORTUGUESE](https://img.shields.io/static/v1?label=&message=THIS+PAGE+IN+PORTUGUESE&color=%23009BD5&style=for-the-badge)](/index.md)
  ```
  - **Exibição:**

    [![THIS PAGE IN PORTUGUESE](https://img.shields.io/static/v1?label=&message=THIS+PAGE+IN+PORTUGUESE&color=%23009BD5&style=for-the-badge)]()


- **Título**: `# About` com o mesmo conteúdo que a página em português, porém com o texto em inglês.
  ```markdown
  [![Information Systems UNIFEB](https://img.shields.io/badge/Information%20Systems_UNIFEB-302683?logo=htmlacademy)](https://vestibular.unifeb.edu.br/curso.php?id=28) [![UNIFEB Contact](https://img.shields.io/badge/UNIFEB_Contact-25D366?logo=whatsapp&logoColor=white)](https://wa.me/551733216411) [![Instagram Information Systems UNIFEB](https://img.shields.io/badge/Instagram_Information_Systems_UNIFEB-8A2BE2?logo=instagram)](https://www.instagram.com/siunifeb/)
  ```
  - **Exibição:**

    [![Information Systems UNIFEB](https://img.shields.io/badge/Information%20Systems_UNIFEB-302683?logo=htmlacademy)]() [![UNIFEB Contact](https://img.shields.io/badge/UNIFEB_Contact-25D366?logo=whatsapp&logoColor=white)]() [![Instagram Information Systems UNIFEB](https://img.shields.io/badge/Instagram_Information_Systems_UNIFEB-8A2BE2?logo=instagram)]()


- **Menu**: Botões que redirecionam para os ``Faculty`` (Docentes) e ``Studentes`` (Discentes) respectivamente.
  ```markdown
  [![FACULTY](https://img.shields.io/static/v1?label=&message=FACULTY&color=%23009BD5&style=for-the-badge)](/docentes/docentes_en.md) 

  [![STUDENTS](https://img.shields.io/static/v1?label=&message=STUDENTS&color=%23009BD5&style=for-the-badge)](/discentes/discentes_en.md)
  ```
  - **Exibição:**
    
    [![FACULTY](https://img.shields.io/static/v1?label=&message=FACULTY&color=%23009BD5&style=for-the-badge)]() 

    [![STUDENTS](https://img.shields.io/static/v1?label=&message=STUDENTS&color=%23009BD5&style=for-the-badge)]()

- **Source Code:** Badges que redirecionam para o repositório do projeto no GitHub, mostram a quantidade de estrelas e de forks.
  ```markdown
  [![CyberChase - si-unifeb.github.io](https://img.shields.io/static/v1?label=CyberChase&message=si-unifeb.github.io&color=black&logo=github)](https://github.com/si-unifeb/si-unifeb.github.io "Go to Repository") [![stars - si-unifeb.github.io](https://img.shields.io/github/stars/si-unifeb/si-unifeb.github.io?style=social)](https://github.com/si-unifeb/si-unifeb.github.io) [![forks - unifeb.github.io](https://img.shields.io/github/forks/si-unifeb/si-unifeb.github.io?style=social)](https://github.com/si-unifeb/si-unifeb.github.io)
  ```
  - **Exibição:**

    [![CyberChase - si-unifeb.github.io](https://img.shields.io/static/v1?label=CyberChase&message=si-unifeb.github.io&color=black&logo=github)]() [![stars - si-unifeb.github.io](https://img.shields.io/github/stars/si-unifeb/si-unifeb.github.io?style=social)]() [![forks - unifeb.github.io](https://img.shields.io/github/forks/si-unifeb/si-unifeb.github.io?style=social)]()    
  
- **Collaborators:** Link para a página inicial de collaborators
  ```markdown
  [![COLLABORATORS](https://img.shields.io/static/v1?label=&message=COLLABORATORS&color=%23009BD5&style=for-the-badge)](/collaborators/initial.md)
  ```
  - **Exibição:**
    
    [![COLLABORATORS](https://img.shields.io/static/v1?label=&message=COLLABORATORS&color=%23009BD5&style=for-the-badge)]()

- **Advisor:** Badges com link para o perfil no GitHub e indicação do número de seguidores.
  ```markdown
  [![Miguel dos Santos Martins](https://img.shields.io/badge/Miguel%20dos%20Santos%20Martins-302683?&color=gray&logo=github)](https://github.com/omiguelsma "Go to GitHub Profile") [![Followers](https://img.shields.io/github/followers/omiguelsma)](https://github.com/omiguelsma)
  ```
  - **Exibição:**

    [![Miguel dos Santos Martins](https://img.shields.io/badge/Miguel%20dos%20Santos%20Martins-302683?&color=gray&logo=github)]() [![Followers](https://img.shields.io/github/followers/omiguelsma)]()

- **Web Template:** Badge para o link do Template usado para a criação desse projeto.
  ```markdown
  [![omiguelsma - omiguelsma.github.io](https://img.shields.io/static/v1?label=omiguelsma&message=omiguelsma.github.io&color=blue&logo=github)](https://github.com/omiguelsma/omiguelsma.github.io)
  ```
  - **Exibição:**
    
    [![omiguelsma - omiguelsma.github.io](https://img.shields.io/static/v1?label=omiguelsma&message=omiguelsma.github.io&color=blue&logo=github)]()

### 5.3. `docentes/` e `discentes/`



### 5.4. `colaboradores/inicial.md` e `collaborators/initial.md`



---

## 6. Como Criar Novas Páginas

1. Crie o arquivo `.md` na pasta apropriada.
2. Copie o padrão de badges do topo de arquivos similares.
3. Defina o título (`#`) e escreva o conteúdo.
4. Commit & push: o GitHub Pages renderiza automaticamente.

---


