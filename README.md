## Sobre o projeto

Este repositório documenta a criação de um caderno temático no **NotebookLM** sobre a cultura da pizza napolitana e sua aplicação no conceito da marca **A Boa de Napole**.

O projeto foi desenvolvido como parte de um desafio da **DIO**, com o objetivo de utilizar inteligência artificial como ferramenta de aprendizagem ativa, combinando curadoria de fontes, engenharia de prompts, análise crítica e organização do conhecimento.

> **Observação:** este é um projeto educacional. A análise das normas da pizza napolitana não representa certificação oficial da marca pela AVPN.

---

## Contexto e objetivos

A pizza napolitana envolve história, cultura, técnica artesanal e controle rigoroso de ingredientes e processos. O caderno foi criado para compreender como esses elementos influenciam a qualidade, a leveza e a identidade do produto.

Os principais objetivos foram:

- compreender as características da autêntica pizza napolitana;
- estudar fermentação, maturação e digestibilidade da massa;
- identificar ingredientes, proporções e técnicas tradicionais;
- diferenciar regras oficiais de adaptações operacionais da marca;
- relacionar a tradição napolitana com o posicionamento da **A Boa de Napole**;
- transformar o conteúdo em resumos, glossário, flashcards, infográficos e material em áudio;
- avaliar criticamente as respostas produzidas pela IA.

---

## Curadoria de fontes

Foram combinadas fontes públicas institucionais com documentos próprios da marca.

### Fontes públicas

1. [Disciplinare Internazionale da Associazione Verace Pizza Napoletana — AVPN](https://www.pizzanapoletana.org/public/pdf/Disciplinare_AVPN_2022.pdf)  
   Documento técnico com regras de preparo, ingredientes, fermentação, abertura e cocção da verdadeira pizza napolitana.

2. [Arte do Pizzaiuolo Napolitano — UNESCO](https://ich.unesco.org/en/RL/art-of-neapolitan-pizzaiuolo-00722)  
   Registro da prática como Patrimônio Cultural Imaterial da Humanidade.

3. [Regulamento Europeu nº 97/2010 — Pizza Napoletana STG](https://eur-lex.europa.eu/legal-content/PT/TXT/?uri=CELEX%3A32010R0097)  
   Especificação da União Europeia sobre a Pizza Napoletana como Especialidade Tradicional Garantida.

### Fontes próprias

4. **Manual de identidade da A Boa de Napole**  
   Utilizado para estudar propósito, tom de voz, cores, tipografia e aplicações da marca.

5. **Planilha técnica de produção**  
   Utilizada para analisar hidratação, fermentação, rendimento, peso das massas e quantidades de ingredientes.

As fontes próprias foram usadas como referências operacionais da marca, e não como normas universais da pizza napolitana.

---

## Metodologia

O trabalho foi desenvolvido em cinco etapas:

1. seleção e inclusão das fontes no NotebookLM;
2. elaboração de perguntas para mapear os assuntos principais;
3. comparação entre documentos normativos e materiais internos;
4. refinamento dos prompts para obter respostas mais estruturadas;
5. transformação do conhecimento em materiais de revisão.

O NotebookLM foi utilizado como apoio à pesquisa, mas as respostas foram confrontadas com as fontes antes de serem incorporadas ao projeto.

---

## Engenharia de prompts

### Prompt inicial

```text
Faça um resumo sobre a pizza napolitana com base nas fontes.
```

Esse prompt produziu uma resposta útil, porém genérica. Faltavam separação por temas, indicação das fontes e distinção entre regras oficiais e práticas internas.

### Prompt refinado

```text
Com base exclusivamente nas fontes selecionadas, explique o que caracteriza
uma pizza napolitana autêntica. Organize a resposta em: ingredientes, massa,
fermentação, abertura, cocção e características do produto final. Inclua as
referências utilizadas e indique quando houver divergência entre as fontes.
```

A versão refinada melhorou a organização, reduziu generalizações e facilitou a verificação das informações.

### Prompt para comparação de fontes

```text
Compare o disciplinar da AVPN com a planilha técnica da A Boa de Napole.
Crie uma tabela com os valores de hidratação, fermentação, peso das massas,
temperatura e tempo de cocção. Não trate uma prática interna como regra oficial.
Sinalize todas as divergências.
```

### Prompt para geração de flashcards

```text
Crie flashcards de pergunta e resposta sobre os conceitos mais importantes.
Use respostas curtas, mantenha números e unidades e não acrescente informações
que não estejam nas fontes. Entregue o resultado em CSV.
```

### Prompt para roteiro de áudio

```text
Crie um roteiro de podcast curto e didático sobre a ciência da pizza
napolitana. Explique fermentação, maturação, abertura manual e cocção em alta
temperatura com linguagem simples. Diferencie tradição oficial e adaptação da
marca A Boa de Napole.
```

### Prompt para infográfico

```text
Crie o conteúdo de um infográfico em português sobre a pizza napolitana.
Apresente fermentação, abertura manual, ingredientes e cocção. Use frases
curtas, revise números e ortografia e preserve a identidade visual da marca.
```

---

## “Cicatrizes” e aprendizados do processo

A IA acelerou a organização do conhecimento, mas também exigiu revisão humana.

### 1. Perguntas genéricas geraram respostas genéricas

Quando o prompt não definia estrutura, fontes ou profundidade, a resposta misturava história, receita e comunicação da marca. A solução foi dividir a pesquisa em tópicos e solicitar referências.

### 2. Fontes diferentes apresentaram valores diferentes

As normas oficiais, a planilha interna e os materiais gerados não utilizam necessariamente os mesmos números. Por exemplo, a hidratação operacional de **65%** da marca não deve ser apresentada como regra universal da AVPN.

A solução foi pedir ao NotebookLM que separasse:

- norma oficial;
- recomendação técnica;
- prática interna;
- adaptação operacional.

### 3. Um flashcard apresentou inconsistência

No arquivo de flashcards, uma pergunta menciona “três ingredientes básicos”, mas a resposta lista **quatro**: farinha, água, sal e fermento. Esse caso demonstra que um resultado aparentemente pronto ainda precisa de validação.

### 4. Imagens geradas também precisam ser revisadas

Os infográficos apresentaram boa síntese visual, mas textos, números e traduções produzidos dentro das imagens exigem conferência. Em materiais técnicos, o visual não substitui a fonte original.

### 5. A IA pode misturar tradição e identidade de marca

Foi necessário reforçar nos prompts que os documentos da marca representam decisões próprias e não uma certificação da AVPN.

### Principal aprendizado

O melhor resultado não veio de um único “prompt perfeito”, mas de um ciclo:

**perguntar → conferir → identificar falhas → refinar → comparar com as fontes.**

---

## Miniguia de estudo

### 1. Massa

A base tradicional utiliza farinha de trigo, água, sal e uma pequena quantidade de fermento. Óleo, gordura e açúcar não fazem parte da formulação tradicional estudada.

A proporção exata pode variar conforme o disciplinar, a farinha, a temperatura ambiente e o processo adotado.

### 2. Fermentação e maturação

A fermentação permite a produção dos gases responsáveis pela expansão da massa. A maturação prolongada favorece o desenvolvimento de sabor, aroma e textura.

Na operação estudada, períodos maiores, inclusive sob refrigeração, são usados para organizar a produção e desenvolver as características da massa. Esses períodos não devem ser confundidos automaticamente com exigências oficiais.

### 3. Abertura manual

O disco deve ser aberto com as mãos. O movimento leva o gás do centro para a borda, ajudando a formar o **cornicione** alto e aerado.

Rolos e prensas podem retirar os gases da fermentação e prejudicar a formação dos alvéolos.

### 4. Cocção

A pizza é assada por pouco tempo em forno de temperatura muito elevada. Dependendo do equipamento e da referência adotada, são encontradas faixas próximas de **400°C a 500°C**, com cocção aproximada de **60 a 90 segundos**.

O choque térmico expande rapidamente os gases e cria uma borda leve, macia e com manchas características.

### 5. Ingredientes

Entre os ingredientes associados à tradição estão:

- farinha adequada para fermentações prolongadas;
- tomate San Marzano;
- fior di latte ou mozzarella de búfala;
- manjericão;
- azeite de oliva extravirgem;
- água potável e sal.

### 6. Produto final

A pizza napolitana apresenta:

- centro fino e flexível;
- borda alta e alveolada;
- massa macia e elástica;
- cobertura úmida e equilibrada;
- pontos escuros produzidos pela cocção intensa;
- equilíbrio entre massa, tomate, queijo e azeite.

### 7. Cultura e experiência

A arte do pizzaiuolo napolitano foi reconhecida pela UNESCO em 2017. Mais do que uma receita, ela envolve conhecimentos, gestos, tradição e convivência.

Na identidade da **A Boa de Napole**, essa ideia é traduzida pelo propósito de criar bons momentos ao redor de uma boa pizza.

---

## Glossário

| Conceito | Definição |
|---|---|
| **AVPN** | Associazione Verace Pizza Napoletana, organização dedicada à preservação da tradição. |
| **Cornicione** | Borda alta, macia e aerada da pizza napolitana. |
| **Fermentação** | Processo em que o fermento produz gases e contribui para o crescimento da massa. |
| **Maturação** | Transformações enzimáticas que desenvolvem sabor, aroma e características da massa ao longo do tempo. |
| **Hidratação** | Relação percentual entre a quantidade de água e a quantidade de farinha. |
| **Alvéolos** | Espaços de ar formados no interior da massa. |
| **Fior di latte** | Queijo fresco de leite de vaca utilizado em pizzas. |
| **San Marzano** | Variedade de tomate tradicionalmente associada à pizza napolitana. |
| **STG** | Especialidade Tradicional Garantida, registro europeu de um produto tradicional. |
| **Leopard spots** | Pontos escuros formados na borda durante a cocção em temperatura elevada. |
| **Choque térmico** | Exposição rápida da massa a alta temperatura, provocando expansão e cocção aceleradas. |
| **Equilíbrio sensorial** | Harmonia entre massa, acidez do tomate, queijo, azeite, textura e aromas. |

---

## Prompts reutilizáveis

### Resumo com referências

```text
Com base exclusivamente nas fontes deste caderno, resuma [TEMA] em cinco
tópicos. Inclua a referência correspondente em cada tópico e informe quando
uma afirmação não puder ser confirmada.
```

### Comparação entre fontes

```text
Compare o que cada fonte afirma sobre [ASSUNTO]. Apresente uma tabela com
convergências, divergências, contexto e nível de confiança. Não tente resolver
as diferenças sem evidência.
```

### Verificação de números

```text
Localize todos os valores numéricos relacionados a [ASSUNTO], incluindo
unidades e fonte. Aponte valores conflitantes e explique se representam norma,
recomendação ou prática interna.
```

### Revisão ativa

```text
Crie dez perguntas progressivas sobre [TEMA]: quatro básicas, quatro
intermediárias e duas avançadas. Espere minha resposta antes de apresentar
o gabarito e explique os erros com base nas fontes.
```

### Flashcards

```text
Transforme os principais conceitos em flashcards. Cada cartão deve testar
apenas uma ideia. Use respostas curtas e entregue em CSV com as colunas
pergunta e resposta.
```

### Auditoria de resposta

```text
Revise a resposta anterior como um auditor. Para cada afirmação, informe:
confirmada pelas fontes, parcialmente confirmada ou não confirmada. Corrija
inconsistências sem inventar informações.
```

---

## Materiais produzidos

- [Flashcards para revisão](./flashcards.csv)
- [Infográfico: Guia da Autêntica Pizza Napolitana](./Guia_da_Aut%C3%AAntica_Pizza_Napolitana.png)
- [Infográfico: Authentic Neapolitan Pizza Quality Guide](./Authentic_Neapolitan_Pizza_Quality_Guide.png)
- [Podcast: A ciência da pizza que não estufa](./PodCast%20A_ci%C3%AAncia_da_pizza_que_n%C3%A3o_estufa.zip)

---

## Conclusão

O NotebookLM foi útil para pesquisar, comparar documentos e transformar fontes extensas em materiais de estudo. Entretanto, o projeto também mostrou que respostas e conteúdos gerados por IA não devem ser aceitos automaticamente.

A qualidade do resultado depende de três práticas:

1. selecionar fontes confiáveis;
2. elaborar prompts claros e verificáveis;
3. revisar criticamente cada resposta.

Mais do que aprender sobre pizza napolitana, este trabalho demonstrou como utilizar inteligência artificial com método, rastreabilidade e pensamento crítico.
