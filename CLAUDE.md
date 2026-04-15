# CLAUDE.md — MARIAHELENAMISTURINHAS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** MARIAHELENAMISTURINHAS
**Nicho:** Cosméticos
**Keywords:** Trabalhando ha mais de 40 anos como manicure Maria Helena Soares sempre
**Paleta de cores:** violet | **Fonte:** poppins

Trabalhando há mais de 40 anos como manicure, Maria Helena Soares sempre gostou de desenvolver cores exclusivas para suas clientes. Nascida em Ijuí, no Rio Grande do Sul, Maria Helena adora viajar e observar tudo ao seu redor com o mesmo fascínio e entusiasmo com que faz suas misturinhas. Compondo cores obtidas através de quatro, seis e até oito nuances diferentes, a manicure é capaz de criar esmaltes apenas se inspirando em alguma coisa que viu por aí, ou mesmo a pedido das clientes. O que era somente um serviço exclusivo ganhou vida num projeto em parceria com Ruchelle Crepaldi – Maria Helena Misturinhas Limitadas, uma marca exclusiva de esmaltes que leva o conceito de “cores com história”. Cada coloração tem uma inspiração, que pode ser uma flor, uma paisagem ou um determinado universo – qualquer coisa que passe em frente aos olhos de Maria Helena e chame sua atenção. A produção de apenas 500 unidades por cor também garante a exclusividade das misturinhas. A fórmula foi desenvolvida levando em conta os desejos e necessidades de clientes e manicures. Com secagem rápida, cobertura perfeita e alta durabilidade, as misturinhas Maria Helena contam com o selo Tox Free, ou seja, não possuem toxinas como de DBP, tolueno e formoldeído, que são substituídas por resina mais natural. As pessoas mais sensíveis podem usar e abusar das misturinhas sem problema nenhum. As embalagens são um capricho à parte. Os pincéis, achatados e com cerdas chanfradas, são de altíssima qualidade e contam com uma tecnologia recém-chegada ao Brasil, que espalha melhor e oferece acabamento perfeito; a tampa é emborrachada para segurar melhor e bolinhas de inox garantem a homogeneidade do produto. Se tudo isso já não fosse suficiente, as embalagens ainda são retornáveis e recicláveis – saiba mais.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-J |
| Features | Features-B |
| About Section | About-C |
| Posts | Posts-C |
| Footer | Footer-H |
| Página Sobre | Sobre-G |
| Página Contato | Contato-G |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
