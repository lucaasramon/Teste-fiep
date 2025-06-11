# Vaga desenvolvedor Front End

O desafio envolve desenvolver uma aplicação baseando-se em um protótipo no Figma e implementar funcionalidades como: listar todos os produtos, adicionar produtos ao carrinho e criar tela de login com autenticação.  

## Instruções
- Faça um fork desse projeto para sua conta do Github;
- Desenvolva conforme as intruções técnicas;
- Crie um README com intruções de como executar o projeto;
  
## Projeto
Você foi selecionado para participar de um teste técnico para a vaga de Front-End. Sua missão é desenvolver uma aplicação seguindo o [layout](https://www.figma.com/file/HYMUQxxwvGfSHeQMyY6ZKM/Teste-Front-end?type=design&node-id=604%3A431&mode=design&t=TFNLa19Qm8W8AH2J-1) no Figma. 

# Especificações Técnicas

## Tecnologias
- **Framework**: Next.js (versão mais recente recomendada).
- **Estilização**: Tailwind CSS.
- **HTTP Client**: Axios ou `fetch`.
- **Autenticação**: JWT via endpoint da API.

## Requisitos

## 🔌 Endpoints da API
[Link para mais informações da API](https://fakeapi.platzi.com/en/rest/products/)

### Produtos
```http
GET https://api.escuelajs.co/api/v1/products
```

### Autenticação
1. Login para obter token:
```http
POST https://api.escuelajs.co/api/v1/auth/login
Content-Type: application/json

{
  "email": "john@mail.com",
  "password": "changeme"
}
```

2. Perfil do usuário (protegido):
```http
GET https://api.escuelajs.co/api/v1/auth/profile
Authorization: Bearer {token}
```

### Funcionalidades
- Página pública com listagem de produtos
- Sistema de autenticação (login + proteção de rotas)
- Página de perfil do usuário (após login)

  
