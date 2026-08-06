# 📖 Projeto de Literatura Clássica

Trabalho de Conclusão de Curso (TCC) do Ensino Técnico Integrado ao Ensino Médio — uma plataforma web dedicada à obra de **Machado de Assis**, reunindo textos, audiobooks e conteúdo biográfico do autor, com sistema de cadastro e login de usuários.

## 🎯 Sobre o projeto

O projeto foi desenvolvido como TCC do curso técnico e tem como objetivo aproximar leitores da literatura clássica brasileira, oferecendo uma experiência de leitura e escuta (audiobooks) das obras de Machado de Assis, além de conteúdo sobre a vida e o contexto do autor.

## ✨ Funcionalidades

- Página inicial com apresentação do projeto e do autor
- Seção "Sobre o Autor" com informações biográficas
- Catálogo de obras e audiobooks/contos do autor
- Cadastro e login de usuários (autenticação com JWT e senhas com hash via bcrypt)
- Painel administrativo para edição de dados do usuário
- Upload de imagens de capa de livro (via Multer)
- Textos complementares sobre o projeto

## 🛠️ Tecnologias

**Frontend**
- HTML5, CSS3 e JavaScript
- Bootstrap 5

**Backend**
- Node.js + Express
- Sequelize (ORM) + MySQL
- JWT (autenticação) e bcryptjs (hash de senhas)
- Multer (upload de imagens)

## 📁 Estrutura do projeto

```
literatura-classica-tcc/
├── index.html                # Página inicial
├── sobreAutor.html           # Sobre o autor
├── audiobooksContos.html     # Catálogo de obras/audiobooks
├── textosProjeto.html        # Textos do projeto
├── login.html / cadastrar.html   # Autenticação de usuários
├── administrador.html        # Painel administrativo
├── js-codigo/                # Scripts do frontend
├── css/                      # Estilos
├── imagens/ imagens2/        # Recursos visuais
└── js/                       # Backend (API, models e conexão com o banco)
    ├── index.js               # Servidor Express e rotas
    ├── banco.js                # Conexão com o banco de dados
    ├── Usuario.js               # Model de usuário
    ├── livros.js                 # Model de livros/obras
    └── imagens.js                 # Model de imagens
```

## 🚀 Como rodar localmente

### Pré-requisitos
- Node.js
- Um banco de dados MySQL

### Passo a passo

```bash
# 1. Clonar o repositório
git clone https://github.com/seu-usuario/literatura-classica-tcc.git
cd literatura-classica-tcc/js

# 2. Instalar as dependências do backend
npm install

# 3. Criar o arquivo .env dentro da pasta js/
DB_NAME=nome_do_banco
DB_USER=usuario_do_banco
DB_PASSWORD=senha_do_banco
DB_HOST=localhost

# 4. Iniciar o servidor
node index.js
```

O backend sobe nas portas `3000` e `3001`. Depois, basta abrir o arquivo `index.html` (fora da pasta `js/`) no navegador para acessar o frontend.


---

*Projeto acadêmico desenvolvido como Trabalho de Conclusão de Curso do Ensino Técnico Integrado ao Ensino Médio.*
