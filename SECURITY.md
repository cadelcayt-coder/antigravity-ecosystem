# Política de Segurança

## 🛡️ Versões Suportadas

Atualmente, estamos fornecendo suporte de segurança para as seguintes versões:

| Versão | Suportada          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |
| < 1.0   | :x:                |

## 🚨 Reportando Vulnerabilidades

**NÃO** reporte vulnerabilidades de segurança através de issues públicas.

Se você descobrir uma vulnerabilidade de segurança, por favor:

### 1. Contato Privado

Envie um email para: **cadelcayt@gmail.com**

Incluir:
- Descrição detalhada da vulnerabilidade
- Passos para reproduzir
- Impacto potencial
- Sugestões de correção (se houver)

### 2. Não Divulgar Publicamente

Por favor, aguarde nossa resposta antes de divulgar publicamente. Trabalhamos para:

- Confirmar o problema em **48 horas**
- Fornecer um plano de ação em **1 semana**
- Lançar patch de segurança em **2 semanas** (casos críticos)

### 3. Hall da Fama

Pesquisadores de segurança que reportarem vulnerabilidades serão:

- Creditados publicamente (se desejarem)
- Listados em nosso Hall da Fama de Segurança
- Receberão reconhecimento oficial

## 🔒 Práticas de Segurança

### Para Usuários

1. **Mantenha Atualizado**: Use sempre a versão mais recente
2. **Credenciais**: Nunca compartilhe tokens ou chaves de API
3. **MCP Servers**: Verifique URLs e configurações antes de conectar
4. **Skills**: Revise código de skills de terceiros antes de usar
5. **Logs**: Não exponha logs com informações sensíveis

### Para Desenvolvedores

1. **Input Validation**: Sempre valide entradas de usuário
2. **Secrets Management**: Use variáveis de ambiente para credenciais
3. **Dependencies**: Mantenha dependências atualizadas
4. **Code Review**: Todo código passa por review de segurança
5. **Testing**: Inclua testes de segurança em skills

## 📊 Auditoria de Segurança

### Skills com SECURITY_LEVEL: High

Skills marcadas como `SECURITY_LEVEL: High` passam por:

- ✅ Revisão manual de código
- ✅ Análise de dependências
- ✅ Testes de penetração
- ✅ Validação de input sanitization
- ✅ Verificação de credential handling

### MCP Servers

Servidores MCP conectados são:

- Verificados quanto a autenticidade
- Monitorados por atividade suspeita
- Isolados em containers quando possível
- Atualizados regularmente

## ⚠️ Avisos de Segurança

### Skills de Cibersegurança

Skills como `pentest-commands`, `metasploit-framework`, etc., devem ser usadas:

- **APENAS** em ambientes de teste autorizados
- **NUNCA** contra sistemas sem permissão explícita
- Com total conformidade legal e ética

O uso inadequado é **ILEGAL** e de **RESPONSABILIDADE DO USUÁRIO**.

## 📝 Histórico de Segurança

### 2026

- **2026-02-06**: Release inicial 1.0.0
  - Implementação de políticas de segurança
  - Skills auditadas para SECURITY_LEVEL
  - MCP servers validados

## 🔗 Recursos

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE/SANS Top 25](https://cwe.mitre.org/top25/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

## 📞 Contato

Para questões de segurança:

- **Email**: cadelcayt@gmail.com
- **GitHub**: [@cadelcayt-coder](https://github.com/cadelcayt-coder)

---

*"Segurança não é um produto, é um processo." - Bruce Schneier*