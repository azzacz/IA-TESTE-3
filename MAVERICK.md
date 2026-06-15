# MAVERICK AI OPERATING RULES

Este repositório faz parte do ecossistema técnico Maverick. O objetivo deste arquivo é servir como memória operacional para agentes de IA, automações, revisores de código e futuras sessões de desenvolvimento.

## 1. Princípios centrais

1. Segurança acima de velocidade.
2. Código deve ser rastreável, revisável e reversível.
3. Nunca remover logs, auditoria ou validações sem justificativa técnica.
4. Nunca inserir chaves, senhas, tokens ou dados pessoais reais no repositório.
5. Toda alteração relevante deve ter plano de rollback.
6. Preferir arquitetura simples, modular e auditável.
7. Evitar gambiarra invisível. Se houver atalho, documentar.
8. Respostas e commits devem priorizar produção, não demonstração.

## 2. Contexto estratégico

Projetos Maverick podem envolver:

- ERP para posto de combustível;
- automação operacional;
- fiscalização de NFC-e e cancelamentos;
- monitoramento remoto;
- IA corporativa;
- análise financeira;
- GoldFinder/geotecnologia;
- clínica/saúde;
- agropecuária.

Este repositório deve ser tratado como base experimental para agentes de IA, gateway de modelos, automações e integração futura com módulos internos.

## 3. Padrão técnico preferencial

Quando aplicável, priorizar:

- Python 3.11+;
- FastAPI para serviços HTTP;
- PostgreSQL para persistência;
- Redis para filas/cache quando necessário;
- Docker Compose para ambiente local;
- GitHub Actions para CI;
- testes automatizados antes de deploy;
- variáveis de ambiente via `.env.example`, nunca `.env` real.

## 4. Segurança obrigatória

Nunca commitar:

- `.env` real;
- token GitHub;
- API key OpenAI/Anthropic/Groq/Gemini/etc.;
- senha de banco;
- certificado fiscal;
- chave privada;
- arquivo de backup com dados reais;
- dados de clientes, pacientes, funcionários ou fornecedores.

Toda nova integração deve prever:

- autenticação;
- controle de permissões;
- logs;
- rate limit quando exposta à internet;
- tratamento de erro sem vazamento de segredo;
- documentação mínima.

## 5. Regras para agentes de IA

Antes de alterar código, o agente deve:

1. Ler este arquivo.
2. Ler `AGENTS.md` se existir.
3. Verificar `SECURITY.md`.
4. Identificar stack do projeto.
5. Procurar arquivos de configuração.
6. Evitar alterações destrutivas.
7. Preferir branch/PR para mudanças grandes.

O agente deve produzir respostas com:

- resumo do que mudou;
- riscos;
- como testar;
- próximos passos.

## 6. Padrão de commits

Usar commits semânticos:

- `docs:` documentação;
- `feat:` funcionalidade;
- `fix:` correção;
- `refactor:` refatoração;
- `security:` melhoria de segurança;
- `test:` testes;
- `chore:` tarefas internas.

Exemplos:

- `docs: add Maverick AI operating rules`
- `security: add secret scanning checklist`
- `feat: add agent configuration baseline`

## 7. Roadmap inicial

Prioridade 1:

- criar documentação base;
- mapear estrutura real do repositório;
- identificar riscos de segurança;
- padronizar `.env.example`;
- criar checklist de auditoria.

Prioridade 2:

- configurar CI;
- criar testes mínimos;
- organizar scripts;
- preparar ambiente Docker.

Prioridade 3:

- integrar agentes;
- criar automações;
- separar módulos Maverick;
- preparar deploy controlado.

## 8. Nota importante

Este repositório é público. Portanto, qualquer informação sensível deve ficar fora daqui. Para projetos privados do Grupo Maverick, criar repositório privado separado e aplicar as mesmas regras com controle de acesso mais rigoroso.
