
# Desafio React Native - Nível Pleno

## Objetivo

O objetivo deste desafio é avaliar suas habilidades em desenvolvimento de aplicativos móveis com React Native, com Expo. Você deverá criar um aplicativo simples que consome uma API pública, exibe os dados em uma lista, permite a navegação para uma tela de detalhes e possui uma funcionalidade de busca.

## Requisitos

- **Plataforma:** O aplicativo deve ser compatível com Android.
- **Linguagem:** O código principal do aplicativo deve ser escrito em inglês e TypeScript.
- **Framework:** React Native (com Expo).
- **API:** Utilize a API pública [JSONPlaceholder](https://jsonplaceholder.typicode.com/) para obter os dados.

## Funcionalidades

### 1. Tela de Login

- Crie uma tela de login com campos para usuário e senha.
- Utilize a API [DummyJSON](https://dummyjson.com/docs/auth) para autenticar o usuário. A rota de autenticação é `https://dummyjson.com/auth/login`.
- As credenciais do usuário devem ser armazenadas de forma segura no dispositivo (por exemplo, usando AsyncStorage) para que o usuário permaneça logado ao fechar e reabrir o aplicativo junto com a estratégia de refreshtoken quando o token do usuário expirar.
- Adicione uma funcionalidade de logout.

### 2. Tela de Listagem de Posts

- Após o login, a primeira tela deve exibir uma lista de posts.
- Cada item da lista deve exibir o título do post.
- Os dados dos posts devem ser obtidos da rota `/posts` da API do JSONPlaceholder.

### 3. Tela de Detalhes do Post

- Ao tocar em um item da lista, o usuário deve ser redirecionado para uma tela de detalhes do post.
- A tela de detalhes deve exibir o título e o corpo do post.
- Os dados do post podem ser passados da tela de listagem ou obtidos da rota `/posts/:id` da API.

### 4. Funcionalidade de Busca

- Na tela de listagem, adicione um campo de busca para filtrar os posts pelo título.
- A busca deve ser realizada em tempo real, à medida que o usuário digita.

### 5. Navegação

- Utilize uma biblioteca de navegação de sua escolha (por exemplo, React Navigation) para gerenciar a transição entre as telas.

## Estrutura do Projeto

- Organize o código-fonte em uma estrutura clara e coesa. Sugerimos a seguinte estrutura:

```
/app
  /_laiout.tsx
  /index.tsx
  /screens
    /_layout.tsx
    /list.tsx
    /details.tsx
  /services
    /authentication.tsx
```

## Avaliação

Serão avaliados os seguintes pontos:

- **Qualidade do código:** Clareza, organização, manutenibilidade e boas práticas de programação.
- **Componentização:** Reutilização de componentes e separação de responsabilidades.
- **Gerenciamento de estado:** Como o estado do aplicativo é gerenciado (por exemplo, com hooks do React, Redux, etc.).
- **Estilo e UI:** A interface do usuário deve ser limpa, intuitiva e responsiva.
- **Funcionalidade:** O aplicativo deve atender a todos os requisitos funcionais descritos.
- **Commits:** O histórico de commits no Git será analisado.

## Como Entregar

1. Crie um fork deste repositório.
2. Implemente a solução.
3. Faça um pull request para o repositório original.

**Boa sorte!**
