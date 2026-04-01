# 🐧 Linux Cheat Sheet

## 📚 Índice

* [📂 Arquivos e Diretórios](#-arquivos-e-diretórios)
* [🔐 Permissões](#-permissões)
* [⚙️ Processos](#-processos)
* [🌐 Rede](#-rede)
* [📦 Pacotes](#-pacotes)
* [🔍 Busca](#-busca)
* [📜 Logs](#-logs)
* [🔧 Systemd](#-systemd)
* [🐳 Docker](#-docker)
* [🧪 Troubleshooting](#-troubleshooting)

---

## 📂 Arquivos e Diretórios

| Comando                | Descrição                     |
| ---------------------- | ----------------------------- |
| `ls -la`               | Lista arquivos detalhado      |
| `cd /path`             | Navega entre diretórios       |
| `pwd`                  | Mostra diretório atual        |
| `du -sh *`             | Mostra tamanho dos diretórios |
| `df -h`                | Espaço em disco               |
| `cp -r origem destino` | Copia diretórios              |
| `mv origem destino`    | Move/renomeia                 |
| `rm -rf pasta`         | Remove diretório              |

---

## 🔐 Permissões

| Comando                 | Descrição                  |
| ----------------------- | -------------------------- |
| `chmod +x file`         | Torna executável           |
| `chmod 755 file`        | Define permissões          |
| `chown user:group file` | Altera dono                |
| `umask`                 | Define padrão de permissão |

---

## ⚙️ Processos

| Comando       | Descrição             |
| ------------- | --------------------- |
| `ps aux`      | Lista processos       |
| `top`         | Monitor em tempo real |
| `htop`        | Monitor avançado      |
| `kill PID`    | Finaliza processo     |
| `kill -9 PID` | Força finalização     |
| `pgrep nome`  | Busca processo        |

---

## 🌐 Rede

| Comando          | Descrição             |
| ---------------- | --------------------- |
| `ip a`           | Mostra IP             |
| `ss -tulnp`      | Portas abertas        |
| `ping host`      | Testa conectividade   |
| `curl url`       | Testa requisição HTTP |
| `wget url`       | Baixa arquivos        |
| `netstat -tulnp` | Portas (legado)       |

---

## 📦 Pacotes

### Debian/Ubuntu

| Comando           | Descrição             |
| ----------------- | --------------------- |
| `apt update`      | Atualiza repositórios |
| `apt upgrade`     | Atualiza pacotes      |
| `apt install pkg` | Instala pacote        |
| `apt remove pkg`  | Remove pacote         |

### RHEL/CentOS

| Comando           | Descrição        |
| ----------------- | ---------------- |
| `yum install pkg` | Instala pacote   |
| `yum update`      | Atualiza sistema |

---

## 🔍 Busca

| Comando                | Descrição       |
| ---------------------- | --------------- |
| `grep "texto" arquivo` | Busca texto     |
| `grep -r "texto" .`    | Busca recursiva |
| `find / -name arquivo` | Busca arquivo   |
| `locate arquivo`       | Busca rápida    |

---

## 📜 Logs

| Comando                   | Descrição          |
| ------------------------- | ------------------ |
| `tail -f /var/log/syslog` | Logs em tempo real |
| `less arquivo.log`        | Visualiza logs     |
| `journalctl -xe`          | Logs do systemd    |
| `dmesg`                   | Logs do kernel     |

---

## 🔧 Systemd

| Comando                     | Descrição         |
| --------------------------- | ----------------- |
| `systemctl status serviço`  | Status do serviço |
| `systemctl start serviço`   | Inicia serviço    |
| `systemctl stop serviço`    | Para serviço      |
| `systemctl restart serviço` | Reinicia          |
| `systemctl enable serviço`  | Habilita no boot  |
| `systemctl disable serviço` | Desabilita        |

---

## 🐳 Docker

| Comando                          | Descrição         |
| -------------------------------- | ----------------- |
| `docker ps`                      | Lista containers  |
| `docker ps -a`                   | Todos containers  |
| `docker images`                  | Lista imagens     |
| `docker run imagem`              | Executa container |
| `docker exec -it container bash` | Acessa container  |
| `docker logs container`          | Logs              |

---

## 🧪 Troubleshooting

| Problema         | Comando                 |
| ---------------- | ----------------------- |
| Porta ocupada    | `lsof -i :80`           |
| Processo travado | `kill -9 PID`           |
| Disco cheio      | `df -h`                 |
| Alto uso CPU     | `top`                   |
| Serviço não sobe | `journalctl -u serviço` |

---

💡 Dica: mantenha este cheat sheet atualizado com comandos que você usa no dia a dia.
