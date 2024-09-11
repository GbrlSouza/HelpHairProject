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
├── api/                    # Backend (API em Python)
│   ├── app/                # Lógica da aplicação e rotas
│   └── tests/              # Testes unitários
│
├── web/                    # Site institucional (Vue.js)
├── webapp/                 # Aplicação Web (Vue.js)
├── desktop/                # Aplicação Desktop (Electron + Vue.js)
└── mobile/                 # Aplicativo Mobile (Quasar Framework)
