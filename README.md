## 🎮 X360AutoGod e X360AutoXex

Ferramenta automatizada para processamento de jogos de Xbox 360 nos formatos **ISO, XEX e GOD**, com suporte a envio via **FTP**, cópia offline e **dashboard em tempo real via navegador**.

### 📦 Projetos incluídos

* `X360AutoXex.exe` → Conversão e envio em formato **XEX/XBE**
* `X360AutoGod.exe` → Conversão e envio em formato **GOD (Games on Demand)**

---

## 🚀 Funcionalidades

* ✔ Processamento automático de:

  * ISOs
  * Jogos extraídos (XEX / XBE)
  * GOD (Games on Demand)

* ✔ Suporte a arquivos compactados:
  `.zip`, `.7z`, `.rar`, `.tar`, `.gz`, `.bz2`, `.xz`

* ✔ **Watch Folder (modo automático)**

* ✔ Fila inteligente (evita duplicação e conflitos)

* ✔ Envio via **FTP** ou cópia **offline**

* ✔ **Dashboard Web em tempo real (WebSocket)**

* ✔ Histórico de processamento

* ✔ Acesso remoto via **ngrok**

* ✔ Botão para desligamento remoto do PC

---

## ⚙️ Pré-requisitos

* Windows 10 ou superior
* .NET 6 ou superior

### 📁 Pasta `tools` obrigatória:

* `7za.exe` → Extração de arquivos
* `extract-xiso.exe` → Conversão ISO → XEX
* `iso2god.exe` → Conversão ISO → GOD
* `WinSCP.com` → Envio via FTP
* `ngrok.exe` → Acesso remoto (opcional)

---

## 📝 Configuração (`config.ini`)

```ini
# ==============================
# CONFIGURAÇÃO FTP - XBOX 360
# ==============================

ftp=true
ip=192.168.1.15
user=xboxftp
password=xboxftp

DEST=/Hdd1/Content/0000000000000000/
DEST_XEX=/Hdd1/MeusXEX/
DEST_XBE=/Hdd1/MeusClassicos/
DEST_TU_CACHE=/Hdd1/Cache/
DEST_OFF=E:/JogosXbox360/

# ==============================
# WATCH FOLDER
# ==============================

WATCH_FOLDER=true
WATCH_FOLDER_PATH=WatchFolder
```

---

## ▶️ Como usar

1. Coloque os arquivos (ISO, jogos ou compactados) na:

   * Pasta do programa **ou**
   * Pasta configurada como Watch Folder

2. Execute o programa desejado:

```bash
X360AutoXex.exe
```

ou

```bash
X360AutoGod.exe
```

3. Acesse o dashboard no navegador:

```
http://localhost:5000
```

4. acesso remoto com ngrok

```
primeiro acesso precisa fazer cadastro (mas sera direcionado diretamente para isso ai pode logar com conta google)
```

---

## 🌐 Dashboard

O sistema possui um painel web com:

* Progresso em tempo real por arquivo
* Status de cada etapa (extração, conversão, envio)
* Atualização automática via WebSocket
* Botão para desligamento remoto do PC

---

## ⚠️ Observações importantes

* Processamento em **fila (1 por vez)** para evitar conflitos
* Detecção automática de arquivos antes do processamento
* Limpeza automática de arquivos temporários
* Suporte a múltiplos formatos no mesmo fluxo
* Dashboard com atualização em tempo real
* **Sistema aprimorado para maior compatibilidade com diferentes hardwares e ambientes de uso**
* **Ajustes internos focados em estabilidade e adaptação a diversas situações do dia a dia**
* **Melhor comportamento em cenários variados, garantindo mais consistência durante o uso contínuo**

---

## 📌 Notas finais

* Após configurado, o sistema funciona de forma **totalmente automática**
* Ideal para servidores, setups dedicados ou uso contínuo
* Pode ser acessado localmente ou remotamente