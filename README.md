<p align="center">
  <img src="https://img.shields.io/badge/Linux-Administração-ff69b4" alt="Linux Admin">
  <img src="https://img.shields.io/badge/50+-Comandos-ff1493" alt="50+ Comandos">
  <img src="https://img.shields.io/badge/DevOps-Essencial-dc7fb9" alt="DevOps">
</p>

<h1 align="center" style="color: #ff69b4;">🐧 Guia Essencial de Comandos Linux</h1>

<h3 align="center" style="color: #db7093;">Repositório criado para a disciplina de Administração de Servidores Linux</h3>

---

## 📚 Índice

- [🎯 Objetivo](#objetivo)
- [📋 Lista de Comandos](#lista-de-comandos)
  - [🗂️ Sistema de Arquivos](#sistema-de-arquivos)
  - [👥 Usuários e Permissões](#usuários-e-permissões)
  - [🔧 Gerenciamento de Sistema](#gerenciamento-de-sistema)
  - [🌐 Rede e Conectividade](#rede-e-conectividade)
  - [⚡ Desenvolvimento e Utilitários](#desenvolvimento-e-utilitários)
- [💡 Dicas Práticas](#dicas-práticas)
- [🤝 Como Contribuir](#como-contribuir)

---

## 🎯 Objetivo

Este repositório foi desenvolvido como atividade acadêmica para compilar os **comandos essenciais do Linux** utilizados na administração de servidores, seguindo os requisitos específicos da disciplina.

---

## 📋 Lista de Comandos

### 🗂️ Sistema de Arquivos

| Comando | Função | Uso Comum |
|---------|--------|-----------|
| `ls -la` | Lista detalhada com arquivos ocultos | `ls -la /home` |
| `cd ~` | Vai para o diretório home | `cd ~` |
| `pwd -P` | Mostra caminho físico real | `pwd -P` |
| `mkdir -p` | Cria diretórios com pais | `mkdir -p projeto/src` |
| `cp -r` | Copia recursivamente | `cp -r dir1/ dir2/` |
| `mv -i` | Move com confirmação | `mv -i arquivo.txt backup/` |
| `rm -rf` | Remove forçadamente | `rm -rf tmp/` |
| `touch -a` | Altera apenas acesso | `touch -a log.txt` |
| `cat -n` | Mostra com numeração | `cat -n script.sh` |
| `less -N` | Visualiza com números | `less -N config.conf` |
| `head -15` | Primeiras 15 linhas | `head -15 arquivo.log` |
| `tail -f` | Segue arquivo em tempo real | `tail -f app.log` |
| `find -name` | Busca por nome | `find /var -name "*.log"` |
| `grep -r` | Busca recursiva | `grep -r "ERROR" /logs` |
| `locate` | Busca rápida no sistema | `locate nginx.conf` |

### 👥 Usuários e Permissões

| Comando | Função | Uso Comum |
|---------|--------|-----------|
| `chmod 644` | Permissões padrão arquivos | `chmod 644 *.conf` |
| `chmod 755` | Permissões padrão executáveis | `chmod 755 script.sh` |
| `chown user:group` | Altera dono e grupo | `chown www-data:www-data site/` |
| `chgrp -R` | Altera grupo recursivo | `chgrp -R dev projeto/` |
| `whoami` | Identifica usuário atual | `whoami` |
| `id` | Mostra IDs do usuário | `id` |
| `who` | Usuários logados | `who` |
| `w` | Usuários e processos | `w` |
| `last` | Histórico de logins | `last` |
| `sudo -i` | Login como root | `sudo -i` |
| `su - username` | Troca de usuário | `su - deploy` |
| `passwd -l` | Bloqueia usuário | `passwd -l usuario` |

### 🔧 Gerenciamento de Sistema

| Comando | Função | Uso Comum |
|---------|--------|-----------|
| `ps aux` | Todos processos | `ps aux | grep mysql` |
| `top -p` | Monitora processo específico | `top -p 1234` |
| `htop` | TOP interativo | `htop` |
| `kill -9` | Mata processo forçadamente | `kill -9 1234` |
| `pkill` | Mata por nome | `pkill chrome` |
| `killall` | Mata todos do processo | `killall nginx` |
| `nice -n` | Altera prioridade | `nice -n 10 backup.sh` |
| `renice` | Re-altera prioridade | `renice 15 1234` |
| `df -h` | Espaço em disco legível | `df -h /home` |
| `du -sh` | Tamanho de diretório | `du -sh /var/log` |
| `free -m` | Memória em MB | `free -m` |
| `uname -r` | Versão do kernel | `uname -r` |
| `lsb_release -a` | Distribuição | `lsb_release -a` |
| `uptime` | Tempo ligado | `uptime` |
| `dmesg` | Mensagens do kernel | `dmesg | tail -20` |

### 🌐 Rede e Conectividade

| Comando | Função | Uso Comum |
|---------|--------|-----------|
| `ping -c 4` | 4 pacotes apenas | `ping -c 4 google.com` |
| `curl -I` | Apenas cabeçalhos | `curl -I http://localhost` |
| `wget -c` | Continua download | `wget -c arquivo.iso` |
| `ip addr show` | Interfaces de rede | `ip addr show eth0` |
| `netstat -tulnp` | Portas e processos | `netstat -tulnp` |
| `ss -tuln` | Socket statistics | `ss -tuln` |
| `scp -r` | Copia recursiva | `scp -r site/ user@host:/var/www` |
| `rsync -av` | Sincroniza arquivos | `rsync -av src/ dest/` |
| `ssh -p` | SSH em porta específica | `ssh -p 2222 user@host` |
| `traceroute` | Rota até host | `traceroute github.com` |
| `dig` | Consulta DNS | `dig example.com` |
| `nslookup` | Lookup DNS | `nslookup google.com` |
| `hostname -I` | IPs da máquina | `hostname -I` |
| `route -n` | Tabela de roteamento | `route -n` |
| `iptables -L` | Lista regras firewall | `iptables -L` |

### ⚡ Desenvolvimento e Utilitários

| Comando | Função | Uso Comum |
|---------|--------|-----------|
| `git clone` | Clona repositório | `git clone https://github.com/user/repo` |
| `docker ps` | Containers ativos | `docker ps -a` |
| `systemctl status` | Status de serviço | `systemctl status nginx` |
| `journalctl -f` | Segue logs systemd | `journalctl -f -u nginx` |
| `crontab -e` | Edita agendamentos | `crontab -e` |
| `tar -xzf` | Extrai tar.gz | `tar -xzf app.tar.gz` |
| `gzip` | Compacta arquivos | `gzip access.log` |
| `alias` | Cria atalhos | `alias ll='ls -la'` |
| `history` | Histórico de comandos | `history | grep ssh` |
| `man` | Manual do comando | `man grep` |
| `which` | Localiza comando | `which python3` |
| `whereis` | Localiza binários | `whereis nginx` |
| `date` | Data e hora | `date '+%Y-%m-%d %H:%M:%S'` |
| `timedatectl` | Configura data/hora | `timedatectl set-timezone America/Sao_Paulo` |
| `bc` | Calculadora terminal | `echo "5 + 3" | bc` |

---

## 💡 Dicas Práticas

```bash
# Combine comandos para maior produtividade
ps aux --sort=-%mem | head -10  # Top 10 processos por memória
grep -r "pattern" . --include="*.log"  # Busca em arquivos específicos
find . -name "*.tmp" -mtime +7 -delete  # Apaga arquivos antigos
