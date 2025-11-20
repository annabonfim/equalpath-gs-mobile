# EqualPath - Aplicativo de Orientação Profissional

## 📱 Sobre o Projeto

EqualPath é um aplicativo mobile desenvolvido em React Native com Expo que ajuda pessoas a descobrirem trilhas de carreira baseadas nas habilidades que elas já possuem e nos seus interesses.

O aplicativo não oferece cursos nem vagas; apenas ajuda o usuário a entender quais trilhas de carreira se alinham melhor com seu perfil atual e quais habilidades precisam ser desenvolvidas.

## 🎯 Funcionalidades

- **Login e Registro**: Autenticação básica com e-mail e senha
- **Perfil do Usuário**: Cadastro de habilidades e área de interesse
- **Trilhas de Carreira**: Visualização de diferentes trilhas disponíveis (Dados, Front-end, Customer Success, Suporte Técnico, UX/UI Design)
- **Detalhes da Trilha**: 
  - Descrição da trilha
  - Habilidades necessárias
  - Habilidades que o usuário já possui
  - Habilidades que faltam
  - Cursos recomendados com links externos
- **Edição de Perfil**: Atualização de habilidades e área de interesse

## 🛠️ Tecnologias Utilizadas

- **React Native** - Framework para desenvolvimento mobile
- **Expo** - Plataforma para desenvolvimento React Native
- **React Navigation** - Navegação entre telas (Stack Navigator e Bottom Tabs)
- **Dados Mockados** - Dados fictícios para demonstração (não requer backend)

## 📁 Estrutura do Projeto

```
equalpath/
├── src/
│   ├── components/        # Componentes reutilizáveis
│   │   ├── Button.js
│   │   ├── Input.js
│   │   └── Card.js
│   ├── screens/          # Telas do aplicativo
│   │   ├── LoginScreen.js
│   │   ├── RegisterScreen.js
│   │   ├── HomeScreen.js
│   │   ├── TrilhasScreen.js
│   │   ├── TrilhaDetalheScreen.js
│   │   └── PerfilScreen.js
│   ├── navigation/       # Configuração de navegação
│   │   └── AppNavigator.js
│   ├── data/            # Dados mockados
│   │   └── mockData.js
│   └── styles/          # Estilos e tema
│       ├── theme.js
│       └── globalStyles.js
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

O aplicativo utiliza um tema consistente com cores definidas em `src/styles/theme.js`:
- **Primary**: Indigo (#6366F1)
- **Secondary**: Pink (#EC4899)
- **Background**: Light Gray (#F9FAFB)
- **Surface**: White (#FFFFFF)

## 📝 Notas Importantes

- **Dados Mockados**: O aplicativo utiliza dados fictícios armazenados em `src/data/mockData.js`
- **Sem Backend**: Não há integração com API real (conforme requisitos do projeto acadêmico)
- **Navegação**: Utiliza React Navigation com Stack Navigator para telas de autenticação e Bottom Tabs para telas principais
- **Validações**: Validações básicas de campos obrigatórios e número mínimo de habilidades

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



