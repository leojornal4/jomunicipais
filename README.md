# JOM Completo

Este projeto é uma aplicação Next.js.

## Requisitos
- Node.js LTS (instalado)
- npm 10+
- Opcional: pnpm

## Instalação
No PowerShell:

```
npm install --legacy-peer-deps
```

> Observação: há um conflito de peer dependencies (React 19 vs alguns pacotes). O parâmetro `--legacy-peer-deps` resolve a instalação.

## Desenvolvimento
Inicie o servidor de desenvolvimento:

```
npm run dev
```

A aplicação ficará disponível em:
- `http://localhost:3000`
- (rede local) `http://<seu-ip-local>:3000`

## Build e Produção
Crie o build de produção:

```
npm run build
```

Execute o servidor de produção:

```
npm run start
```

## Dicas de Ambiente (Windows)
Se o comando `npm`/`node` não for reconhecido em novos terminais, adicione `C:\Program Files\nodejs` ao PATH do usuário. Já foi configurado automaticamente, mas você pode verificar nas Variáveis de Ambiente.

## Observações
- Há 1 vulnerabilidade moderada reportada por `npm audit`. Para tentar corrigir:

```
npm audit fix --force
```

- O projeto possui `pnpm-lock.yaml`; caso opte por usar `pnpm`, instale-o globalmente e rode:

```
pnpm install --no-frozen-lockfile
pnpm dev
```