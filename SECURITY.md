# Security Policy

## Regra de ouro

Este repositório é público. Não publique credenciais, dados pessoais, dados financeiros, dados fiscais, dados de pacientes, dados de funcionários, certificados, backups reais ou qualquer segredo operacional.

## Nunca commitar

- `.env` real;
- tokens de API;
- senhas;
- chaves SSH;
- certificados digitais;
- arquivos `.pfx`, `.pem`, `.key`, `.crt` privados;
- dumps de banco;
- planilhas internas;
- dados de clientes, pacientes, funcionários ou fornecedores;
- logs de produção com informações sensíveis.

## Variáveis de ambiente

Use apenas exemplos seguros em arquivos como:

```bash
.env.example
```

Exemplo permitido:

```bash
OPENAI_API_KEY=coloque_sua_chave_aqui
DATABASE_URL=postgresql://usuario:senha@localhost:5432/app
```

Exemplo proibido:

```bash
OPENAI_API_KEY=sk-chave-real
DATABASE_URL=postgresql://usuario:senha-real@host-real:5432/banco-real
```

## Checklist antes de cada commit

- [ ] Rodei busca por `sk-`, `token`, `password`, `secret`, `private_key`, `BEGIN PRIVATE KEY`.
- [ ] Não inclui `.env` real.
- [ ] Não inclui arquivos de backup.
- [ ] Não inclui dados pessoais reais.
- [ ] Não inclui certificado fiscal ou chave privada.
- [ ] A alteração tem rollback possível.

## Comandos úteis locais

```bash
git status
```

```bash
git diff --cached
```

```bash
grep -R "sk-\|token\|password\|secret\|BEGIN PRIVATE KEY" . --exclude-dir=.git
```

## Vulnerabilidades

Ao encontrar falha de segurança:

1. Não abrir issue pública com segredo exposto.
2. Remover o segredo do código.
3. Revogar a credencial no provedor.
4. Rotacionar nova credencial.
5. Revisar histórico do Git se necessário.

## Padrão para produção

Sistemas Maverick em produção devem usar:

- MFA;
- princípio do menor privilégio;
- logs de auditoria;
- backup testado;
- HTTPS;
- secrets fora do Git;
- revisão antes de deploy.
