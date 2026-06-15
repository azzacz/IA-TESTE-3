# Maverick Roadmap

## Objetivo inicial

Organizar o repositório `IA-TESTE-3` como base de experimentação para IA, agentes, automações e integração futura com o ecossistema Maverick.

## Fase 0 — Segurança e inventário

- [ ] Confirmar se o repositório deve continuar público.
- [ ] Mapear arquivos grandes e dependências.
- [ ] Verificar existência de segredos expostos.
- [ ] Criar `.gitignore` adequado.
- [ ] Criar `.env.example` seguro.
- [ ] Documentar stack real.

## Fase 1 — Organização

- [ ] Separar documentação Maverick da documentação original do projeto base.
- [ ] Criar pasta `docs/maverick/` se necessário.
- [ ] Criar mapa de módulos.
- [ ] Criar checklist de deploy.
- [ ] Criar padrão de issues e pull requests.

## Fase 2 — Qualidade

- [ ] Rodar testes existentes.
- [ ] Identificar falhas críticas.
- [ ] Criar GitHub Actions mínimo.
- [ ] Adicionar análise de segurança de dependências.
- [ ] Adicionar lint/format quando aplicável.

## Fase 3 — Agentes

- [ ] Criar especificação do agente financeiro.
- [ ] Criar especificação do agente operacional.
- [ ] Criar especificação do agente jurídico/documental.
- [ ] Criar especificação do agente GoldFinder.
- [ ] Criar gateway seguro para modelos de IA.

## Fase 4 — Produção controlada

- [ ] Ambiente de staging.
- [ ] Logs centralizados.
- [ ] Backup.
- [ ] Monitoramento.
- [ ] Controle de acesso.
- [ ] Plano de rollback.

## Riscos atuais

- Repositório público.
- Base possivelmente derivada de LiteLLM.
- Tamanho grande do repositório.
- Necessidade de auditoria antes de usar em produção.

## Próxima ação recomendada

Fazer auditoria de segurança e inventário técnico antes de qualquer integração com dados reais do Grupo Maverick.
