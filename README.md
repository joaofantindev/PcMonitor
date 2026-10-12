# PcMonitor

Anotações em Markdown sobre monitoramento de PCs (estações de trabalho e
servidores) com **Zabbix Agent**.

Este repositório reúne configurações, itens e templates usados para monitorar
máquinas Windows e Linux, centralizando cada host no Zabbix Server.

## Objetivo

- Padronizar a instalação e configuração do Zabbix Agent.
- Documentar itens de monitoramento (CPU, memória, disco, rede, logs).
- Registrar templates e User Parameters customizados.
- Facilitar o deploy em novos PCs.

## Conteúdo

- **Instalação** — Windows e Linux.
- **Configuração** — `zabbix_agentd.conf` / `zabbix_agent2.conf`.
- **Itens** — chaves nativas e User Parameters.
- **Templates** — templates vinculados aos hosts.
- **Alertas** — triggers e ações de notificação.
- **Troubleshooting** — problemas comuns e soluções.

## Estrutura

```
PcMonitor/
├── install/         # Instalação do agente (Windows/Linux)
├── config/          # Arquivos de configuração de exemplo
├── templates/       # Templates e User Parameters
├── items/           # Chaves e itens monitorados
└── troubleshooting/ # Erros comuns e soluções
```

## Convenções

- Um arquivo `.md` por assunto.
- Inclua o sistema operacional e a versão do Zabbix testada.
- Use blocos de código com a linguagem indicada (` ```conf `, ` ```bash `, ` ```powershell `).
- Nunca commite senhas, chaves ou tokens reais.

## Exemplo

```conf
# /etc/zabbix/zabbix_agent2.conf
Server=192.168.0.10
ServerActive=192.168.0.10
Hostname=pc-dev-01
```

## Referências

- Documentação Zabbix: https://www.zabbix.com/documentation/current/
