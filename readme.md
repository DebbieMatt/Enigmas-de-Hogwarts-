# Code And Riddle Acronyms

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![React](https://img.shields.io/badge/React-18+-61DAFB?logo=react&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)
![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)

Jogo educativo de decodificação de siglas baseado no universo Harry Potter, desenvolvido com React e Tailwind CSS.

## 📚 Documentação Completa

Para informações detalhadas sobre o jogo, mecânicas, regras e estratégias, consulte a **[Wiki do Projeto](../../wiki)**.

## 🚀 Demo

**[🎮 Jogar Agora](https://seu-usuario.github.io/code-and-riddle-acronyms/)**

## 🛠️ Stack Tecnológica

### Frontend
- **React** 18.2.0 - Biblioteca JavaScript para construção de interfaces
- **Tailwind CSS** 3.4.0 - Framework CSS utilitário
- **Lucide React** 0.263.1 - Biblioteca de ícones

### Ferramentas de Desenvolvimento
- **Node.js** ≥ 16.x
- **npm** ≥ 8.x

### Estrutura
```
src/
├── components/
│   └── CodeAndRiddleAcronyms.jsx  # Componente principal do jogo
├── data/
│   └── levels.js                  # Configuração dos 10 níveis
├── utils/
│   ├── validation.js              # Lógica de validação de respostas
│   └── scoring.js                 # Sistema de pontuação
└── styles/
    └── animations.css             # Animações customizadas
```

## 📋 Pré-requisitos

- Node.js (versão 16 ou superior)
- npm ou yarn
- Navegador moderno com suporte a ES6+

## 🔧 Instalação

### Clonar o Repositório
```bash
git clone https://github.com/seu-usuario/code-and-riddle-acronyms.git
cd code-and-riddle-acronyms
```

### Instalar Dependências
```bash
npm install
```

### Executar em Desenvolvimento
```bash
npm start
```
O aplicativo estará disponível em `http://localhost:3000`

### Build para Produção
```bash
npm run build
```
Os arquivos otimizados estarão na pasta `build/`

## 🏗️ Arquitetura do Código

### Componente Principal
```javascript
CodeAndRiddleAcronyms
├── Estado do Jogo (useState)
│   ├── currentLevel
│   ├── score
│   ├── attempts
│   └── gameState (started/playing/complete)
│
├── Lógica de Validação
│   ├── normalizeAnswer()
│   └── checkAnswer()
│
└── Renderização Condicional
    ├── IntroScreen
    ├── GameScreen
    └── CompletionScreen
```

### Sistema de Níveis
```javascript
levels = [
  {
    id: number,
    difficulty: string,
    title: string,
    description: string,
    question: string,
    answers: string[],
    hint: string,
    points: number,
    type: string
  }
]
```

### Validação de Respostas
O sistema implementa normalização inteligente:
- Remoção de acentuação (NFD)
- Conversão para lowercase
- Remoção de pontuação
- Normalização de espaços
- Suporte a múltiplas variações de resposta

## 📊 Versionamento

Este projeto segue [Semantic Versioning](https://semver.org/).

### Histórico de Versões

- **v2.0.0** (2025-11-11) - Versão React completa com 10 níveis
  - Migração para React
  - Sistema de dificuldade progressiva
  - Interface moderna com Tailwind CSS
  - Sistema de validação aprimorado

- **v1.0.0** (2022-10-12) - Versão original HTML/CSS/JS
  - Conceito inicial por Debbie Matt
  - 5 níveis básicos
  - Interface temática Harry Potter

## 👥 Autores

### Conceito Original
**Debbie Matt** - Criadora do jogo "Jogo de Enigma e Codificação" (2022)

### Desenvolvimento Moderno
**Debbie Matt** - Implementação React e expansão para 10 níveis (2025)
- GitHub: [@DebbieMatt](https://github.com/DebbieMatt)
- LinkedIn: [Débora Mateus Camargo](https://www.linkedin.com/in/d%C3%A9bora-mateus-camargo-a21031190)

## 🤝 Como Contribuir

Contribuições são bem-vindas! Siga os passos abaixo:

### 1. Fork do Projeto
```bash
# Clique no botão "Fork" no GitHub
```

### 2. Crie uma Branch
```bash
git checkout -b feature/nova-funcionalidade
```

### 3. Faça suas Alterações
- Siga o padrão de código existente
- Comente código complexo
- Teste todas as funcionalidades

### 4. Commit
```bash
git commit -m "feat: adiciona nova funcionalidade X"
```

**Padrões de Commit:**
- `feat:` Nova funcionalidade
- `fix:` Correção de bug
- `docs:` Documentação
- `style:` Formatação de código
- `refactor:` Refatoração
- `test:` Testes
- `chore:` Tarefas de manutenção

### 5. Push
```bash
git push origin feature/nova-funcionalidade
```

### 6. Abra um Pull Request
- Descreva suas mudanças detalhadamente
- Referencie issues relacionadas
- Aguarde revisão

## 🐛 Reportar Bugs

Encontrou um bug? [Abra uma issue](../../issues/new) com:

1. **Título claro** descrevendo o problema
2. **Passos para reproduzir** o erro
3. **Comportamento esperado** vs **comportamento atual**
4. **Screenshots** (se aplicável)
5. **Ambiente**: Navegador, versão, SO

## 💡 Sugerir Melhorias

Tem uma ideia? [Abra uma issue](../../issues/new) com a tag `enhancement`:

- Descreva a funcionalidade proposta
- Explique o caso de uso
- Sugira implementação (opcional)

## 📝 Propósito do Desenvolvedor

### Objetivos do Projeto

1. **Educacional**
   - Ensinar conceitos de decodificação e lógica
   - Promover conhecimento sobre o universo Harry Potter
   - Desenvolver habilidades de resolução de problemas

2. **Técnico**
   - Demonstrar boas práticas em React
   - Implementar validação robusta de entrada
   - Criar interface acessível e responsiva
   - Exemplo de gerenciamento de estado eficiente

3. **Comunitário**
   - Código aberto para aprendizado
   - Base para expansões e modificações
   - Ferramenta educacional gratuita

### Filosofia de Desenvolvimento

> "Criar uma experiência de jogo educativa que combine entretenimento com aprendizado, mantendo código limpo, documentado e acessível para contribuidores."

## 📊 Status do Desenvolvimento

### ✅ Funcionalidades Implementadas
- [x] Sistema de 10 níveis progressivos
- [x] Validação inteligente de respostas
- [x] Sistema de pontuação (0-1.850 pts)
- [x] Sistema de dicas (-10 pts)
- [x] Interface responsiva
- [x] Animações e efeitos visuais
- [x] Sistema de tentativas (3 por nível)
- [x] Avaliação por estrelas
- [x] Suporte a teclado (Enter)

### 🚧 Em Desenvolvimento
- [ ] Sistema de salvamento de progresso (localStorage)
- [ ] Modo competitivo com ranking
- [ ] Estatísticas detalhadas de desempenho
- [ ] Internacionalização (i18n)

### 📋 Backlog
- [ ] Modo história expandido (15+ níveis)
- [ ] Sistema de conquistas
- [ ] Multiplayer em tempo real
- [ ] Efeitos sonoros e trilha sonora
- [ ] Modo treino (prática sem pontuação)
- [ ] API backend para ranking global

## 🧪 Testes

### Executar Testes
```bash
npm test
```

### Cobertura de Testes
```bash
npm run test:coverage
```

### Tipos de Teste
- **Unitários**: Validação de funções
- **Integração**: Fluxo de jogo completo
- **E2E**: Experiência do usuário

## 📦 Build e Deploy

### Build Local
```bash
npm run build
```

### Deploy no GitHub Pages
```bash
npm run deploy
```

### Deploy no Vercel/Netlify
```bash
# Vercel
vercel --prod

# Netlify
netlify deploy --prod
```

## ⚙️ Configuração

### Variáveis de Ambiente
Crie um arquivo `.env` na raiz:

```env
REACT_APP_VERSION=2.0.0
REACT_APP_API_URL=https://api.exemplo.com
```

### Personalização
Edite `src/data/levels.js` para adicionar ou modificar níveis:

```javascript
{
  id: 10,
  difficulty: "Extremo",
  title: "Seu Novo Nível",
  description: "Descrição...",
  question: "Pergunta?",
  answers: ["resposta1", "resposta2"],
  hint: "Dica útil",
  points: 300,
  type: "custom"
}
```

## 📄 Licença

Este projeto está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para detalhes.

### Resumo da Licença
```
✅ Uso comercial
✅ Modificação
✅ Distribuição
✅ Uso privado
❌ Responsabilidade
❌ Garantia
```

## 🙏 Agradecimentos

- **Debbie Matt** - Conceito original e inspiração
- **J.K. Rowling** - Universo Harry Potter
- **Comunidade React** - Ferramentas e suporte
- **Contribuidores** - Melhorias e correções

## 📞 Contato e Suporte

- **Issues**: [GitHub Issues](../../issues)
- **Discussões**: [GitHub Discussions](../../discussions)
- **Email**: deboramateusdec@gmail.com

## 🔗 Links Úteis

- 📖 **[Wiki do Projeto](https://github.com/DebbieMatt/code-and-riddle-acronyms/wiki)** - Documentação completa do jogo
- 🎮 **[Demo Live](https://debbiematt.github.io/code-and-riddle-acronyms/)**
- 📊 **[Roadmap](https://github.com/DebbieMatt/code-and-riddle-acronyms/projects/1)** - Planejamento de funcionalidades
- 🐛 **[Bug Tracker](https://github.com/DebbieMatt/code-and-riddle-acronyms/issues?q=is%3Aissue+is%3Aopen+label%3Abug)**
- 💡 **[Feature Requests](https://github.com/DebbieMatt/code-and-riddle-acronyms/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement)**

## 📈 Estatísticas

![GitHub stars](https://img.shields.io/github/stars/DebbieMatt/code-and-riddle-acronyms?style=social)
![GitHub forks](https://img.shields.io/github/forks/DebbieMatt/code-and-riddle-acronyms?style=social)
![GitHub issues](https://img.shields.io/github/issues/DebbieMatt/code-and-riddle-acronyms)
![GitHub pull requests](https://img.shields.io/github/issues-pr/DebbieMatt/code-and-riddle-acronyms)
![GitHub last commit](https://img.shields.io/github/last-commit/DebbieMatt/code-and-riddle-acronyms)

---

<div align="center">

**Desenvolvido com ⚡ por [Debbie Matt](https://github.com/DebbieMatt)**

*Para jogar e entender as mecânicas do jogo, consulte a [Wiki](https://github.com/DebbieMatt/code-and-riddle-acronyms/wiki)*

</div>
