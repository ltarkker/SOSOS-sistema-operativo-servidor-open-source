# 🐧 [SOSOS] Sistema Operativo Servidor Open Source

> **CTeSP em Redes e Sistemas Informáticos** · ISTEC Porto · Ano letivo 2024/2025

---

## 📋 Informações da UC

| Campo | Detalhe |
|-------|---------|
| **Unidade Curricular** | Sistema Operativo Servidor Open Source |
| **Professor** | Joaquim Silva |
| **Curso** | CTeSP — Redes e Sistemas Informáticos |
| **Turma** | 2.º RSI |
| **Semestre** | 3.º Semestre |
| **Ano letivo** | 2024 / 2025 |
| **Aluno** | Gonçalo Lopes Fernandes · Nº 2022148 |
| **Nota Final** | Previsão de publicação final de curso em junho de 2026 |

---

## 📁 Estrutura do Repositório

```
.
├── material/
│   └── guia_avancado_redes_SOOS17_1.pdf       # Guia avançado de redes — VLANs, OSPF, UFW, Wireshark, Bash e Python
│
├── notas/
│   └── a.txt                                   # Placeholder
│
└── README.md
```

---

## 📝 Trabalhos Realizados

### Guia Avançado de Redes em Ubuntu

Guia prático completo de configuração e administração de redes em ambiente Linux (Ubuntu), dividido em três grandes módulos:

---

**1. Configuração de Rede**

**1.1 — Configuração de VLANs no Ubuntu:**
- Instalação do pacote `vlan` e ativação do módulo `802.1q`
- Configuração de VLANs via Netplan (`/etc/netplan/01-netcfg.yaml`)
- Exemplo prático: VLAN 10 (`192.168.10.2/24`) e VLAN 20 (`192.168.20.2/24`) na interface `ens33`
- Aplicação com `sudo netplan apply` e verificação com `ip addr show`

**1.2 — Roteamento Dinâmico com OSPF:**
- Instalação do FRR (Free Range Routing) — `sudo apt install frr`
- Configuração do OSPF em `/etc/frr/frr.conf` — redes `192.168.10.0/24` e `192.168.20.0/24` na área 0
- Reinício do serviço com `sudo systemctl restart frr`

---

**2. Segurança de Redes**

**2.1 — Configuração de Firewall com UFW:**
- Ativação do UFW — `sudo ufw enable`
- Regra para permitir SSH — `sudo ufw allow ssh`
- Regras personalizadas — permitir tráfego HTTP apenas da rede `192.168.10.0/24`
- Verificação de regras com `sudo ufw status verbose`

**2.2 — Monitorização de Tráfego com Wireshark:**
- Instalação do Wireshark e TShark
- Captura de pacotes na interface VLAN (`sudo tshark -i 3`)
- Análise de pacotes para identificação de problemas ou intrusões

---

**3. Automação e Scripts**

**3.1 — Introdução ao Bash:**
- Script de backup automático com `tar` para `/var/www/html`
- Permissões de execução com `chmod +x`
- Agendamento via `crontab` — execução diária às 02:00

**3.2 — Introdução ao Python para Redes:**
- Script Python para verificação de conectividade com `os.system("ping")`
- Teste de acessibilidade a múltiplos hosts (`192.168.10.1`, `8.8.8.8`)
- Execução com `python3 script.py`

---

## 🧠 Temas Abordados na UC

| Tema | Conteúdo |
|------|----------|
| Ubuntu Server | Administração de servidor Linux em ambiente de rede |
| VLANs em Linux | Pacote `vlan`, módulo `802.1q`, configuração via Netplan |
| Roteamento Dinâmico | OSPF com FRR (Free Range Routing) |
| Firewall (UFW) | Regras de entrada/saída, SSH, HTTP, filtragem por sub-rede |
| Wireshark / TShark | Captura e análise de pacotes de rede |
| Bash Scripting | Scripts de backup, `tar`, `chmod`, `crontab` |
| Python para Redes | Verificação de conectividade com `os.system` e `ping` |
| Netplan | Configuração de interfaces de rede em Ubuntu |

---

## 📬 Contacto

**Gonçalo Fernandes** · [goncalo.fernandes.2022148@my.istec.pt](mailto:goncalo.fernandes.2022148@my.istec.pt)
