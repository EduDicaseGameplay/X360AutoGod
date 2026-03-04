# 🎮 X360 AUTO TOOL SUITE

### Automação Inteligente para Xbox 360 RGH / Exploit

O **X360 Auto Tool Suite** é um conjunto de ferramentas desenvolvidas por **Eduardo Henrique (Edu Dicas e Gameplay)** para automatizar completamente o preparo e envio de jogos para Xbox 360 desbloqueado (RGH/JTAG/Exploit).

O projeto é dividido em dois módulos independentes que trabalham juntos:

---

# 🔷 1️⃣ X360 Auto GOD Tool

Automatiza o processo completo de:

📦 Arquivo compactado → 🎮 ISO → 💿 GOD → 🌐 FTP ou 💾 Offline

## 🔥 Funcionalidades

* Detecção automática de `.zip`, `.rar`, `.7z`, `.iso`
* Extração automática via 7-Zip
* Conversão ISO → GOD via iso2god
* Monitoramento de progresso real
* Modo FILA automático
* Watch Folder com processamento sequencial
* Validação de estrutura GOD:

  * 00007000
  * 000B0000
  * 00000002
* Verificação de TitleID no console (evita duplicados)
* Envio automático de pasta Cache (Title Update)
* Modo FTP inteligente
* Modo OFFLINE (cópia para HD externo)
* Teste automático de conexão com console

Ideal para quem usa formato **Content\0000000000000000**.

---

# 🔷 2️⃣ X360 Auto XEX Tool

Automatiza:

🎮 ISO → 📂 XEX
🎮 ISO Clássico → 📂 XBE

## 🔥 Funcionalidades

* Extração automática via extract-xiso
* Detecção automática de jogo:

  * Xbox 360 (.xex)
  * Xbox Clássico (.xbe)
* Separação automática:

  * temp/XEX
  * temp/XBE
* Sanitização automática do nome do jogo
* Modo FILA unificada
* Watch Folder com fila sequencial
* Proteção contra envio duplicado
* Upload separado para:

  * DEST_XEX
  * DEST_XBE
* Modo OFFLINE (DEST_OFF)
* Validação inteligente de config.ini
* Teste automático de conexão FTP
* Proteção contra divisão por zero
* Mensagens claras e status detalhado

Ideal para quem prefere rodar jogos em formato **pasta extraída**.

---

# ⚙️ Modos Disponíveis

| Modo         | Descrição                                |
| ------------ | ---------------------------------------- |
| FTP          | Envia direto para o console              |
| OFFLINE      | Copia para HD externo                    |
| FILA         | Processa múltiplos jogos automaticamente |
| WATCH FOLDER | Monitora pasta e processa sozinho        |
| CACHE AUTO   | Envia Title Update automaticamente       |

---

# 🖥️ Requisitos

* Windows 10 ou superior

### Ferramentas externas necessárias:

* 7za.exe (7-Zip portátil)
* iso2god.exe
* extract-xiso.exe
* WinSCP.com

---

# 🔒 Aviso Legal

O projeto é destinado exclusivamente para uso com **seus próprios dumps de jogos**.

Não apoiamos:

* Pirataria
* Distribuição de jogos protegidos
* Uso ilegal de conteúdo

Use com responsabilidade.

---

# 💖 Apoie o Projeto

Se deseja apoiar o desenvolvimento contínuo:

Chave Pix:
`838ef691-cfae-41ec-9b98-8fbb3d0e47a4`

---

# 🧠 Desenvolvido por

Eduardo Henrique
Canal: Edu Dicas e Gameplay