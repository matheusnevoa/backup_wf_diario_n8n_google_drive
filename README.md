# 🔄 backup_wf_diario_n8n_google_drive

Backup automático dos workflows do **n8n** para o **Google Drive**, com organização por data e nome original dos fluxos.

---

## 📌 Visão Geral

Este fluxo permite que você realize **backups diários automáticos** de todos os seus workflows no n8n, exportando-os em formato `.json` para uma pasta no Google Drive.

### O que ele faz:

- 🗂️ Usa uma **pasta raiz definida por você** no Drive
- 📅 Cria uma **subpasta automaticamente com a data** do backup (ex: `2025-07-13`)
- 🧾 Exporta todos os workflows via API do n8n
- 💾 Converte para `.json` com o **nome original do fluxo**
- ☁️ Faz o upload para o Google Drive, organizando os arquivos por data

---

## ⚙️ Requisitos

- Conta no [n8n](https://n8n.io/)
- Google Drive com OAuth2 configurado no n8n
- API Key do n8n habilitada
- Permissões de escrita na pasta de destino no Drive

---

## 🚀 Como usar

1. Importe o arquivo `backup_wf_diario_n8n_google_drive.json` no seu n8n
2. No nó **"Create folder"**, defina o ID da pasta raiz no Google Drive
3. Configure sua credencial Google Drive OAuth2
4. Ajuste a agenda no nó `Schedule Trigger` (ex: rodar todos os dias às 3h)
5. Salve e ative o fluxo

---

## 📂 Estrutura no Google Drive

```
Pasta_Raiz/
├── 2025-07-13/
│   ├── fluxo_cadastro_clientes.json
│   ├── processo_de_aprovacao.json
│   └── ...
├── 2025-07-14/
│   └── ...
```

---

## 📄 Exemplo de uso

Imagine que você tem 30 workflows ativos no seu ambiente n8n. Este fluxo criará uma subpasta com a data do dia e salvará todos os `.json` com seus nomes originais, organizando diariamente os backups.

---

## 👨‍💻 Autor

Desenvolvido por **[Matheus Névoa](https://www.linkedin.com/in/matheusnevoa/)**  
Especialista em automações com n8n, Fluig e integrações corporativas.

---

## 🏷️ Tags

`n8n` `backup` `google drive` `workflow automation` `json` `OAuth2` `n8n API` `low-code` `dataops` `cloud automation`
