# Terra Nobre — Imóveis de Caráter

> *"Onde a terra conta uma história."*

![Terra Nobre Preview](https://img.shields.io/badge/status-portfolio%20project-c4956a?style=flat-square&labelColor=2e2118)
![HTML](https://img.shields.io/badge/HTML-single%20file-6b7c5c?style=flat-square&labelColor=2e2118)
![CSS](https://img.shields.io/badge/CSS-inline-9b6a3e?style=flat-square&labelColor=2e2118)
![JS](https://img.shields.io/badge/JS-vanilla-c4956a?style=flat-square&labelColor=2e2118)

---

## A História por Trás do Projeto

Tudo começa com uma pergunta simples: **o que faz um imóvel ser verdadeiramente especial?**

Não é o preço. Não é a metragem. É o que ele carrega — a luz que entra pela janela às sete da manhã, o cheiro de madeira velha no corredor, a pedra que guarda o calor do sol de inverno. É a *alma* do lugar.

A **Terra Nobre** nasceu como um exercício criativo de design para portfólio, mas rapidamente se tornou algo mais: uma exploração sobre como uma marca imobiliária de luxo *deveria* se apresentar ao mundo — não com frieza corporativa, mas com calor, textura e intenção.

---

## O Briefing Imaginário

**Cliente fictício:** Terra Nobre Imóveis  
**Fundação:** 2011, Belo Horizonte — MG  
**Posicionamento:** Curadoria de propriedades com caráter histórico e arquitetônico singular  
**Público:** Compradores de alto padrão que valorizam autenticidade acima de ostentação  
**Problema:** As grandes imobiliárias tratam imóveis como produtos. A Terra Nobre trata como patrimônio.

O desafio de design era claro: criar uma identidade visual que comunicasse **luxo orgânico** — nem fria como o mármore branco dos concorrentes, nem rústica demais a ponto de perder sofisticação. O ponto de equilíbrio entre uma fazenda centenária e um editorial da Apartamento Magazine.

---

## Decisões de Design

### Paleta de cores — A terra como paleta

Cada cor foi escolhida a partir de elementos naturais:

| Variável | Hex | Inspiração |
|----------|-----|------------|
| `--sand` | `#F2EAD8` | Areia de rio seco |
| `--clay` | `#C4956A` | Argila úmida |
| `--clay-dk` | `#9B6A3E` | Barro cozido |
| `--earth` | `#5C4033` | Terra húmus |
| `--moss` | `#6B7C5C` | Musgo em pedra |
| `--bark` | `#2E2118` | Casca de peroba |
| `--cream` | `#FAF6EE` | Papel de carta antigo |

### Tipografia — Três vozes distintas

A hierarquia tipográfica foi construída para três "vozes" diferentes dentro da marca:

- **Fraunces** *(display)* — A voz da marca. Óptica variável, serifada, levemente melancólica. Usada em headlines e números grandes.
- **Cormorant Garamond** *(corpo)* — A voz do narrador. Elegante, leve, com ascendentes generosas. Usada em textos corridos e subtítulos.
- **DM Sans** *(UI)* — A voz funcional. Limpa, sem serifa, neutra. Usada em labels, botões e navegação.

### Ilustrações SVG — Artesanato em código

Em vez de fotografias de stock (que soam genéricas), todas as imagens da página são **ilustrações arquitetônicas desenhadas em SVG puro** — diretamente no código. Cada uma representa um tipo de propriedade do portfólio fictício:

1. **Fazenda Mata Branca** — Propriedade rural com montanhas ao fundo e lua cheia
2. **Casa Serra Verde** — Residência moderna com piscina no jardim
3. **Solar dos Arcos** — Solar colonial do século XVIII com arcadas
4. **Loft Armazém 7** — Loft industrial em Vila Madalena
5. **Chalé Pedra Branca** — Chalé serrano com jardim florido

Essa escolha não é apenas estética — é uma demonstração de habilidade técnica: provar que é possível criar atmosfera e beleza sem depender de assets externos.

### Textura de granulado

A sobreposição de ruído SVG (`feTurbulence`) em toda a página cria uma sensação de impressão em papel — como uma revista de arquitetura de qualidade. É sutil, mas muda completamente como o olho percebe as superfícies.

---

## Estrutura da Página

```
terra-nobre/
│
├── index.html          ← Página principal (arquivo único autocontido)
├── README.md           ← Este arquivo
└── deploy.sh           ← Script de publicação no GitHub Pages
```

### Seções

| Seção | Propósito |
|-------|-----------|
| **Nav** | Navegação fixa com blend-mode e scroll freeze |
| **Hero** | Headline + estatísticas + ilustração de mansão + cursor customizado |
| **Features** | 6 diferenciais competitivos com ícones SVG orgânicos |
| **Gallery** | Grid editorial 2×2+1 com 5 propriedades fictícias |
| **FAQ** | Acordeão interativo com ilustração botânica decorativa |
| **CTA** | Captura de lead com validação e feedback visual |
| **Footer** | Rodapé minimalista |

---

## Interações & Animações

- **Cursor personalizado** — substitui o cursor padrão por um ponto em argila que expande em elementos interativos
- **Scroll reveal** — `IntersectionObserver` com delays escalonados por seção
- **Nav adaptativa** — transparente no topo, congela com `backdrop-filter: blur` ao rolar
- **Gallery hover** — zoom suave na imagem + overlay com nome e localização
- **FAQ accordion** — abertura/fechamento com `max-height` animado e rotação de ícone
- **CTA feedback** — botão muda de cor e texto após envio

---

## Como Rodar Localmente

```bash
# Clone o repositório
git clone https://github.com/SEU_USUARIO/terra-nobre.git

# Entre na pasta
cd terra-nobre

# Abra no navegador (qualquer um destes)
open index.html
# ou
python3 -m http.server 8080
# depois acesse http://localhost:8080
```

Não há dependências, build steps ou package managers. É um único arquivo HTML.

---

## Publicar no GitHub Pages

```bash
# Torne o script executável e rode
chmod +x deploy.sh
./deploy.sh
```

O script cria o repositório, faz o commit inicial e ativa o GitHub Pages automaticamente.

---

## Referências de Inspiração

- [Lapa Ninja](https://www.lapa.ninja/) — Curadoria de landing pages de referência mundial
- [House of Honey](https://www.houseofhoney.com/) — Estúdio de interiores californiano
- [Frequency Breathwork](https://frequencybreathwork.com/) — Paleta orgânica e tipografia expressiva
- Revistas: *Apartamento*, *Cabana*, *Kinfolk*

---

## Sobre este Projeto

Este projeto faz parte de um portfólio de landing pages fictícias criadas para demonstrar habilidades em:

- Design de identidade visual coesa
- Tipografia editorial
- Ilustração técnica em SVG
- CSS avançado (variáveis, animações, blend modes, backdrop-filter)
- JavaScript vanilla sem dependências
- UX writing em português

---

*Feito com cuidado e muita serifa. Nenhum imóvel foi vendido na produção deste projeto.*
