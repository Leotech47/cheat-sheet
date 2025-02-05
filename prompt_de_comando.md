Aqui está uma **cheat sheet** completa do **Prompt de Comando (CMD) do Windows**, com suas características técnicas, comandos essenciais e utilidades.  

---

# **🖥️ Windows CMD Cheat Sheet**

## **📌 Características Técnicas**
- **Nome**: Prompt de Comando (Command Prompt, CMD)  
- **Base**: MS-DOS (Microsoft Disk Operating System)  
- **Extensão de Scripts**: `.bat` e `.cmd` (arquivos de lote)  
- **Modo de Execução**: Linha de comando interativa  
- **Arquitetura**: Suporte para comandos internos e externos do Windows  
- **Execução Elevada**: Pode ser executado como **Administrador**  
- **Suporte a Variáveis de Ambiente**: `%PATH%`, `%USERPROFILE%`, `%TEMP%`  
- **Manipulação de Arquivos e Diretórios**  
- **Administração do Sistema e Rede**  

---

## **🛠️ Comandos Básicos**
| **Comando** | **Descrição** |
|------------|-------------|
| `cls` | Limpa a tela do CMD |
| `exit` | Fecha o Prompt de Comando |
| `ver` | Exibe a versão do Windows |
| `help` | Lista os comandos disponíveis |

---

## **📂 Comandos para Arquivos e Pastas**
| **Comando** | **Descrição** |
|------------|-------------|
| `dir` | Lista arquivos e diretórios na pasta atual |
| `cd NomeDaPasta` | Entra em uma pasta específica |
| `cd ..` | Volta um nível no diretório |
| `mkdir NomeDaPasta` | Cria uma nova pasta |
| `rmdir NomeDaPasta /s /q` | Remove uma pasta e todo seu conteúdo |
| `del arquivo.txt` | Deleta um arquivo específico |
| `copy origem destino` | Copia um arquivo para outro local |
| `move origem destino` | Move um arquivo para outro local |

---

## **⚡ Comandos para Processos e Tarefas**
| **Comando** | **Descrição** |
|------------|-------------|
| `tasklist` | Lista os processos em execução |
| `taskkill /IM nome.exe /F` | Finaliza um processo pelo nome |
| `taskkill /PID 1234 /F` | Finaliza um processo pelo ID |
| `start programa.exe` | Abre um programa |

---

## **🌍 Comandos de Rede**
| **Comando** | **Descrição** |
|------------|-------------|
| `ipconfig` | Exibe informações da rede |
| `ipconfig /all` | Exibe detalhes da configuração de rede |
| `ping site.com` | Testa a conectividade com um servidor |
| `tracert site.com` | Rastreia a rota até um servidor |
| `nslookup site.com` | Obtém informações DNS de um site |
| `netstat -an` | Exibe conexões de rede ativas |
| `arp -a` | Exibe a tabela ARP da rede local |

---

## **🔑 Comandos de Usuário e Sistema**
| **Comando** | **Descrição** |
|------------|-------------|
| `whoami` | Exibe o usuário atual |
| `net user` | Lista todos os usuários do sistema |
| `net user nome /add` | Cria um novo usuário |
| `net user nome /delete` | Remove um usuário |
| `shutdown /s /t 0` | Desliga o computador imediatamente |
| `shutdown /r /t 0` | Reinicia o computador imediatamente |

---

## **🖥️ Comandos Avançados**
| **Comando** | **Descrição** |
|------------|-------------|
| `sfc /scannow` | Verifica e repara arquivos do sistema |
| `chkdsk /f` | Verifica e corrige erros no disco |
| `diskpart` | Gerencia partições de disco |
| `wmic` | Exibe informações do sistema |
| `powercfg /batteryreport` | Gera um relatório sobre a bateria |

---

## **📜 Scripts e Automação (Batch)**
- Para criar um **arquivo de script** no CMD:
  1. Abra o **Bloco de Notas**
  2. Digite os comandos, exemplo:
     ```bat
     @echo off
     echo Olá, mundo!
     pause
     ```
  3. Salve como **meuscript.bat**
  4. Execute no CMD digitando:  
     ```cmd
     meuscript.bat
     ```

---

## **💡 Dicas Úteis**
- **Executar o CMD como Administrador:**  
  Pressione `Win + R`, digite `cmd` e pressione `Ctrl + Shift + Enter`.
- **Copiar e Colar no CMD:**  
  Use `Ctrl + C` para copiar e `Ctrl + V` para colar (disponível no Windows 10+).
- **Histórico de Comandos:**  
  Pressione a tecla `F7` para ver os comandos já utilizados.

---

Abaixo, adiciono mais algumas seções para complementar a **cheat sheet do Prompt de Comando do Windows**, incluindo comandos adicionais, configurações avançadas e opções de personalização.

---

## **🖥️ Personalização do CMD**
| **Opção** | **Descrição** |
|------------|-------------|
| `color XY` | Altera as cores do fundo e do texto (`X` = fundo, `Y` = texto) |
| `title Meu Título` | Muda o título da janela do CMD |
| `mode con:cols=100 lines=30` | Define tamanho da janela do CMD |
| `prompt $P$G` | Personaliza o prompt de entrada |
| `echo Mensagem` | Exibe uma mensagem na tela |

📌 **Exemplo de comando para mudar a cor:**  
```cmd
color 0A
```
*(Fundo preto, texto verde)*  
Para ver a lista completa de cores, digite:  
```cmd
color /?
```

---

## **📝 Manipulação de Texto e Arquivos no CMD**
| **Comando** | **Descrição** |
|------------|-------------|
| `type arquivo.txt` | Exibe o conteúdo de um arquivo |
| `more arquivo.txt` | Exibe o conteúdo paginado de um arquivo |
| `find "palavra" arquivo.txt` | Busca uma palavra dentro de um arquivo |
| `sort arquivo.txt` | Ordena linhas de um arquivo em ordem alfabética |
| `clip < arquivo.txt` | Copia o conteúdo do arquivo para a área de transferência |

📌 **Exemplo: Buscar a palavra "erro" em um arquivo de log:**  
```cmd
find "erro" C:\logs\log.txt
```

---

## **📂 Gerenciamento de Drives e Discos**
| **Comando** | **Descrição** |
|------------|-------------|
| `diskpart` | Inicia a ferramenta de gerenciamento de discos |
| `wmic logicaldisk get name` | Lista todas as unidades de disco |
| `format X:` | Formata a unidade "X:" |
| `label X: Nome` | Altera o nome da unidade "X:" |
| `convert X: /FS:NTFS` | Converte um disco FAT32 para NTFS |

📌 **Para abrir a ferramenta de gerenciamento de discos diretamente:**  
```cmd
diskmgmt.msc
```

---

## **📡 Comandos de Rede Avançados**
| **Comando** | **Descrição** |
|------------|-------------|
| `netsh wlan show profiles` | Exibe redes Wi-Fi salvas |
| `netsh wlan show profile "NomeWiFi" key=clear` | Mostra a senha de uma rede Wi-Fi |
| `netstat -b` | Exibe programas que estão usando a rede |
| `route print` | Exibe tabela de roteamento da rede |
| `netsh int ip reset` | Reseta a configuração de IP |

📌 **Exemplo para descobrir a senha de uma rede Wi-Fi salva:**  
```cmd
netsh wlan show profile "MinhaRedeWiFi" key=clear
```
*(Substitua `"MinhaRedeWiFi"` pelo nome real da rede.)*

---

## **🔄 Gerenciamento de Tarefas e Serviços**
| **Comando** | **Descrição** |
|------------|-------------|
| `sc query` | Lista todos os serviços do Windows |
| `sc start NomeDoServico` | Inicia um serviço |
| `sc stop NomeDoServico` | Para um serviço |
| `schtasks /query` | Lista todas as tarefas agendadas |
| `schtasks /run /tn "NomeDaTarefa"` | Executa uma tarefa agendada manualmente |

📌 **Exemplo para reiniciar o serviço de spooler de impressão:**  
```cmd
sc stop Spooler && sc start Spooler
```

---

## **🔑 Segurança e Controle de Acesso**
| **Comando** | **Descrição** |
|------------|-------------|
| `cipher /E /S:C:\Pasta` | Criptografa uma pasta e seus arquivos |
| `cipher /D /S:C:\Pasta` | Descriptografa uma pasta e seus arquivos |
| `takeown /f C:\Arquivo.txt` | Assume a propriedade de um arquivo |
| `icacls C:\Arquivo.txt /grant Administradores:F` | Concede permissão total a um arquivo |

📌 **Exemplo para criptografar uma pasta inteira:**  
```cmd
cipher /E /S:"C:\MeusDocumentos"
```

---

## **🚀 Outras Ferramentas Úteis**
| **Comando** | **Descrição** |
|------------|-------------|
| `msconfig` | Abre a configuração do sistema |
| `gpedit.msc` | Abre o editor de diretivas de grupo (Windows Pro) |
| `regedit` | Abre o Editor do Registro do Windows |
| `dxdiag` | Exibe informações do DirectX |
| `cleanmgr` | Inicia a limpeza de disco |

📌 **Exemplo para abrir a limpeza de disco diretamente:**  
```cmd
cleanmgr /d C:
```

---

## **🎯 Atalhos Úteis no CMD**
| **Atalho** | **Função** |
|-----------|-----------|
| `Ctrl + C` | Interrompe a execução de um comando |
| `Ctrl + V` | Cola um texto (Windows 10+) |
| `Tab` | Completa automaticamente nomes de arquivos e diretórios |
| `F7` | Exibe histórico de comandos já digitados |
| `F3` | Repete o último comando digitado |

---

## **🔄 Redirecionamento de Saída e Entrada**
| **Comando** | **Descrição** |
|------------|-------------|
| `comando > arquivo.txt` | Salva a saída do comando em um arquivo |
| `comando >> arquivo.txt` | Adiciona a saída ao final do arquivo |
| `comando < arquivo.txt` | Usa um arquivo como entrada para um comando |
| `comando1 | comando2` | Envia a saída de um comando para outro comando |

📌 **Exemplo para salvar a saída de `dir` em um arquivo:**  
```cmd
dir > lista_arquivos.txt
```

---

## **📜 Exemplo de Script Completo no CMD**
Abaixo, um exemplo de script em **batch (`.bat`)** para **listar arquivos, criar backup e desligar o PC após a execução**:
```bat
@echo off
echo Listando arquivos...
dir C:\Users\Public\Documents > arquivos.txt

echo Criando backup...
xcopy C:\Users\Public\Documents D:\Backup /E /I /Y

echo Backup concluído. O PC será desligado em 1 minuto.
shutdown /s /t 60

pause
```
📌 **Para executar:**  
1. Copie o código para o **Bloco de Notas**  
2. Salve como **backup.bat**  
3. Dê um **duplo clique** para rodar  

---

## **📌 Conclusão**
O **Prompt de Comando do Windows (CMD)** é uma ferramenta poderosa para executar comandos, automatizar tarefas e administrar o sistema operacional. Com os comandos e truques acima, você pode melhorar sua produtividade e gerenciar o Windows de forma eficiente.

Parece que cobrimos praticamente **todos os comandos essenciais** e avançados do **Prompt de Comando do Windows (CMD)**. No entanto, podemos aprofundar ainda mais alguns tópicos úteis, como **diagnóstico de problemas, depuração, criação de menus interativos e integração com outras ferramentas**.

---

## **🛠️ Diagnóstico e Solução de Problemas no Windows via CMD**
Se precisar **identificar e corrigir problemas** no Windows diretamente pelo CMD, veja alguns comandos úteis:

| **Comando** | **Descrição** |
|------------|-------------|
| `sfc /scannow` | Verifica e repara arquivos do sistema corrompidos |
| `chkdsk C: /f /r` | Verifica e corrige erros no disco rígido |
| `DISM /Online /Cleanup-Image /RestoreHealth` | Repara a imagem do Windows |
| `net stop wuauserv && net stop bits` | Para serviços de atualização do Windows (útil para reset) |
| `systeminfo` | Exibe informações detalhadas sobre o sistema |
| `driverquery` | Lista todos os drivers instalados |
| `eventvwr` | Abre o Visualizador de Eventos do Windows |

📌 **Exemplo:** Para reparar arquivos corrompidos do sistema, execute:
```cmd
sfc /scannow
```
*(Pode levar alguns minutos para finalizar.)*

---

## **📜 Criando Scripts com Menus Interativos no CMD**
Você pode criar um **menu interativo** no CMD para facilitar a execução de comandos. Veja um exemplo prático:

```bat
@echo off
title Menu Principal - Ferramentas CMD
:menu
cls
echo ===================================
echo        MENU DE OPCOES
echo ===================================
echo 1. Listar arquivos da pasta atual
echo 2. Verificar conexoes de rede
echo 3. Limpar cache DNS
echo 4. Reiniciar o computador
echo 5. Sair
echo ===================================
set /p opcao="Escolha uma opcao: "

if "%opcao%"=="1" dir
if "%opcao%"=="2" netstat -an
if "%opcao%"=="3" ipconfig /flushdns
if "%opcao%"=="4" shutdown /r /t 0
if "%opcao%"=="5" exit

pause
goto menu
```

📌 **Como usar:**  
1. **Copie e cole** o código acima no **Bloco de Notas**  
2. **Salve como** `menu.bat`  
3. **Execute o arquivo** clicando duas vezes nele  

Esse script exibe um **menu interativo** e permite ao usuário escolher opções para executar comandos específicos.

---

## **🖥️ Integração do CMD com PowerShell**
O CMD permite rodar comandos **do PowerShell** diretamente, facilitando automação avançada.  
📌 **Exemplo: Executar um comando do PowerShell dentro do CMD**  
```cmd
powershell -command "Get-Service | Where-Object { $_.Status -eq 'Running' }"
```
Isso lista apenas os serviços que **estão em execução**.

📌 **Exemplo: Criar um usuário via CMD chamando PowerShell**
```cmd
powershell -command "New-LocalUser -Name 'NovoUsuario' -Password (ConvertTo-SecureString 'Senha123' -AsPlainText -Force) -FullName 'Usuario Teste' -Description 'Criado via CMD'"
```

---

## **📡 Integração do CMD com o Linux via WSL**
Se o **Windows Subsystem for Linux (WSL)** estiver instalado, você pode executar comandos Linux diretamente no CMD.

📌 **Exemplo:**  
```cmd
wsl ls -la
```
Isso lista os arquivos no diretório atual no ambiente Linux.

📌 **Executar um comando específico do Ubuntu no CMD:**
```cmd
wsl uname -r
```
Isso exibe a versão do kernel do Linux.

📌 **Executar um script bash do CMD:**
```cmd

wsl bash script.sh
```
Isso executa um script Linux dentro do Windows.

---

## **🛑 CMD vs. PowerShell: Qual Escolher?**
Se você ainda está em dúvida sobre **quando usar CMD ou PowerShell**, veja a comparação:

| **Critério** | **CMD** | **PowerShell** |
|-------------|---------|---------------|
| **Facilidade de Uso** | Simples e direto | Mais avançado |
| **Automação** | Suporte limitado a `.bat` | Suporte a `.ps1` com comandos avançados |
| **Manipulação de Arquivos** | Básico (`copy`, `move`, `del`) | Rico (`Copy-Item`, `Move-Item`, `Remove-Item`) |
| **Administração do Sistema** | Funciona, mas é básico | Permite gerenciar serviços, rede, Active Directory, etc. |
| **Objetos e Estruturas** | Baseado em texto puro | Baseado em objetos (JSON, XML, .NET) |
| **Execução de Scripts** | `.bat` ou `.cmd` | `.ps1` (PowerShell) |
| **Execução de Comandos do Linux** | Apenas via WSL | Mais integrado ao Linux |

📌 **Resumo:**  
- **Use CMD** para tarefas rápidas e comandos simples.  
- **Use PowerShell** para **automação avançada e administração do sistema**.

---

## **🔚 Conclusão**
O **Prompt de Comando (CMD)** do Windows continua sendo uma **ferramenta poderosa e essencial** para administração, diagnóstico e automação básica. Com os comandos e técnicas abordadas nesta **cheat sheet**, você pode:

✅ **Navegar e gerenciar arquivos e diretórios**  
✅ **Executar diagnósticos e resolver problemas do sistema**  
✅ **Automatizar tarefas com scripts `.bat`**  
✅ **Integrar-se ao PowerShell e Linux (WSL)**  
✅ **Criar menus interativos e scripts avançados**  

No **Prompt de Comando (CMD)** do Windows, você pode criar arquivos de diversas formas. Abaixo estão os principais métodos:

---

## **📜 Criando um Arquivo no CMD**

### **1. Criar um arquivo vazio (`echo.`)**
```cmd
echo. > arquivo.txt
```
Isso cria um arquivo **"arquivo.txt"** vazio.

---

### **2. Criar um arquivo com conteúdo (`echo`)**
```cmd
echo Este é um teste > arquivo.txt
```
Isso cria um arquivo **"arquivo.txt"** e insere o texto `"Este é um teste"` dentro dele.

📌 **Para adicionar mais linhas sem sobrescrever:**
```cmd
echo Nova linha >> arquivo.txt
```
O `>>` adiciona conteúdo ao final do arquivo sem apagar o que já existe.

---

### **3. Criar um arquivo usando `copy con` (método interativo)**
```cmd
copy con arquivo.txt
```
Depois, digite o conteúdo do arquivo e pressione **`Ctrl + Z`** seguido de **Enter** para salvar.

---

### **4. Criar um arquivo vazio com `fsutil` (requer permissões de admin)**
```cmd
fsutil file createnew arquivo.txt 0
```
Isso cria um arquivo vazio chamado **"arquivo.txt"** com **0 bytes**.

📌 **Criar um arquivo de tamanho específico (exemplo: 1 MB = 1048576 bytes):**
```cmd
fsutil file createnew arquivo.txt 1048576
```

---

### **5. Criar um arquivo usando `notepad`**
```cmd
notepad arquivo.txt
```
Isso abre o Bloco de Notas. Se o arquivo não existir, o Notepad perguntará se deseja criá-lo.

---

## **📌 Conclusão**
| **Método** | **Descrição** |
|------------|-------------|
| `echo. > arquivo.txt` | Cria um arquivo vazio |
| `echo Texto > arquivo.txt` | Cria um arquivo com conteúdo |
| `copy con arquivo.txt` | Modo interativo (salvar com `Ctrl + Z`) |
| `fsutil file createnew arquivo.txt 0` | Cria um arquivo de tamanho definido |
| `notepad arquivo.txt` | Abre o arquivo no Bloco de Notas |

Esses comandos funcionam para criar **arquivos de texto** no **CMD**, mas você pode alterar a extensão para `.bat`, `.csv`, `.log`, `.html` e outros conforme necessário.

No **Prompt de Comando (CMD)** do Windows, você pode **instalar, atualizar, verificar a versão e executar um software** de diferentes maneiras, dependendo do programa.  

Aqui estão os **principais métodos** para gerenciar softwares via CMD:

---

## **📥 1. Instalar um Software via CMD**
A instalação pode ser feita de diferentes formas:

### **1.1 Usando o `winget` (Windows 10 e 11)**
O **winget** é o gerenciador de pacotes oficial da Microsoft:
```cmd
winget install NomeDoSoftware
```
📌 **Exemplo:** Para instalar o Google Chrome:
```cmd
winget install Google.Chrome
```
📌 **Para encontrar o nome correto de um software:**
```cmd
winget search NomeDoSoftware
```

---

### **1.2 Usando o `choco` (Chocolatey)**
Se o **Chocolatey** estiver instalado, você pode usá-lo:
```cmd
choco install nome-do-software -y
```
📌 **Exemplo:** Instalar o **VLC Player**:
```cmd
choco install vlc -y
```

---

### **1.3 Instalando via Arquivo `.exe` ou `.msi`**
Se você já tem o arquivo de instalação, use:
```cmd
start /wait nome-do-arquivo.exe /silent /norestart
```
📌 **Exemplo:** Instalar o Chrome via `.exe` baixado:
```cmd
start /wait chrome_installer.exe /silent /install
```
📌 **Para um `.msi`:**
```cmd
msiexec /i nome-do-arquivo.msi /qn
```
*(O `/qn` executa em modo silencioso.)*

---

## **🔄 2. Atualizar um Software**
### **2.1 Atualizar com `winget`**
```cmd
winget upgrade NomeDoSoftware
```
📌 **Exemplo:** Atualizar o Chrome:
```cmd
winget upgrade Google.Chrome
```
📌 **Atualizar todos os softwares de uma vez:**
```cmd
winget upgrade --all
```

---

### **2.2 Atualizar com `choco`**
```cmd
choco upgrade nome-do-software -y
```
📌 **Exemplo:** Atualizar o VLC:
```cmd
choco upgrade vlc -y
```

---

## **🆙 3. Verificar a Versão de um Software**
### **3.1 Com `winget`**
```cmd
winget list NomeDoSoftware
```
📌 **Exemplo:** Verificar a versão do Chrome:
```cmd
winget list Google.Chrome
```

---

### **3.2 Verificar a versão manualmente**
Alguns programas oferecem um comando próprio para exibir a versão:
```cmd
nome-do-software --version
```
📌 **Exemplo:** Verificar a versão do Node.js:
```cmd
node --version
```
Ou:
```cmd
node -v
```

📌 **Para programas instalados via `.msi`:**
```cmd
wmic product get name,version
```
Isso lista **todos os softwares instalados** e suas versões.

---

## **🚀 4. Executar um Software via CMD**
### **4.1 Método Simples**
Se o programa estiver no **PATH do Windows**, basta digitar o nome:
```cmd
notepad
```
Isso abre o **Bloco de Notas**.

📌 **Outros exemplos:**
```cmd
chrome
calc
explorer
```

---

### **4.2 Executar a partir do Caminho Completo**
Se o programa não estiver no PATH, use o caminho completo:
```cmd
"C:\Program Files\Google\Chrome\Application\chrome.exe"
```

📌 **Exemplo para abrir o VLC:**
```cmd
"C:\Program Files\VideoLAN\VLC\vlc.exe"
```

---

### **4.3 Executar um Software como Administrador**
```cmd
runas /user:Administrador "C:\Caminho\Do\Programa.exe"
```
📌 **Exemplo:** Executar o CMD como admin:
```cmd
runas /user:Administrador "cmd.exe"
```

---

### **4.4 Executar um Programa e Esperar sua Finalização**
```cmd
start /wait notepad.exe
```
Isso abre o Bloco de Notas e o CMD só continua depois que ele for fechado.

---

## **📌 Resumo dos Comandos**
| **Ação** | **Comando** |
|------------|----------------------------|
| **Instalar com Winget** | `winget install NomeDoSoftware` |
| **Instalar com Chocolatey** | `choco install nome-do-software -y` |
| **Instalar via `.exe`** | `start /wait nome.exe /silent /install` |
| **Atualizar com Winget** | `winget upgrade NomeDoSoftware` |
| **Atualizar todos (Winget)** | `winget upgrade --all` |
| **Atualizar com Chocolatey** | `choco upgrade nome-do-software -y` |
| **Verificar a versão (Winget)** | `winget list NomeDoSoftware` |
| **Verificar versão de todos os programas** | `wmic product get name,version` |
| **Executar um programa** | `notepad`, `chrome`, `vlc`, etc. |
| **Executar via caminho completo** | `"C:\Caminho\Do\Programa.exe"` |
| **Executar como Administrador** | `runas /user:Administrador "cmd.exe"` |

---

