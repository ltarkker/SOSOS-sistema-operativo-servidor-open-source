# 🐧 [SOSOS] Sistema Operativo Servidor Open Source

> **CTeSP em Redes e Sistemas Informáticos** · ISTEC Porto · Ano letivo 2024/2025

---

## 📋 Informações da UC

| Campo | Detalhe |
|-------|---------|
| **Unidade Curricular** | Sistema Operativo Servidor Open Source |
| **Professor** | Joaquim Silva |
| **Curso** | CTeSP — Redes e Sistemas Informáticos |
| **Período Letivo** | 1.º Semestre |
| **Ano Curricular** | 2.º (3.º Semestre) |
| **Ano letivo** | 2024 / 2025 |
| **Aluno** | Gonçalo Lopes Fernandes · Nº 2022148 |
| **Nota Final** | 19 — Dezanove valores |

---

## 📁 Estrutura do Repositório

```
.
├── material/
│   ├── FICHAUBUNTUSERVER_GoncaloFernandes.pdf    # Ficha — Instalação e configuração do Ubuntu Server
│   ├── guia_avancado_redes_SOOS17_1.pdf          # Guia avançado de redes — VLANs, OSPF, UFW, Wireshark, Bash e Python
│   ├── Instalação do Fedora no VirtualBox.pdf    # Guia de instalação do Fedora no VirtualBox
│   ├── Relatorio_FICHA2.docx                     # Ficha 2 — Instalação de aplicações e monitorização de rede (Fedora)
│   └── Relatorio_FICHA4.pdf                      # Ficha 4 — Nginx, Virtual Hosts e HTTPS com Let's Encrypt
└── notas/
    └── MOD.IP.022.R3.12.24 Pauta CTeSP 2º RSI.pdf  # Pauta final — 19 valores
```

---

## 📝 Trabalhos Realizados

### 1. Ficha — Instalação e Configuração do Ubuntu Server

Relatório completo de instalação do Ubuntu Server 24.04.1 LTS numa máquina virtual, cobrindo:

- **Preparação** — Download da ISO LTS e criação de USB bootável com Rufus
- **Instalação** — Assistente de instalação, configuração de rede (DHCP/estático), particionamento de disco, criação de utilizador
- **Configuração inicial** — Atualização do sistema (`sudo apt update && sudo apt upgrade`), configuração de rede via Netplan (`/etc/netplan/01-netcfg.yaml`)
- **Gestão de pacotes com APT** — Instalação, remoção e pesquisa de pacotes, adição de repositórios PPA
- **Servidores Web** — Instalação e configuração do Apache (`sudo apt install apache2`)

### 2. Ficha 2 — Atividades Básicas com Linux Fedora

Guia prático de atividades em Fedora Linux abrangendo:

- **Atualização do sistema** — `sudo dnf update -y`
- **Instalação de aplicações** — GNOME Tweaks, VLC, GIMP, LibreOffice, Flatpak
- **Ferramentas de monitorização de rede** — Wireshark (análise de tráfego), Nmap (varredura de rede), vnstat (monitorização de tráfego)
- **Aplicações adicionais** — Steam, OBS Studio, VirtualBox

### 3. Guia Avançado de Redes em Ubuntu

Guia prático completo de configuração e administração de redes em ambiente Linux (Ubuntu), dividido em três módulos:

**Módulo 1 — Configuração de Rede:**
- Configuração de VLANs — pacote `vlan`, módulo `802.1q`, Netplan (VLAN 10 e VLAN 20 na interface `ens33`)
- Roteamento dinâmico com OSPF — instalação e configuração do FRR (Free Range Routing)

**Módulo 2 — Segurança de Redes:**
- Firewall com UFW — regras SSH, HTTP, filtragem por sub-rede (`192.168.10.0/24`)
- Monitorização de tráfego com Wireshark e TShark — captura e análise de pacotes

**Módulo 3 — Automação e Scripts:**
- Bash — script de backup automático com `tar`, agendamento via `crontab` (diário às 02:00)
- Python para redes — script de verificação de conectividade com `os.system("ping")`

### 4. Ficha 4 — Nginx, Virtual Hosts e HTTPS

Trabalho prático de configuração completa de um servidor web Nginx em Ubuntu, com quatro atividades:

1. **Instalação do Nginx** — `sudo apt install nginx`, verificação de status com `systemctl`, acesso à página padrão
2. **Configuração de Virtual Host** — Criação de diretório do site, configuração em `/etc/nginx/sites-available/`, link simbólico para `sites-enabled/`, página HTML personalizada
3. **Simulação de domínio local** — Edição do ficheiro `/etc/hosts` para mapear `meusite.com` para `127.0.0.1`
4. **HTTPS com Let's Encrypt** — Instalação do Certbot (`python3-certbot-nginx`), obtenção de certificado SSL, teste de renovação automática, redirecionamento HTTP → HTTPS

---

## 🧠 Temas Abordados na UC

| Tema | Conteúdo |
|------|----------|
| Ubuntu Server | Instalação, configuração inicial e administração de servidor Linux |
| Fedora Linux | Instalação em VirtualBox, gestão de pacotes com DNF, aplicações |
| Gestão de pacotes | APT (Ubuntu) e DNF (Fedora) — instalação, remoção, repositórios |
| Configuração de rede | Netplan, IP estático, DHCP, interfaces de rede |
| VLANs em Linux | Pacote `vlan`, módulo `802.1q`, configuração via Netplan |
| Roteamento Dinâmico | OSPF com FRR (Free Range Routing) |
| Firewall (UFW) | Regras de entrada/saída, SSH, HTTP, filtragem por sub-rede |
| Wireshark / TShark | Captura e análise de pacotes de rede |
| Servidores Web | Apache e Nginx — instalação, configuração, Virtual Hosts |
| HTTPS / SSL | Let's Encrypt, Certbot, certificados SSL, redirecionamento HTTP→HTTPS |
| Bash Scripting | Scripts de backup, `tar`, `chmod`, `crontab` |
| Python para Redes | Verificação de conectividade com `os.system` e `ping` |

---

## 📬 Contacto

**Gonçalo Fernandes** · [goncalo.fernandes.2022148@my.istec.pt](mailto:goncalo.fernandes.2022148@my.istec.pt)

---

*CTeSP em Redes e Sistemas Informáticos · ISTEC Porto · 2024/2025*
