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
<img width="356" height="775" alt="Screenshot 2025-11-20 at 7 38 54 PM" src="https://github.com/user-attachments/assets/d2ea4894-8755-41f8-b8fd-7ad47c8701ea" />

### 2. RegisterScreen
<img width="360" height="779" alt="Screenshot 2025-11-20 at 7 39 04 PM" src="https://github.com/user-attachments/assets/53efa626-52db-4710-bd74-dfd97bed7c5a" />
<img width="357" height="777" alt="Screenshot 2025-11-20 at 7 40 12 PM" src="https://github.com/user-attachments/assets/57787feb-167e-456b-b7d0-db07e5344efa" />

### 3. HomeScreen (Meu Caminho)
<img width="358" height="783" alt="Screenshot 2025-11-20 at 7 41 51 PM" src="https://github.com/user-attachments/assets/74fa21d7-5f70-498d-b231-f6d6631c494a" />

### 4. TrilhasScreen
<img width="357" height="777" alt="Screenshot 2025-11-20 at 7 42 03 PM" src="https://github.com/user-attachments/assets/c530511f-efc0-4c87-8ea0-a40b9f1868e4" />


### 5. TrilhaDetalheScreen
<img width="356" height="773" alt="Screenshot 2025-11-20 at 8 10 39 PM" src="https://github.com/user-attachments/assets/5a3ec139-b0f5-4727-8869-83b904842fcb" />

### 6. PerfilScreen
<img width="368" height="779" alt="Screenshot 2025-11-20 at 7 42 40 PM" src="https://github.com/user-attachments/assets/4d0054b0-1f5f-43b0-913e-d02b7b464610" />


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
- ✅ Estilização com cores, fontes e componentes personalizados
- ✅ Arquitetura organizada com separação de componentes, telas, navegação e dados
- ✅ Projeto funcional e pronto para demonstração

## 👥 Integrantes do Grupo

1. Alane Rocha da Silva — RM561052
2. Anna Beatriz de Araujo Bonfim — RM559561
3. Maria Eduarda Araujo Penas — RM560944

## 🎥 Vídeo de Demonstração

[Adicione o link do vídeo do YouTube aqui]

---

Desenvolvido para FIAP - Mobile Application Development



