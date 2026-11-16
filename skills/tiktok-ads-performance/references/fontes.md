# Fontes — mapa das aulas e notação de citação

Toda afirmação da skill aponta para uma aula no formato **`Dxx @mm:ss`**: aula `video_Dxx`, a partir
da marcação de tempo indicada (início do segmento da transcrição em que a fala aparece).

- Transcrição legível: `Transcricoes/<Módulo>/video_Dxx.md`
- Dados brutos (segmentos, tempos, parâmetros): `Transcricoes/<Módulo>/video_Dxx.json`
- Índice geral: `Transcricoes/INDICE.md` · Inventário: `Transcricoes/inventario.csv`
- Vídeo original: `Curso/<Módulo>/video_Dxx.mp4`

## O curso

Um único curso ("trilha de TikTok Ads"), de um único professor, que se apresenta como **Caio**,
"convidado pela FNM como expert em TikTok Ads" (D01 @00:28). São 5 módulos e 29 aulas, com ~2h04min
no total. Os arquivos não trazem títulos de aula. Os títulos abaixo foram inferidos da fala de
abertura de cada vídeo.

| Aula | Módulo | Tema (inferido da fala) | Usada na skill |
|---|---|---|---|
| D01 | 01 Boas-vindas | Apresentação da trilha | contexto |
| D02 | 01 | Conhecendo o TikTok Ads: ecossistema, vantagens, FOMO | sim |
| D03 | 01 | "Segredo do TikTok": persona e segmentação no criativo | sim |
| D04 | 02 Produtos e Criativos | Produtos "TikTokáveis" e mineração (#TikTokMadeMeBuyIt) | sim |
| D05 | 02 | Mineração de criativos, biblioteca de anúncios de alta performance | sim (c/ ressalva) |
| D06 | 02 | UGC: conceito, comparação com anúncio comum, benefícios | sim |
| D07 | 02 | Como encontrar/produzir mídias UGC | sim |
| D08 | 02 | Edição de criativo no Clipchamp + narração com IA | sim (c/ ressalva) |
| D09 | 02 | Resumo do módulo 2 (estrutura de criativo) | sim |
| D10 | 03 Gerenciador | Criar conta no TikTok Ads | sim |
| D11 | 03 | "Fortalecendo sua conta": verificação, aprovação | parcial |
| D12 | 03 | Criação e configuração do Pixel | sim |
| D13 | 03 | Maturação da conta | sim |
| D14 | 03 | ABO x CBO | sim |
| D15 | 03 | **Subindo a 1ª campanha de conversão (aula "80/20")** | sim — central |
| D16 | 03 | Resumo do módulo 3 | contexto |
| D17 | 04 Análise e Escala | Decifrando métricas, faixa de corte | sim — central |
| D18 | 04 | Otimização e manutenção, duplicação, orçamento quebrado | sim — central |
| D19 | 04 | Alavancagem/escala, caso real de conta | sim — central |
| D20 | 04 | Saturação de criativos/produtos | sim |
| D21 | 04 | Resumo do módulo 4 | contexto |
| D22–D29 | 05 Contingência | Proxy, multilogin, fingerprint, metadados, evasão de bloqueios | **não** (ver [escopo-excluido.md](escopo-excluido.md)) |

## Qualidade das transcrições (ler antes de citar literalmente)

- Transcrição: `openai/whisper-large-v3` via API do OpenRouter, idioma fixado em `pt`, temperatura 0.
- Algumas grafias erradas são recorrentes. Leia sempre com esta correção:

| Na transcrição | Termo real (interpretação) |
|---|---|
| "inconformados" / "Falem conformados" / "Farem conformados" | "Fala, inconformados" (saudação) |
| "Pengo", "pingo", "pangol" | **Pangle** (rede de apps parceiros do TikTok) |
| "Fiso", "Fizz", "não fiz" | provavelmente **Fizzo**, posicionamento do TikTok Ads (interpretação; não confirmado no áudio) |
| "comprar payment", "a completa payment" | **Complete Payment** (evento de compra do Pixel) |
| "day party", "deipar", "dayparting" | **Dayparting** (programação por horário) |
| "IGC", "GC", "método GC" | **UGC** |
| "IAMP" | plataforma de checkout citada (provavelmente **Yampi**; interpretação) |
| "SnapTik/Snapchick" | site de download de vídeos do TikTok |
| "ROE" (D12 @00:54) | o professor fala de retorno sobre investimento (ROI) |

- Nos vídeos D13, D22, D24 e D26 os segmentos são longos (20–30 s), então a marcação de tempo é menos precisa.
- O serviço não devolve confiança por palavra, por isso não há palavras marcadas como `[?incerta?]`.
  Trechos de baixa confiança, quando houver, aparecem sinalizados no `.md`.
- Uma primeira versão de D06, D15 e D19 veio com acentos truncados por um dos provedores. Esses
  vídeos foram retranscritos e verificados. Um teste local com `large-v3-turbo` está em
  `Transcricoes/_teste_local/` e serve só como referência.
