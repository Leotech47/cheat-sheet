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

