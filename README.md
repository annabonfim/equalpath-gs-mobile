# EqualPath - Aplicativo de Orientação Profissional

## 📱 Sobre o Projeto

EqualPath é um aplicativo mobile desenvolvido em React Native com Expo que ajuda pessoas a descobrirem trilhas de carreira baseadas nas habilidades que elas já possuem e nos seus interesses.

O aplicativo não oferece cursos nem vagas; apenas ajuda o usuário a entender quais trilhas de carreira se alinham melhor com seu perfil atual e quais habilidades precisam ser desenvolvidas.

## 📸 Screenshots

### Tela de Login
![Login Screen](./screenshots/login.png)

### Tela de Cadastro
![SignUp Screen](./screenshots/signup.png)

### Tela Inicial (Home)
![Home Screen](./screenshots/home.png)

### Explorar Trilhas
![Trilhas Screen](./screenshots/trilhas.png)

### Detalhes da Trilha
![Trilha Detalhe Screen](./screenshots/trilha-detalhe.png)

### Minhas Trilhas
![Minhas Trilhas Screen](./screenshots/minhas-trilhas.png)

### Perfil do Usuário
![Perfil Screen](./screenshots/perfil.png)

## 🎯 Funcionalidades

- **Autenticação Completa**: Login e cadastro com persistência local (AsyncStorage)
- **Perfil Personalizado**: Cadastro de habilidades e áreas de interesse
- **Recomendações Inteligentes**: Trilhas recomendadas baseadas no perfil do usuário
- **Exploração de Trilhas**: Visualização de todas as trilhas disponíveis com filtros
- **Detalhes da Trilha**: 
  - Descrição completa
  - Habilidades necessárias (destacando possuídas e faltantes)
  - Cursos recomendados com links
  - Opção de seguir trilha
  - Marcação de trilha como concluída
- **Minhas Trilhas**: Visualização de trilhas seguidas com filtros (todas, em progresso, concluídas)
- **Estatísticas**: Contador de trilhas concluídas e em progresso no perfil
- **Edição de Perfil**: Atualização completa de dados pessoais e profissionais

## 🛠️ Tecnologias Utilizadas

- **React Native** - Framework para desenvolvimento mobile
- **Expo** - Plataforma para desenvolvimento React Native
- **React Navigation** - Navegação entre telas (Stack Navigator e Bottom Tabs)
- **AsyncStorage** - Persistência local de dados
- **Expo Vector Icons** - Biblioteca de ícones (MaterialIcons)
- **React Native Safe Area Context** - Gerenciamento de áreas seguras
- **Dados Mockados** - Dados fictícios para demonstração (não requer backend)

## 📁 Estrutura do Projeto

```
equalpath/
├── src/
│   ├── components/        # Componentes reutilizáveis
│   │   ├── Button.js
│   │   └── Input.js
│   ├── screens/          # Telas do aplicativo
│   │   ├── LoginScreen.js
│   │   ├── SignUpScreen.js
│   │   ├── SignUpProfileScreen.js
│   │   ├── HomeScreen.js
│   │   ├── TrilhasScreen.js
│   │   ├── TrilhaDetalheScreen.js
│   │   ├── MinhasTrilhasScreen.js
│   │   └── PerfilScreen.js
│   ├── navigation/       # Configuração de navegação
│   │   └── MainNavigator.js
│   ├── data/            # Dados mockados
│   │   ├── areasAndSkills.js
│   │   ├── trilhas.js
│   │   └── userData.js
│   ├── services/        # Serviços e lógica de negócio
│   │   └── authService.js
│   ├── utils/           # Utilitários
│   │   └── stringUtils.js
│   └── styles/          # Estilos e tema
│       └── colors.js
├── assets/              # Imagens e recursos
│   └── logo-cameleon.png
├── App.js               # Arquivo principal
└── package.json
```

## 🚀 Como Executar

1. **Instalar dependências:**
```bash
npm install
```

2. **Iniciar o aplicativo:**
```bash
npm start
```

3. **Executar no dispositivo:**
   - Escaneie o QR code com o app Expo Go (iOS) ou Expo Go (Android)
   - Ou pressione `i` para iOS simulator ou `a` para Android emulator

## 📱 Telas do Aplicativo

### 1. LoginScreen
- Campos de e-mail e senha
- Botão para entrar
- Link para criar conta

### 2. RegisterScreen
- Campos: nome, e-mail, senha
- Seleção de área de interesse (modal)
- Adição de habilidades (mínimo 2)
- Botão para criar conta

### 3. HomeScreen (Meu Caminho)
- Resumo do perfil do usuário
- Lista de trilhas recomendadas
- Navegação para detalhes da trilha

### 4. TrilhasScreen
- Lista completa de todas as trilhas disponíveis
- Navegação para detalhes de cada trilha

### 5. TrilhaDetalheScreen
- Descrição da trilha
- Habilidades necessárias com níveis
- Habilidades que o usuário já tem (em verde)
- Habilidades que faltam (em amarelo)
- Cursos recomendados com links externos

### 6. PerfilScreen
- Edição de nome
- Edição de área de interesse
- Edição de habilidades
- Botão para salvar alterações

## 🎨 Tema e Estilização

O aplicativo utiliza um tema consistente com cores definidas em `src/styles/colors.js`:
- **Primary**: Teal (#3DA1A1)
- **Primary Light**: Light Teal (#80CBC4)
- **Secondary**: Cyan (#00ACC1)
- **Background**: Light Gray (#F9FAFB)
- **Surface**: White (#FFFFFF)
- **Text**: Dark Gray (#1F2937)
- **Text Light**: Gray (#6B7280)
- **Border**: Light Gray (#E5E7EB)
- **Error**: Red (#B00020)

## 📝 Notas Importantes

- **Persistência Local**: O aplicativo utiliza AsyncStorage para salvar dados do usuário localmente
- **Dados Mockados**: Trilhas, áreas e habilidades são dados fictícios armazenados em `src/data/`
- **Sem Backend**: Não há integração com API real (conforme requisitos do projeto acadêmico)
- **Navegação**: Utiliza React Navigation com Bottom Tabs (4 abas) e Stack Navigators aninhados
- **Autenticação**: Sistema completo de login/cadastro com validação e proteção de rotas
- **Trilhas Concluídas**: Sistema de marcação de trilhas como concluídas com estatísticas

## 📚 Requisitos Acadêmicos

Este projeto atende aos requisitos da disciplina de Mobile Application Development:
- ✅ Mínimo de 5 telas
- ✅ Navegação entre telas (React Navigation)
- ✅ CRUD mockado (Create, Read, Update, Delete de perfil e trilhas)
- ✅ Estilização com cores, fontes e componentes personalizados
- ✅ Arquitetura organizada com separação de componentes, telas, navegação e dados
- ✅ Projeto funcional e pronto para demonstração

## 👥 Integrantes do Grupo

[Adicione os nomes dos integrantes do grupo aqui]

## 🎥 Vídeo de Demonstração

[Adicione o link do vídeo do YouTube aqui]

## 📄 Descrição da Solução Global Solution

[Adicione a descrição da solução escolhida na Global Solution aqui]

---

Desenvolvido para FIAP - Mobile Application Development



