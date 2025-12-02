# 👕 TexFlow 3.0 (Enterprise Edition)

**Sistema Integrado de Gestão para Confecções Têxteis (SaaS).**

O **TexFlow** evoluiu de um simples gerenciador de estoque para uma plataforma completa de gestão têxtil baseada em nuvem, com segurança de nível bancário e controle de licenciamento.

![Status](https://img.shields.io/badge/Status-Production-green)
![Versão](https://img.shields.io/badge/Version-3.0-blue)
![Database](https://img.shields.io/badge/MongoDB-Atlas-forestgreen)
![Security](https://img.shields.io/badge/Encryption-AES256-red)

---

## 🚀 O Que Há de Novo na v3.0?

### 🔐 Segurança & Licenciamento (SaaS)
* **Validação em Tempo Real:** O sistema verifica a licença do cliente a cada inicialização, consultando servidores de hora mundial (NTP) para evitar fraudes de relógio.
* **Alertas de Vencimento:** Barra de notificação visual (Laranja/Vermelha) no rodapé quando a licença está próxima do fim.
* **Bloqueio Automático:** Suspensão automática de acesso após o período de carência, com gestão remota pelo administrador.

### 📢 Comunicação em Tempo Real
* **Central de Avisos:** Sistema de broadcast onde o administrador pode enviar notificações (Manutenção, Cobrança, Avisos Gerais) que aparecem instantaneamente na tela de todos os usuários ativos.

### 🛡️ Infraestrutura Blindada
* **Criptografia de Ponta a Ponta:** As conexões com o banco de dados são criptografadas com chave simétrica (Fernet/AES). O arquivo de configuração local é protegido e oculto do usuário final.
* **Multi-Tenant:** Arquitetura preparada para múltiplos clientes isolados, com bancos de dados segregados e busca automática de credenciais em repositório privado.

---

## 📦 Funcionalidades Principais

### 🏭 Chão de Fábrica
- **Rastreamento Total:** Controle de Lotes (Corte -> Costura -> Acabamento -> Estoque).
- **Materiais:** Suporte completo a **Algodão, Peruana, Suedine e Moletom**.
- **Status Dinâmico:** Atualização automática baseada no setor do prestador de serviço.

### 💰 Comercial & Estoque
- **Venda Rápida:** Baixa de estoque intuitiva com proteção contra cliques duplos.
- **Estorno Seguro:** Função "Desfazer Venda" que corrige lançamentos errados e devolve os itens ao estoque automaticamente.
- **Visão Geral:** Painel com totais separados por tipo de tecido em tempo real.

### 🎨 Interface (UI/UX)
- **Modo Escuro/Claro:** Alternância nativa de temas.
- **Responsividade:** Adaptação automática para telas de baixa resolução (Notebooks/720p) com barras de rolagem inteligentes.
- **Menu de Ajustes:** Nova central de configurações (Engrenagem) para gestão da conta e suporte.

---

## 🛠️ Stack Tecnológico

- **Core:** Python 3.11
- **GUI:** CustomTkinter (Modern Design)
- **Database:** MongoDB Atlas (NoSQL)
- **Security:** Cryptography (Fernet)
- **Deploy:** PyInstaller (Single-file EXE)

---

## 📞 Suporte

Dúvidas ou problemas técnicos?
Acesse o menu de **Configurações (⚙️)** dentro do sistema e clique em **"Falar com Suporte"** para atendimento via WhatsApp.

---
**Desenvolvido por SugarFoot** *© 2025 TexFlow Systems*

# 👕 TexFlow 2.0

**Sistema Inteligente de Gestão para Confecções Têxteis.**

O **TexFlow** é uma solução completa desenvolvida em Python para gerenciar o ciclo de vida de produção de roupas, desde o corte do tecido até a venda final, com controle de estoque em tempo real na nuvem.

![Status](https://img.shields.io/badge/Status-Stable-green)
![Python](https://img.shields.io/badge/Python-3.11+-blue)
![Database](https://img.shields.io/badge/MongoDB-Atlas-forestgreen)
![Interface](https://img.shields.io/badge/UI-CustomTkinter-orange)

---

## 🚀 Funcionalidades Principais

### 🏭 Controle de Produção
- **Rastreamento de Lotes:** Acompanhe cada lote (Corte -> Costura -> Acabamento -> Estoque).
- **Status Dinâmico:** O sistema identifica automaticamente o setor (ex: "Na Costura", "No Silk", "No Embolso") baseando-se no parceiro selecionado.
- **Gestão de Parceiros:** Cadastro de prestadores de serviço com categorias específicas.

### 📦 Estoque & Vendas
- **Estoque em Nuvem:** Sincronização em tempo real via MongoDB Atlas.
- **Venda Rápida:** Seleção direta na tabela de estoque com baixa automática.
- **Histórico e Correção:** Log completo de vendas com função de **"Desfazer Venda"** (estorno de estoque).
- **Visualização:** Tabelas separadas por tipo de tecido (Algodão, Peruana, Suedine).

### 🛡️ Segurança & Tecnologia
- **Autenticação Blindada:** O sistema busca as credenciais do banco de dados em um **Repositório Privado** no GitHub, garantindo que a senha nunca fique exposta.
- **Configuração Oculta:** Criação de arquivo `config.ini` oculto no sistema do cliente.
- **Auto-Updater:** Sistema de atualização automática (OTA) integrado ao GitHub Releases. O cliente sempre tem a última versão.

### 🎨 Interface Moderna
- **Design Responsivo:** Adapta-se a monitores pequenos (720p) e grandes (1080p+).
- **Dark/Light Mode:** Alternância de tema nativa.
- **Ícone e Logo:** Identidade visual integrada.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3.11
- **Interface Gráfica:** CustomTkinter (Modern UI) & Tkinter (Treeview)
- **Banco de Dados:** MongoDB Atlas (NoSQL)
- **Bibliotecas:** - `pymongo` & `certifi` (Conexão DB)
    - `requests` (API GitHub e Updates)
    - `pillow` (Manipulação de Imagens)
    - `pyinstaller` (Compilação EXE)

---

📦 Instalação (Para Clientes)
Baixe a última versão na aba Releases.

Coloque o arquivo TexFlow.exe em uma pasta de sua preferência.

Execute o programa.

Na primeira execução, digite seu Nome de Cliente para ativar a licença e conectar ao banco de dados.

---

## 📸 Galeria de Evolução (Screenshots)

Aqui você pode ver a evolução visual do projeto, desde a primeira versão até o design moderno atual.

<details>
<summary><strong>✨ Versão 2.0 (Atual - Design Moderno & Dark Mode)</strong></summary>
<br>

> A versão atual conta com interface CustomTkinter, Modo Escuro nativo e ícones integrados.

| Tela Inicial | Corte |
| :---: | :---: |
| ![Home](Screenshots/v2.0/telainicial.png) | ![Estoque](Screenshots/v2.0/corte.png) |

| Produção | Vendas |
| :---: | :---: |
| ![Cadastro](Screenshots/v2.0/producao.png) | ![Vendas](Screenshots/v2.0/estoque.png) |

</details>

<details>
<summary><strong>🏚️ Versão 1.0 (Legado - Visual Clássico)</strong></summary>
<br>

> A primeira versão utilizava interface nativa do Windows (Tkinter Padrão) e layout cinza.

![Versão 1.0 Geral](Screenshots/v1.0/telainicial.png)

</details>


---

Desenvolvido por SugarFoot Versão Atual: 2.0
