# HelpHairProject

HelpHairProject é uma aplicação completa voltada para gerenciamento de informações relacionadas à saúde capilar, abrangendo três plataformas: web, desktop e mobile. O projeto é desenvolvido utilizando **Python** para o backend e **Vue.js** no frontend, sendo projetado para ser hospedado no **Heroku**.

## Tecnologias Utilizadas

### Backend (API)
- **Linguagem**: Python
- **Frameworks**: Flask ou FastAPI
- **Banco de Dados**: PostgreSQL (Hospedado no Heroku)
- **ORM**: SQLAlchemy (ou Django ORM se usar Django)
- **Testes**: Pytest

### Frontend
- **Web**: Vue.js (SPA)
- **Mobile**: Quasar Framework (Vue.js) para Android/iOS
- **Desktop**: Electron + Vue.js

### Hospedagem
- **Backend**: Heroku
- **Frontend Web**: Heroku ou Netlify (opcional)
- **Mobile**: Compilado para Android/iOS usando Capacitor/Cordova
- **Desktop**: Empacotado com Electron para Windows, macOS e Linux

## Estrutura do Projeto

```bash
HelpHairProject/
│
├── api/                    # Diretório para a API (Python)
│   ├── app/                # Aplicação principal
│   │   ├── __init__.py     # Inicialização do módulo
│   │   ├── main.py         # Ponto de entrada da aplicação
│   │   ├── models.py       # Modelos de dados (ORM, se usado)
│   │   ├── routes.py       # Definição de rotas/endpoints
│   │   ├── config.py       # Configurações (DB, autenticação, etc.)
│   │   ├── utils.py        # Funções utilitárias
│   │   └── requirements.txt # Dependências do projeto
│   │
│   └── tests/              # Testes para a API
│       ├── __init__.py     # Inicialização do módulo de testes
│       ├── test_routes.py  # Testes das rotas
│       └── test_models.py  # Testes dos modelos
│
├── web/                    # Diretório para o site institucional
│   ├── public/             # Arquivos estáticos (HTML, CSS, JS)
│   │   ├── index.html      # Página principal
│   │   └── images/         # Imagens estáticas
│   └── src/                # Código Vue.js (SPA)
│       ├── components/     # Componentes Vue.js
│       │   └── Header.vue  # Exemplo de componente
│       ├── pages/          # Páginas principais
│       │   └── HomePage.vue# Exemplo de página
│       ├── App.vue         # Componente principal Vue.js
│       └── main.js         # Ponto de entrada do Vue.js
│
├── webapp/                 # Diretório para o aplicativo web Vue.js
│   ├── public/             # Arquivos estáticos (ícones, HTML)
│   └── src/                # Código-fonte Vue.js para o app web
│       ├── components/     # Componentes do front-end
│       │   └── Header.vue  # Exemplo de componente
│       ├── pages/          # Páginas principais
│       │   └── HomePage.vue# Exemplo de página
│       ├── App.vue         # Componente principal
│       └── main.js         # Ponto de entrada
│   └── package.json        # Dependências do projeto Vue.js
│
├── desktop/                # Diretório para a plataforma desktop
│   ├── main.js             # Ponto de entrada do Electron
│   ├── src/                # Código Vue.js para a versão desktop
│   │   ├── components/     # Componentes Vue.js
│   │   └── main_window.vue # Janela principal
│   ├── electron.js         # Configuração do Electron
│   └── package.json        # Dependências do projeto Electron/Vue.js
│
└── mobile/                 # Diretório para o aplicativo mobile
    ├── src/                # Código Quasar Framework
    │   ├── components/     # Componentes Vue.js
    │   ├── pages/          # Páginas principais do aplicativo mobile
    │   ├── App.vue         # Componente principal Vue.js
    │   └── main.js         # Ponto de entrada
    └── quasar.conf.js      # Configuração do Quasar Framework
