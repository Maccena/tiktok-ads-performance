# Métricas, otimização, escala e saturação (Módulo 04)

Base extraída das aulas D17 a D21. A notação de citação está em [fontes.md](fontes.md).

## 1. Métricas que o curso usa (D17)

| Métrica | Definição dada no curso | Leitura sugerida no curso |
|---|---|---|
| **CPA** | custo por aquisição/conversão | **Métrica principal.** CPA alto indica que a campanha não performa (D17 @00:39) |
| **CTR** | % de quem vê o anúncio e clica | CTR baixo sugere criativo pouco atraente (D17 @00:50) |
| **CPM** | custo por mil impressões | eficiência do gasto (D17 @01:02) |
| **CPC** | custo por clique | métrica secundária (D17 @02:03) |
| **ROAS** | valor gerado por unidade gasta | só é definido; o curso não dá meta numérica (D17 @01:14) |

**Hierarquia de análise** [REGRA DO CURSO] (D17 @02:13):
> "Aqui a gente não faz uma análise por métricas igual a do Facebook. Eu analiso a métrica mais
> importante primeiro, que é o CPA […] E aqui analisamos as outras métricas como secundárias."

O curso **não fornece benchmarks** de CTR, CPM ou CPC (nenhum valor "bom" ou "ruim"). A skill não
deve inventar esses valores. Veja [conflitos-e-lacunas.md](conflitos-e-lacunas.md).

## 2. Faixa de corte (D17, D18, D19, D21)

Estratégia atribuída pelo professor a si mesmo (D17 @03:06; D21 @00:24).

**Corte de conjuntos sem venda** (D17 @02:28–03:13):
- Conjunto que **gastou R$ 15 sem nenhuma compra** → **excluir**.
- Se **CTR e CPM estiverem bons e a loja recebe visitas**, a faixa de corte **sobe para R$ 20**.
- Conjuntos que venderam → **duplicar**.

**CPA máximo/ideal** (D18 @00:57; D18 @02:20):
- Conjunto "bom" é o que tem **CPA ≤ R$ 15**.
- Se um conjunto que vendia **estourar o CPA máximo** ("15, 20 reais") e parar de vender, exclua
  "por mais que tenha saído venda dela". Não tenha dó: "outras campanhas boas vão nascer".

**Variação nos números:** na demonstração de D19, a faixa de corte citada é **R$ 25**
(D19 @03:22) e os conjuntos são excluídos "depois de gastos R$ 20, 25" (D19 @07:08). Isso
aparece numa conta que rodava "para fora", em dólar. Veja
[conflitos-e-lacunas.md](conflitos-e-lacunas.md).

**Excluir, não desativar** [REGRA DO CURSO] (D19 @06:38): "Eu não desligo os conjuntos porque em
escala no TikTok Ads, se você desativa uma campanha ou um conjunto, ele continua gastando. Pode
gastar ali R$ 0,10, R$ 1, R$ 10." *(Afirmação do professor, não verificada.)*

**Frequência:** monitore diariamente, porque as métricas "podem mudar rapidamente" (D17 @03:30).
Teste criativos continuamente (D17 @03:37).

## 3. Rotina de manutenção e pré-escala (D18)

1. Depois do primeiro teste, **corte** os conjuntos ruins e **mantenha** os de CPA < 15 (D18 @00:57).
2. **Duplique sutilmente** os conjuntos bons. "Duplicar exageradamente pode derrubar a conta"
   (D18 @01:04).
   - **[EXEMPLO]** Dos 5 conjuntos, 2 têm CPA < 15. Exclua os 3 ruins e duplique cada bom
     **2 vezes**, ficando com 4 conjuntos novos (D18 @01:16–01:29).
3. Nas duplicatas, use **orçamento quebrado** (R$ 29, 59, 79, ou final 7; "se quiser testar 44,
   33, fica a seu critério") (D18 @01:38–02:11).
4. **Repita uma vez ao dia**, sem duplicar mais conjuntos, "prezando pela maturação da conta"
   (D18 @02:36–02:55).
5. Depois de **2 a 3 dias** de teste e pré-escala, aumente para **3 duplicações por conjunto**,
   "não muito mais do que isso" (D18 @02:55–03:04).

## 4. Alavancagem / escala (D19)

**Cinco passos** (D19 @00:28–02:25):
1. **Comece com pouco**: é possível começar "com R$ 100 ou até menos".
2. **Identifique os conjuntos promissores** (muitas conversões, CPA muito baixo) e **aumente o
   orçamento gradualmente**, monitorando.
3. **Ajuste o investimento** de forma gradual. Na prática: **duplique os vencedores e aumente o
   orçamento nas duplicatas**, preservando o original.
4. **Melhore os criativos**: "é a qualidade do criativo que vai determinar o sucesso". Use pessoas
   reais, UGC e depoimentos de clientes satisfeitos.
5. **Monitore idade, gênero, localização e dispositivo** de quem converte e ajuste a segmentação.
   [EXEMPLO] "se perceber que mulheres de 45 a 54 anos estão comprando mais, ajuste suas campanhas
   para focar nesse grupo".

**Caso real demonstrado** (D19 @03:07–07:25), numa conta já bloqueada que rodava fora do Brasil
e gastou US$ 122:
- Uma campanha teve 14 conversões com CPA de ~US$ 2 (cerca de R$ 11, com faixa de corte de R$ 25).
- Outra teve 49 conversões num único conjunto, em uma semana. Os valores de CPA citados
  **variam na fala** (12 centavos, 50–60 centavos, 3 dólares, 3 centavos). Use só como ilustração
  qualitativa.
- O que ele faria com o vencedor: **duplicar ao menos 3 vezes** e mudar o orçamento das cópias
  para faixas como 29 → 39 → 59 (D19 @04:19–05:12).
- Conjuntos com 5 e 6 conversões (CPA de US$ 1,50 e US$ 1,58) e orçamento de US$ 20,99:
  **duplicar 2 vezes cada**, com orçamentos de US$ 27 e US$ 29,99, "trocando sempre o quebrado
  final" (D19 @05:38–06:38).
- Cópias que não vendem e já gastaram → **selecionar e excluir** (D19 @06:38).
- Cópia que vendeu com CPA de 87 centavos → **duplicar de novo** (D19 @07:08).

## 5. Saturação (D20)

**Definição:** criativo ou produto exibido muitas vezes ao mesmo público, com queda de
engajamento e de conversão (D20 @00:24).

**Sinais** (D20 @00:38–01:04):
- **CTR em queda**;
- **CPA subindo**;
- **conversões caindo mesmo com mais investimento**.

**Tempo de vida de um criativo** [AFIRMAÇÃO DO PROFESSOR, sem demonstração]: **3 a 5 dias, no máximo
uma semana** (D20 @02:52).

**Diagnóstico "vendia e parou de um dia para outro"** (D20 @01:39–03:31). O curso diz que isso "é
normal no TikTok Ads" e propõe três ações:
1. **Melhorar a oferta**: trocar palavras-chave na copy, na página de vendas ou no criativo. Vale
   checar se a venda não foi "um dia de sorte".
2. **Trocar a comunicação com o público**. [EXEMPLO] As vendas vieram de público jovem, mas quem
   parou no criativo foi um público mais velho, e o TikTok passa a entregar para os mais velhos.
   Mude a forma de falar, de apresentar e de começar o vídeo.
3. **Trocar o criativo**, inteiro ou só os segundos iniciais, a narração ou a oferta.

Depois, volte à **"estaca zero"**: o produto já está validado, mas os novos testes recomeçam
"devagar, sem pressa e com poucos conjuntos" (D20 @03:24–03:55).
