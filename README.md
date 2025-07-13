Backup automático de workflows do n8n para o Google Drive, com organização por data e nome original dos fluxos.

Este fluxo realiza, diariamente, a exportação completa dos workflows do ambiente n8n em formato `.json`, criando uma subpasta com a data do backup e armazenando tudo diretamente no Google Drive do usuário. Ideal para versionamento pessoal, segurança de dados e organização em ambientes com múltiplos projetos.

- Agendamento automático via `Schedule Trigger`
- Integração via API do n8n e Google Drive (OAuth2)
- Nome dos arquivos preservado (nome original do workflow)
- Estrutura modular e pronta para produção

Criado por [Matheus Névoa](https://www.linkedin.com/in/matheusnevoa/)
