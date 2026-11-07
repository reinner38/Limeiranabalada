# Limeira na Balada — versão profissional

Portal de eventos, notícias e galerias para Limeira do Oeste - MG.

## Tecnologias
- Next.js
- TypeScript
- Supabase/PostgreSQL
- Supabase Storage
- Sharp para marca d'água nas fotos

## Instalação
1. Instale Node.js 20+
2. Rode `npm install`
3. Copie `.env.example` para `.env.local`
4. Crie um projeto no Supabase e preencha as chaves
5. Execute o SQL em `supabase/schema.sql`
6. Rode `npm run dev`

## Marca d'água
A rota `/api/watermark` recebe uma imagem e devolve uma versão com:
LIMEIRA NA BALADA
Limeira do Oeste - MG

na parte inferior da foto.

## Segurança
A autenticação administrativa deve usar Supabase Auth. Nunca coloque a
SERVICE_ROLE_KEY no navegador.
