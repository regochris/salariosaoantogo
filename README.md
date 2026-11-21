# SaláriosAO

Plataforma de inteligência salarial em Angola: salários por cargo, sector (público e privado) e província, a partir de partilhas anónimas, tabelas oficiais da função pública, dados de empresas e pesquisa própria.

## Stack

- Next.js (App Router) + TypeScript
- Tailwind CSS 4, com as cores e regras de `docs/DESIGN.md`
- Supabase (base de dados, contas e regras de acesso), a partir da fase 4
- Vercel (publicação)

## Começar

```bash
npm install
cp .env.example .env.local   # preencher na fase 4
npm run dev                  # http://localhost:3000
```

## Estrutura

```
app/          páginas (rotas)
components/   componentes partilhados (Header, BottomNav, Footer, SectorBar, ícones)
lib/          formatação e dados (provisórios até à fase 4)
docs/         DESIGN.md
```

## Regras

- Cores e tamanhos só através dos tokens (`bg-surface`, `text-muted`, `bg-primary`…), nunca valores soltos.
- Telemóvel primeiro; testar sempre com internet lenta.
- Nunca mostrar respostas individuais. Nome de empresa só com 5+ partilhas.
- Chaves e segredos só em variáveis de ambiente.
