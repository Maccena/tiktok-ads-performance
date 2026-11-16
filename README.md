# TikTok Ads Performance — skill para Claude

Skill que orienta campanhas de TikTok Ads com base no curso de TikTok Ads de **Caio Dlugosz**.
Ela cobre:

- criação e aprovação da conta, instalação do Pixel e a campanha de conversão do curso;
- estrutura ABO/CBO, segmentação, posicionamentos, orçamento e dayparting;
- escolha de produtos e criativos UGC;
- leitura de métricas (CPA, CTR, CPM, CPC, ROAS), faixa de corte, duplicação e escala;
- diagnóstico de queda de vendas e saturação de criativos.

Cada orientação cita a aula e o minuto de origem (ex.: `D15 @05:57`) e vem marcada como
regra do curso, preferência do professor ou exemplo. Conhecimento de fora do curso aparece
separado, com o rótulo "(fora do curso)".

## Instalação

### Claude Code (recomendado)

Dentro do Claude Code, rode:

```
/plugin marketplace add Maccena/tiktok-ads-performance
/plugin install tiktok-ads-performance@tiktok-ads-performance
```

Para atualizar depois: `/plugin marketplace update tiktok-ads-performance`.

### claude.ai e app desktop do Claude

1. Baixe `tiktok-ads-performance.zip` na [página de releases](https://github.com/Maccena/tiktok-ads-performance/releases/latest).
2. No Claude, abra **Customize > Skills** e envie o arquivo `.zip`, sem descompactar.

### Cópia manual

Copie a pasta `skills/tiktok-ads-performance/` para `~/.claude/skills/` (vale para todos os
projetos) ou para `.claude/skills/` dentro de um projeto.

## Como usar

A skill é ativada sozinha quando o assunto é TikTok Ads, por exemplo: "monta a campanha para
um organizador de maquiagem" ou "meu CPA está em R$ 22, corto o conjunto?". Traga os números
do gerenciador (gasto, compras, CTR, CPM) para receber uma decisão por conjunto.

## Limites

- A fonte é um único curso, gravado por volta de 2024. A interface do TikTok pode ter mudado.
- O curso não traz valores de referência para CTR, CPM ou ROAS, e a skill não inventa esses números.
- O módulo de "contingência" do curso (proxy, multilogin, fingerprint, metadados) **não** foi
  incorporado, porque serve para driblar a fiscalização da plataforma. O motivo está em
  `skills/tiktok-ads-performance/references/escopo-excluido.md`.
- As transcrições integrais das aulas não fazem parte deste repositório. A skill funciona só
  com os arquivos de referência.

## Créditos

Método e conteúdo de origem: curso de TikTok Ads de **Caio Dlugosz**. Esta skill é um resumo
organizado, com citações, e não substitui o curso.
