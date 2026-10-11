# zabbix-noc-lab

> Monitoramento estilo **NOC** com **Zabbix + Grafana**: disponibilidade de hosts e serviços, alertas, dashboards e troubleshooting.

![Status](https://img.shields.io/badge/status-em%20constru%C3%A7%C3%A3o-yellow?style=flat-square) ![Foco](https://img.shields.io/badge/foco-NOC-0d1117?style=flat-square)

## Objetivo

Montar uma central de monitoramento: saber quando algo cai, por quê, e registrar a análise como um analista de NOC faria.

## Ambiente

| Componente | Função |
|---|---|
| Zabbix Server (Docker) | Coleta, triggers e alertas |
| Grafana | Dashboards de disponibilidade e desempenho |
| Zabbix Agent 2 | Linux, Windows 11 e VPS |
| SNMP / ICMP | Ativos de rede e checagem de ping |

## Roteiro

- [ ] Subir Zabbix + Grafana com Docker Compose
- [ ] Cadastrar hosts (Linux, Windows, VPS) com templates
- [ ] Monitorar CPU, memória, disco, serviços e portas
- [ ] Criar triggers e notificações (e-mail/Telegram)
- [ ] Dashboard de disponibilidade no Grafana
- [ ] Simular falhas (serviço parado, link fora, disco cheio) e documentar o diagnóstico

## Estrutura

```
docker/      docker-compose e configs
dashboards/  JSON dos dashboards do Grafana
incidentes/  simulações de falha: alerta → diagnóstico → solução
```

---
<sub>Laboratório em ambiente próprio e isolado.</sub>
