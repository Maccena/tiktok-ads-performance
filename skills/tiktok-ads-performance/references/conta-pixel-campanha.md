# Conta, Pixel e estrutura da campanha (Módulo 03)

Esta é a base extraída das aulas D10 a D15. A notação de citação está em [fontes.md](fontes.md).
Rótulos usados neste arquivo:
- **[REGRA DO CURSO]**: o professor apresenta como procedimento padrão.
- **[PREFERÊNCIA DO PROFESSOR]**: opinião ou estilo pessoal declarado.
- **[EXEMPLO]**: valor usado numa demonstração.

---

## 1. Criação da conta (D10)

1. Acesse `ads.tiktok.com` e clique em "começar" para criar a conta com e-mail e senha. Depois
   confirme o código enviado por e-mail (D10 @00:38, D10 @01:06).
2. **Nome da empresa:** use o nome da loja. Não precisa de CNPJ, pode ser pessoa física. O website
   é opcional. Indústria: e-commerce → "Outros" (D10 @01:20).
3. **Região, moeda e fuso:** Brasil, BRL, horário de São Paulo. Informe um telefone para receber SMS
   (D10 @01:42).
4. **CPF ou CNPJ:** se você tiver CNPJ, o professor recomenda usá-lo. Se não, use o CPF (D10 @02:01).
5. **Pagamento automático por cartão de crédito** [REGRA DO CURSO]. Ele não recomenda conta manual
   (pré-paga): se a conta for bloqueada, o saldo injetado se perde. No cartão, o valor é estornado
   na fatura (D10 @02:18). D11 @01:18 repete a recomendação de método automático.
6. **Verificar o telefone também em User Settings**, com o mesmo número do cadastro, "para passar
   mais credibilidade ao TikTok" (D10 @02:52–03:30).

## 2. Verificação e aprovação (D11)

- Use um número de celular e um e-mail válidos e acessíveis para receber códigos (D11 @00:13).
- Envie os dados (CPF/CNPJ, endereço) e **espere a aprovação**. Pode levar até **2 dias úteis**
  (D11 @00:43).
- Status da conta: `Tools → Account setup`. Os status são *Under Review*, *Approved* ou
  desaprovada. Se a conta for desaprovada, envie os documentos que comprovem a titularidade do
  CPF/CNPJ (D11 @01:46–02:20).
- O professor prefere **não subir campanhas enquanto a conta estiver em análise**, mesmo podendo
  adicionar o pagamento antes (D11 @02:03) [PREFERÊNCIA DO PROFESSOR].
- *Não incorporado:* a dica de "aquecer o navegador" para "estabelecer comportamento de usuário
  real" (D11 @00:53). Veja [escopo-excluido.md](escopo-excluido.md).

## 3. Maturação da conta (D13; reforçada em D18 e D25)

- **O que é:** deixar a conta "descansando" depois de criada, sem subir campanhas nem mexer muito,
  para a plataforma não a tratar como possível ameaça (D13 @01:00–01:30).
- **Por quanto tempo:** "pelo menos **3 dias**", que é "o tempo ideal" segundo o professor
  (D13 @02:00). Em D25 @03:39 ele fala em "pelo menos **uma semana**". Isso é uma
  **contradição**: veja [conflitos-e-lacunas.md](conflitos-e-lacunas.md).
- Durante a maturação, pode entrar de vez em quando no dashboard e navegar pela interface
  (D13 @02:00).
- **Campanha de aquecimento (D15 @01:43):** antes da campanha de conversão, ele sobe uma campanha
  de **visualização de vídeo** e recomenda gastar **pelo menos R$ 15**, "para o TikTok fazer a
  primeira cobrança e não derrubar sua conta". No exemplo, gastou R$ 25 e depois desativou.

## 4. Pixel (D12)

**Para que serve, segundo o curso (D12 @00:29):** criar públicos personalizados a partir do
comportamento no site, fazer remarketing e otimizar campanhas com os dados coletados.

**Passo a passo demonstrado:**
1. `Criar anúncio → Avançado → objetivo Website Conversions (Conversão no website)`. Não publique
   a campanha: use a tela só para criar o pixel (D12 @01:24–01:47).
2. `Data connection → criar novo`. Confirme a identidade por e-mail ou telefone (D12 @01:47–02:07).
3. `Conectar dados → Web → Next` → **conexão manual** [REGRA DO CURSO]. Ele diz para nunca conectar
   via parceiro, como o app do TikTok na Shopify (D12 @02:17). O motivo declarado é de
   "contingência": evitar que a conta fique "marcada".
4. Dê um nome ao pixel e crie os eventos de conversão: **Complete Payment**, **Add to Cart** e
   **View Content** (D12 @02:36–02:53). Método: **Event Builder** (D12 @03:00).
5. Copie o **ID do pixel**, aquele código de letras e números (D12 @03:13, D12 @03:49).
6. Cadastre o pixel no **checkout** (no exemplo, a plataforma "IAMP", provavelmente Yampi):
   `Marketing → Pixels → novo → serviço TikTok`, informando nome e ID. Na configuração dele:
   boleto **não**, PIX **sim**, PIX parcelado **sim**, sem filtrar produtos (D12 @04:00–04:31)
   [EXEMPLO / PREFERÊNCIA DO PROFESSOR]. Ele não instala o código na Shopify (D12 @03:13).
7. Gere um pedido de teste (PIX ou boleto) na loja, para o evento disparar. Depois clique em
   *Refresh* na tela do pixel: o evento aparece "em questão de minutos" (D12 @04:31–04:56).

**Não coberto pelo curso:** Events API (server-side), deduplicação de eventos, parâmetros de valor
e moeda, verificação pelo Pixel Helper, eventos para infoproduto. Veja
[conflitos-e-lacunas.md](conflitos-e-lacunas.md).

## 5. ABO x CBO (D14; preferência reforçada em D17)

| | ABO | CBO |
|---|---|---|
| Onde fica o orçamento | No **conjunto de anúncios** (D14 @01:24) | Na **campanha** (D14 @01:33) |
| Exemplo do curso | 5 conjuntos × R$ 20 = R$ 100/dia (D14 @01:27) | Campanha de R$ 100: o TikTok distribui, e um conjunto pode gastar 30 e outro 5 (D14 @01:33–01:46) |
| Manutenção | Manual: você corta e otimiza (D14 @01:56) | Automática, feita pela plataforma (D14 @02:03) |
| Quando usar (curso) | Mais controle, ajustes frequentes, **campanhas de teste**, testar públicos e criativos (D14 @02:45) | Eficiência, grande escala, quando você confia nos conjuntos (D14 @02:54) |

- **[PREFERÊNCIA DO PROFESSOR]** Ele usa **ABO** "porque tenho mais controle sobre as métricas"
  (D14 @02:08). Em D17 @01:38 diz que "o resultado das campanhas ABO tem **50% de culpa sua**", e
  o restante é entrega da plataforma.
- O próprio curso conclui que "a escolha certa pode variar de acordo com a situação" (D14 @03:03).
  Por isso, não trate ABO como regra universal.
- *Nota terminológica:* o professor expande ABO como "Otimização de Orçamento de Leilão"
  (D14 @00:26). Veja [notas-externas.md](notas-externas.md).

## 6. A campanha "80/20" de conversão (D15) — procedimento central

O professor a chama de estratégia "validada", que serve "para quem tem de R$ 200 a R$ 20 mil"
(D15 @00:28–00:43). A aula foi regravada porque a interface muda (D15 @00:51).

**Pré-requisitos:** conta verificada (e-mail e telefone), maturada, com campanha de aquecimento já
feita (D15 @01:43). Pixel com Complete Payment (D15 @02:50). Criativo pronto, segmentado pela
persona (D15 @01:08–01:32).

**Nível de campanha**
1. `Create → Conversão → Website conversions` (D15 @02:09–02:25).
2. **Nome:** ele não renomeia. Organiza-se pelo nome automático (data e hora; as duplicatas
   recebem "copy", "/2") (D15 @02:25–02:47) [PREFERÊNCIA DO PROFESSOR].
3. **Orçamento:** ABO, isto é, no conjunto (ver seção 5).

**Nível de conjunto de anúncios**
4. **Evento de otimização:** pixel → **Complete Payment** (D15 @02:50).
5. **Posicionamentos** (D15 @03:15–04:13): troque *Automatic Placement* por *Select placement*.
   - **Remova CapCut e Fizzo**: "pesam muito na conversão", e as pessoas não compram por lá.
   - **Mantenha TikTok e Pangle.** Pangle "é 8 ou 80": ou vende muito, ou nada. No **primeiro teste
     ele deixa o Pangle ativo** para medir, e já viu "40, 50% das conversões" virem dele. Se o
     Pangle não converter, **remova-o nas duplicatas**.
6. **Segmentação** (D15 @04:13–05:57) [REGRA DO CURSO]:
   - **Não use interesses**: "quanto mais a gente segmenta, mais caro fica".
   - **Idade:** padrão **18–54**. Para produto de público muito jovem, **18–24**.
   - **Gênero:** só restrinja se o produto for claramente de nicho (masculino ou feminino).
   - Idioma e dispositivo (Android/iOS): não mexe.
   - A segmentação real acontece no **criativo**, via persona (D03; ver
     [produtos-e-criativos.md](produtos-e-criativos.md)).
7. **Orçamento "quebrado"** (D15 @05:57–06:57) [PREFERÊNCIA DO PROFESSOR, apresentada como "segredinho"]:
   - Use valores com final **9 ou 7**. Exemplos: quer R$ 30? Ponha **R$ 39**. Quer 50? Ponha
     **59, 57 ou 54**.
   - Justificativa declarada: "ficar em cima da faixa de leilão" de concorrentes iniciantes. Isso é
     uma **hipótese do professor**: o curso não mostra teste comparativo.
8. **Dayparting** (D15 @06:57–08:28) [REGRA DO CURSO, "80/20 das minhas campanhas"]:
   - Em *Programação*, escolha "selecionar um período específico" e marque **05:00–12:30** e
     **15:30–23:00** (no áudio: "das 5 até meio-dia, meio-dia e meio... a partir das 3h30 até umas
     10h30, 11h no máximo").
   - Motivo: de madrugada o orçamento é gasto com quem não compra. No exemplo de R$ 39, "sobrariam
     uns R$ 15" para o resto do dia (D15 @07:54).
   - Não preencha mais nada nas opções avançadas (D15 @08:42).

**Nível de anúncio**
9. **Identidade:** use uma página/perfil do TikTok por nicho (exemplos: "Dicas da Kari" para
   produtos femininos, "Dicas do Márcio" para masculinos, ou o nome da loja), ou Spark Ads
   (D15 @08:46–09:15) [EXEMPLO].
10. Faça o upload do criativo e confira a pré-visualização (D15 @09:15).
11. **Texto do anúncio:** ele sempre coloca só **um ponto (".")**. Diz que o texto não performa
    pior, mas que "qualquer palavrinha que a gente descuide das políticas, o TikTok pode ficar em
    cima" (D15 @09:34–10:11) [PREFERÊNCIA DO PROFESSOR]. A skill trata isso como escolha de estilo
    e **não** como forma de driblar a revisão. Veja SKILL.md, "Limitações e cuidados".
12. **URL** de destino: a página do produto (D15 @10:14). Depois, publique.

Ele afirma que a estrutura "serve para qualquer tipo de operação", loja ou infoproduto
(D15 @10:22). Só o caso de loja/e-commerce é demonstrado.
