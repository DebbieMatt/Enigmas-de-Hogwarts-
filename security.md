# Security Policy

## 🔒 Política de Segurança

Levamos a segurança do **Code And Riddle Acronyms** muito a sério. Este documento descreve nossas políticas de segurança e como reportar vulnerabilidades.

## 📋 Versões Suportadas

As seguintes versões do projeto estão atualmente recebendo atualizações de segurança:

| Versão | Suportada | Status | Data de Fim de Suporte |
| ------ | --------- | ------ | ---------------------- |
| 2.0.x  | ✅ | Ativa - Suporte completo | Indefinido |
| 1.0.x  | ⚠️ | Suporte limitado | 31/12/2025 |
| < 1.0  | ❌ | Sem suporte | Descontinuado |

### Detalhes das Versões

#### Versão 2.0.x (React - Atual)
- **Status**: Totalmente suportada
- **Atualizações**: Segurança, bugs e features
- **Frequência**: Patches mensais ou conforme necessário
- **Tecnologias**: React 18+, Tailwind CSS 3.4+
- **Recomendação**: ✅ Use esta versão

#### Versão 1.0.x (HTML/CSS/JS - Legacy)
- **Status**: Suporte limitado apenas para segurança crítica
- **Atualizações**: Apenas vulnerabilidades críticas
- **Frequência**: Conforme necessário
- **Tecnologias**: Vanilla JavaScript, CSS3
- **Recomendação**: ⚠️ Migre para 2.0.x

#### Versões < 1.0
- **Status**: Descontinuadas
- **Atualizações**: Nenhuma
- **Recomendação**: ❌ Não use

## 🛡️ Escopo de Segurança

### O que está coberto

Este projeto é um **jogo educacional frontend** que funciona inteiramente no navegador. Nossas considerações de segurança incluem:

✅ **Coberto por esta política:**
- Vulnerabilidades em dependências (React, Tailwind, Lucide)
- Problemas de XSS (Cross-Site Scripting)
- Injeção de código através de inputs
- Exposição de dados sensíveis no código
- Vulnerabilidades em bibliotecas de terceiros
- Problemas de autenticação (se implementados no futuro)
- CSRF (Cross-Site Request Forgery)
- Clickjacking
- Problemas de validação de entrada

❌ **NÃO coberto (fora do escopo):**
- Problemas relacionados ao GitHub Pages (infraestrutura)
- Bugs de gameplay que não envolvem segurança
- Problemas de performance ou UX
- Compatibilidade de navegadores (a menos que cause vulnerabilidade)
- Questões de acessibilidade (use Issues regulares)

### Dados e Privacidade

Este jogo **NÃO coleta, armazena ou transmite** dados pessoais:
- ✅ Nenhum backend ou servidor
- ✅ Nenhum tracking ou analytics
- ✅ Nenhum cookie ou localStorage persistente
- ✅ Nenhuma autenticação ou dados de usuário
- ✅ Execução 100% local no navegador

## 🚨 Reportando uma Vulnerabilidade

### Como Reportar

Se você descobrir uma vulnerabilidade de segurança, por favor **NÃO** abra uma Issue pública. Siga os procedimentos abaixo:

#### 1️⃣ Vulnerabilidades Críticas ou de Alta Gravidade

**Método Preferencial**: GitHub Security Advisory (Privado)

1. Acesse a aba **[Security](https://github.com/DebbieMatt/code-and-riddle-acronyms/security)** do repositório
2. Clique em **"Report a vulnerability"**
3. Preencha o formulário com:
   - **Tipo de vulnerabilidade**
   - **Versão afetada**
   - **Descrição detalhada**
   - **Passos para reproduzir**
   - **Impacto potencial**
   - **Possível correção** (se souber)

**OU**

**Email Privado**: debbiematt@exemplo.com

Assunto: `[SECURITY] Título da Vulnerabilidade`

```markdown
**Tipo**: [XSS / Injection / Dependency / Outro]
**Severidade**: [Crítica / Alta / Média / Baixa]
**Versão Afetada**: 2.0.x
**Ambiente**: [Navegador, OS, etc]

**Descrição**:
[Descrição clara da vulnerabilidade]

**Passos para Reproduzir**:
1. [Passo 1]
2. [Passo 2]
3. [...]

**Impacto**:
[Qual o potencial impacto desta vulnerabilidade?]

**Prova de Conceito** (opcional):
[Código ou screenshots demonstrando o problema]

**Correção Sugerida** (opcional):
[Se você souber como corrigir, descreva aqui]

**Contato**:
[Seu email ou método de contato preferido]
```

#### 2️⃣ Vulnerabilidades de Baixa Gravidade

Para problemas menores que não representam risco imediato:
- Abra uma **Issue privada** usando o template de segurança
- Ou envie por email se preferir

### ⏱️ Tempo de Resposta

Comprometemo-nos com os seguintes tempos de resposta:

| Severidade | Primeira Resposta | Resolução Estimada | Divulgação Pública |
|------------|-------------------|--------------------|--------------------|
| 🔴 Crítica | **24 horas** | 7 dias | Após correção + 7 dias |
| 🟠 Alta | **48 horas** | 14 dias | Após correção + 14 dias |
| 🟡 Média | **5 dias** | 30 dias | Após correção + 30 dias |
| 🟢 Baixa | **7 dias** | 60 dias | Após correção |

### 📊 Processo de Tratamento

#### Fase 1: Triagem (1-2 dias)
- ✅ Confirmação do recebimento
- ✅ Avaliação inicial da severidade
- ✅ Reprodução do problema
- ✅ Validação do escopo

#### Fase 2: Análise (2-5 dias)
- ✅ Investigação profunda
- ✅ Identificação de causa raiz
- ✅ Avaliação de impacto
- ✅ Planejamento da correção

#### Fase 3: Correção (3-14 dias)
- ✅ Desenvolvimento do fix
- ✅ Testes de segurança
- ✅ Code review
- ✅ Preparação do patch

#### Fase 4: Release (1-2 dias)
- ✅ Deploy da correção
- ✅ Atualização de versão
- ✅ Notificação de usuários
- ✅ Publicação de advisory

### 📢 Comunicação

Durante o processo, você pode esperar:

✅ **Confirmação inicial** dentro do prazo de primeira resposta
✅ **Atualizações regulares** sobre o progresso (semanal para críticas, quinzenal para outras)
✅ **Transparência** sobre aceitação ou rejeição da vulnerabilidade
✅ **Reconhecimento público** (se desejar) quando a correção for lançada
✅ **Detalhes do fix** após a divulgação responsável

### ✅ Se a Vulnerabilidade for Aceita

1. **Confirmação**: Reconhecemos o problema e validamos sua severidade
2. **Timeline**: Fornecemos um prazo estimado para correção
3. **Colaboração**: Podemos solicitar mais informações ou testes
4. **Crédito**: Você será creditado no CHANGELOG e Security Advisory (se desejar)
5. **Patch**: Lançaremos uma versão corrigida
6. **Divulgação**: Publicaremos o advisory após período de divulgação responsável

### ❌ Se a Vulnerabilidade for Rejeitada

1. **Explicação**: Forneceremos motivos detalhados da rejeição
2. **Orientação**: Se for um bug regular, direcionaremos para Issues
3. **Feedback**: Você pode contestar a decisão com informações adicionais
4. **Transparência**: Manteremos a comunicação aberta

## 🏆 Reconhecimento de Pesquisadores

Agradecemos aos seguintes pesquisadores de segurança que reportaram vulnerabilidades responsavelmente:

<!-- Esta seção será atualizada conforme vulnerabilidades forem reportadas e corrigidas -->

> Nenhuma vulnerabilidade reportada até o momento.

### Hall da Fama de Segurança

| Pesquisador | Vulnerabilidade | Severidade | Data | Versão Corrigida |
|-------------|-----------------|------------|------|------------------|
| - | - | - | - | - |

*Quer aparecer aqui? Reporte vulnerabilidades responsavelmente!*

## 🔐 Boas Práticas de Segurança para Contribuidores

Se você está contribuindo com o projeto, siga estas práticas:

### Código Seguro

```javascript
// ❌ NÃO FAÇA: Inserir HTML diretamente
element.innerHTML = userInput; 

// ✅ FAÇA: Usar text content ou sanitizar
element.textContent = userInput;
// OU
element.innerHTML = DOMPurify.sanitize(userInput);
```

### Validação de Input

```javascript
// ✅ Sempre normalize e valide inputs do usuário
const normalizeAnswer = (text) => {
  return text
    .toLowerCase()
    .trim()
    .replace(/[<>]/g, '') // Remove caracteres HTML
    .slice(0, 100); // Limite de tamanho
};
```

### Dependências

```bash
# ✅ Sempre audite dependências
npm audit

# ✅ Corrija vulnerabilidades automaticamente
npm audit fix

# ✅ Use versões exatas em produção
npm ci
```

### Checklist de Segurança

Antes de abrir um Pull Request, verifique:

- [ ] Nenhum dado sensível (API keys, senhas) no código
- [ ] Inputs do usuário são validados e sanitizados
- [ ] Dependências estão atualizadas e sem vulnerabilidades
- [ ] Nenhum `eval()` ou `Function()` com input do usuário
- [ ] CORS configurado corretamente (se aplicável)
- [ ] Nenhum console.log com dados sensíveis
- [ ] Error messages não expõem detalhes internos

## 📚 Recursos de Segurança

### Ferramentas Recomendadas

- **npm audit**: Auditoria de dependências
- **Snyk**: Monitoramento contínuo de vulnerabilidades
- **OWASP ZAP**: Teste de segurança de aplicações web
- **ESLint Security Plugin**: Análise estática de código

### Links Úteis

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [GitHub Security Best Practices](https://docs.github.com/en/code-security)
- [React Security Best Practices](https://reactjs.org/docs/dom-elements.html#dangerouslysetinnerhtml)
- [NPM Security Best Practices](https://docs.npmjs.com/auditing-package-dependencies-for-security-vulnerabilities)

## 📄 Divulgação Responsável

Seguimos os princípios de **divulgação responsável**:

### Nosso Compromisso

✅ **Não processaremos** pesquisadores que reportem vulnerabilidades de boa fé
✅ **Responderemos rapidamente** a todos os reports de segurança
✅ **Manteremos confidencialidade** até a correção e período de divulgação
✅ **Creditaremos publicamente** (se desejado) os pesquisadores
✅ **Publicaremos advisories** detalhados após a correção

### Seu Compromisso

Ao reportar uma vulnerabilidade, pedimos que você:

✅ **Mantenha confidencialidade** até a divulgação pública
✅ **Não explore** a vulnerabilidade além do necessário para demonstrá-la
✅ **Não acesse, modifique ou delete** dados de outros usuários
✅ **Não execute DoS** ou testes destrutivos
✅ **Nos dê tempo razoável** para corrigir o problema antes da divulgação pública

## 🚫 Atividades Proibidas

As seguintes atividades são **estritamente proibidas**:

❌ Denial of Service (DoS/DDoS)
❌ Spam ou phishing
❌ Acesso não autorizado a sistemas
❌ Destruição ou corrupção de dados
❌ Social engineering de usuários ou mantenedores
❌ Divulgação pública de vulnerabilidades antes da correção
❌ Extorsão ou chantagem

## 📞 Contato de Segurança

### Canal Primário
- **GitHub Security Advisory**: [Report a vulnerability](https://github.com/DebbieMatt/code-and-riddle-acronyms/security/advisories/new)

### Canal Secundário
- **Email**: debbiematt@exemplo.com (PGP key disponível sob solicitação)
- **Assunto**: `[SECURITY] Título`

### Tempo de Resposta Esperado
- **Crítica**: 24 horas
- **Alta**: 48 horas
- **Média/Baixa**: 5-7 dias

## 📜 Changelog de Segurança

Todas as atualizações de segurança são documentadas no [CHANGELOG.md](CHANGELOG.md) com a tag `[SECURITY]`.

### Histórico

**v2.0.0** (2025-11-11)
- Implementação inicial da política de segurança
- Migração para React com validação aprimorada de inputs
- Auditoria completa de dependências

---

## 📄 Licença desta Política

Esta política de segurança está sob a licença **[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)**.

---

**Última Atualização**: Novembro 11, 2025  
**Versão da Política**: 1.0  
**Mantenedor de Segurança**: [@DebbieMatt](https://github.com/DebbieMatt)

---

<div align="center">

**Obrigado por ajudar a manter o Code And Riddle Acronyms seguro!** 🔒

*Segurança é responsabilidade de todos nós.*

</div>
