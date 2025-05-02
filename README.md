# 🖥️ Comandos CMD & PowerShell para Segurança da Informação

Este repositório contém uma lista de comandos úteis no Windows para atividades relacionadas à segurança da informação, auditoria e diagnóstico de rede.

## 📌 CMD (Prompt de Comando)

### 🔍 Verificar IP e conexões
- `ipconfig` – Mostra as configurações de rede.
- `ipconfig /all` – Exibe todas as informações detalhadas.
- `netstat -ano` – Lista conexões ativas e suas portas.
- `tasklist` – Mostra os processos ativos.

### 🔒 Segurança e usuários
- `net user` – Lista os usuários do sistema.
- `net localgroup administrators` – Mostra os administradores locais.
- `whoami` – Exibe o usuário atual.

---

## 📌 PowerShell

### 🔍 Auditoria e Rede
- `Get-NetIPAddress` – Lista os IPs configurados.
- `Get-EventLog -LogName Security -Newest 20` – Visualiza últimos logs de segurança.
- `Get-Process` – Lista processos em execução.
- `Test-NetConnection google.com` – Teste de conectividade (ping moderno).

### 🔒 Permissões e Acessos
- `Get-LocalUser` – Lista usuários locais.
- `Get-LocalGroupMember -Group "Administrators"` – Lista membros do grupo Admin.
- `Get-ExecutionPolicy` – Mostra a política de execução de scripts.

---

## 📁 Exemplos de Uso
### Verificar conexões suspeitas:
```bash
netstat -ano | findstr :443
