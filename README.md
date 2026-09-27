# Hollow Cloud

Painel estático para supervisionar uma frota de bots Discord.

## Importante

Este repositório é o frontend do produto e pode ser publicado no GitHub Pages. GitHub Pages não executa processos, não mantém bots online, não envia e-mails de verificação e não deve receber senhas, tokens Discord ou chaves SMTP.

Para produção, conecte o painel a um backend com:

- allowlist de IDs de supervisor no servidor;
- autenticação com senha com hash forte, sessão curta e confirmação de e-mail;
- secrets server-side para Discord, SMTP e banco;
- upload de ZIP em sandbox, com limite, validação e proteção contra path traversal;
- worker separado por bot, health checks, logs, backoff e reinício controlado;
- rate limiting, auditoria, CSRF/origin checks e headers de segurança.

Nenhuma credencial fornecida em conversa deve ser colocada neste repositório. Credenciais expostas devem ser rotacionadas.