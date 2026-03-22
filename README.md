# 🎮 X360 Auto Tool (XEX & GOD)

Ferramenta automatizada para processamento de jogos de Xbox 360 em formatos **ISO, XEX e GOD**, com envio via **FTP** ou cópia offline e dashboard em tempo real.

Projetos incluídos:

* `X360AutoXex.exe` → Conversão e envio em formato **XEX/XBE**
* `X360AutoGod.exe` → Conversão e envio em formato **GOD**

---

## 🔹 Funcionalidades

* Processamento automático de:

  * ISOs
  * XEX / XBE
  * GOD (Games on Demand)
* Suporte a arquivos compactados (`.zip`, `.7z`, `.rar`, `.tar`, `.gz`, `.bz2`, `.xz`)
* **Watch Folder** (monitoramento automático)
* Fila de processamento com controle de duplicação
* Envio via **FTP** ou modo **offline**
* Dashboard Web em tempo real (progresso por arquivo)
* Histórico de atividades
* Acesso remoto via **ngrok** (opcional)
* Controle remoto com opção de desligar o PC

---

## ⚙️ Pré-requisitos

* Windows 10 ou superior
* .NET 6+ Runtime

Ferramentas necessárias na pasta `tools`:

* `7za.exe` → Extração de arquivos

* `extract-xiso.exe` → ISO → XEX

* `iso2god.exe` → ISO → GOD

* `WinSCP.com` → Envio via FTP

* `ngrok.exe` → Acesso remoto (opcional)

* Arquivo `config.ini` configurado

---

## 📝 Configuração (`config.ini`)

```ini
# FTP
ip=192.168.0.100
user=usuario
password=senha123
DEST_XEX=/Xbox360/XEX
DEST_XBE=/Xbox360/XBE

# Offline
OFFLINE=false
DEST_OFF=C:\Xbox360\Backup

# Watch Folder
WATCH_FOLDER=true
WATCH_FOLDER_PATH=Watch
```

---

## 🚀 Uso

1. Coloque arquivos ou pastas na **pasta base** ou **Watch Folder**
2. Execute conforme o formato desejado:

```bash
X360AutoXex.exe
```

ou

```bash
X360AutoGod.exe
```

3. Acesse o dashboard:

```
http://localhost:5000
```

4. (Opcional) Configure o ngrok para acesso remoto
5. Acompanhe o progresso em tempo real pelo navegador

---

## 🔧 Observações

* Processamento em **fila (1 por vez)** para evitar conflitos
* Detecção automática de arquivos completos antes do processamento
* Limpeza automática de arquivos temporários
* Suporte a múltiplos formatos no mesmo fluxo
* Dashboard com atualização em tempo real via WebSocket

---

## 📌 Notas

* O comportamento é totalmente automatizado após a configuração
* Ideal para uso contínuo com Watch Folder ativo
* Pode ser utilizado tanto localmente quanto em ambiente remoto