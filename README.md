# 🎮 X360AutoGod e X360AutoXex

Ferramenta automatizada para processamento de jogos de Xbox 360 nos formatos **ISO, XEX e GOD**, com suporte a envio via **FTP**, cópia offline e **dashboard em tempo real via navegador**.

---

## 📸 Interface

<p align="center">
  <img src="assets/screenshot1.png" width="800"/>
</p>

<p align="center">
  <img src="assets/screenshot2.png" width="800"/>
</p>

<p align="center">
  <img src="assets/screenshot3.png" width="800"/>
</p>

---

## 📦 Projetos incluídos

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

1. Coloque os arquivos na pasta do programa ou Watch Folder
2. Execute:

```bash
X360AutoXex.exe
```

ou

```bash
X360AutoGod.exe
```

3. Acompanhe pelo CMD ou dashboard:

```
http://localhost:5000
```

---

## 🌐 Dashboard

* Progresso em tempo real
* Status de cada etapa
* Atualização automática via WebSocket
* Controle remoto do sistema

---

## ⚠️ Observações

* Processamento em **fila (1 por vez)**
* Limpeza automática de arquivos temporários
* Suporte a múltiplos formatos
* Sistema otimizado para uso contínuo

---

## 📌 Notas finais

* Funciona de forma **totalmente automática após configuração**
* Ideal para servidores ou uso contínuo
* Pode ser acessado localmente ou remotamente