# AGENTS.md

Instruções para agentes de IA trabalhando neste repositório.

## Missão

Ajudar a transformar este repositório em uma base segura, organizada e útil para automações Maverick, agentes de IA e experimentos controlados.

## Antes de trabalhar

Leia, nesta ordem:

1. `MAVERICK.md`
2. `SECURITY.md`
3. `README.md`
4. arquivos de configuração relevantes

## Modo de operação

Ao modificar o projeto:

1. Entenda a stack antes de alterar.
2. Não apague arquivos grandes sem confirmação.
3. Não simplifique segurança.
4. Não exponha segredo.
5. Prefira mudanças pequenas e rastreáveis.
6. Documente o motivo da alteração.
7. Informe como testar.

## Saída esperada do agente

Toda entrega deve conter:

- o que foi alterado;
- por que foi alterado;
- risco operacional;
- como testar;
- próximos passos.

## Padrão de segurança

Proibido:

- credenciais reais;
- dados pessoais reais;
- logs sensíveis;
- certificados;
- dumps de banco;
- comandos destrutivos sem alerta.

Obrigatório:

- validação de entrada;
- tratamento de erro;
- logs úteis;
- rollback quando possível;
- testes quando aplicável.

## Prioridade de trabalho

1. Segurança.
2. Organização.
3. Documentação.
4. Testes.
5. Funcionalidade.
6. Performance.

## Áreas Maverick futuras

Este repositório poderá apoiar:

- gateway de LLMs;
- agentes financeiros;
- agentes operacionais;
- auditoria de NFC-e;
- monitoramento remoto;
- GoldFinder;
- clínica;
- agro.

## Regra final

Se houver dúvida entre fazer rápido e fazer seguro, faça seguro.
