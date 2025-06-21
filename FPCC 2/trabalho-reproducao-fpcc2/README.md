# Reproduzindo Experimento de Observabilidade em Sistemas Distribuídos

Este repositório contém os arquivos relacionados à reprodução experimental do artigo:

> **Informed and Assessable Observability Design Decisions in Cloud-Native Microservice Applications**  
> Borges, Maria C.; Bauer, Joshua; Werner, Sebastian; Gebauer, Michael; Tai, Stefan (ICSA 2024)

A reprodução foi conduzida como parte de um trabalho acadêmico do Programa de Pós-Graduação em Ciência da Computação da UFCG, dentro da disciplina FPCC2.

---

## 🧪 Objetivo do Experimento

Avaliar o impacto da injeção de falhas do tipo `pause` em um microsserviço (`recommendation-service`) de uma aplicação distribuída instrumentada com OpenTelemetry, utilizando a ferramenta **oxn**. A análise dos dados observáveis (traces e métricas) foi feita por meio de testes estatísticos automatizados.

---

## 📁 Estrutura dos Arquivos

| Arquivo/Folder | Descrição |
|----------------|-----------|
| `recommendation_pause_no_cpu.yml` | Script de experimento usado pelo `oxn`, define o cenário com falha do tipo *pause* de 120s. |
| `pause_multi_report.yml` | Relatório gerado automaticamente com estatísticas $t$, *p-values* e médias antes/depois da falha. |
| `resultado/` | Contém gráficos gerados a partir dos dados do relatório: barras, heatmaps e linha temporal por métrica. |

---

## 📊 Ferramentas Utilizadas

- [oxn](https://github.com/nymphbox/oxn): motor de experimentação para observabilidade.

---

## 📚 Referência Base

Borges, M. C., Bauer, J., Werner, S., Gebauer, M., & Tai, S. (2024).  
*Informed and Assessable Observability Design Decisions in Cloud-Native Microservice Applications*.  
In: IEEE International Conference on Software Architecture (ICSA 2024), pp. 69–78.  
DOI: [10.1109/ICSA59870.2024.00015](https://doi.org/10.1109/ICSA59870.2024.00015)

---

## 📄 Licença

Este repositório tem fins exclusivamente educacionais e acadêmicos. Consulte a licença dos projetos usados como base (oxn, etc.) em seus respectivos repositórios.

