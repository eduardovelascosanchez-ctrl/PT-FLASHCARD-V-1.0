# Cenários de simulação NRP · 9.ª edição

Versão em **português de Portugal**, preparada para o **Dr. Eduardo Velasco · EDUVESA**. Material educativo independente, baseado no kit fornecido. Versão 1.3 PT-PT, 7 de outubro de 2026.

## Utilização sem ligação à internet

1. Descarregue e descomprima `NRP9_Cenarios_GitHub_PT-PT.zip`.
2. Abra `index.html` num navegador moderno com JavaScript ativo.
3. Pode desligar a internet: as fichas, os estilos, a pesquisa, os filtros, os guiões e o registo estão incorporados no ficheiro.

Não exige instalação, servidor, conta, dependências externas ou ligação a uma API. As ligações de referência requerem internet. Em dispositivos móveis, utilize um navegador que execute JavaScript; algumas pré-visualizações de gestores de ficheiros não o fazem.

A utilização offline pressupõe **uma cópia descarregada**. Esta versão não instala um service worker nem garante que uma página remota fique disponível em cache. Visitar GitHub Pages uma vez não garante acesso posterior sem internet.

## Conteúdo

| Lição | Tema | Competências | Práticas | Simulações originais |
|---|---|---:|---:|---:|
| 2 | Antecipação e preparação | 1 | 2 | 1 |
| 3 | Passos iniciais | 1 | 4 | 1 |
| 4 | Ventilação e máscara laríngea | 1 | 3 | 1 |
| 5 | Intubação e obstrução da via aérea | 1 | 2 | 1 |
| 6 | Compressões torácicas | 1 | 1 | 1 |
| 7 | Acesso vascular, adrenalina e volume | 1 | 1 | 1 |
| **Subtotal original** | **25 fichas** | **6** | **13** | **6** |

Cada ficha apresenta instrução, equipamento, tarefas individuais, guião do instrutor ocultável, critérios de desempenho e debriefing. Os casos têm fases com informação fornecida pelo instrutor e resposta esperada do formando. Nos casos breves, assinale apenas as competências realmente observadas; pratique as restantes na ficha de competência ou noutra ronda.

Inclui pesquisa, filtros, seleção aleatória, cronómetro pedagógico, quatro formandos com nomes editáveis, rotações, notas, avaliação formativa, exportação JSON/CSV e impressão de uma ficha ou de toda a seleção. O registo emite declarações educativas de cenário ou lição; não determina, por si só, a aprovação num curso NRP.

## Organização de uma estação

1. Selecione a lição e a ficha de **Competência**. O instrutor demonstra; cada formando pratica dentro do seu âmbito profissional.
2. Forme pares A–B e C–D e troque as funções de operador e assistente. Nas técnicas avançadas, cada participante executa ou presta assistência conforme as competências autorizadas.
3. Selecione uma ficha de **Prática**, com orientação e correção imediata quando necessário.
4. Selecione uma **Simulação**. Faça prebriefing, distribua funções e explique as limitações do manequim. O instrutor fornece os achados sem antecipar a manobra seguinte.
5. Abra o guião no dispositivo do instrutor ou imprima-o; não o projete para os formandos durante o cenário. Ocultá-lo é uma ajuda pedagógica, não uma restrição de acesso.
6. Selecione o formando antes de assinalar tarefas e resultados. Todos devem liderar uma ronda e demonstrar as competências pertinentes; observar não substitui praticar.
7. Faça debriefing: reação breve, reconstrução, análise por observação e indagação e compromisso de melhoria. Repita as competências que necessitem de reforço.
8. Exporte o registo antes de fechar a página ou mudar de dispositivo.

A tabela de rotações é orientativa. O líder redistribui tarefas de acordo com os profissionais disponíveis e a complexidade; pode ser necessário pessoal adicional. O cronómetro mede tempo pedagógico: não controla o algoritmo nem altera automaticamente os sinais vitais.

## Ficheiros

- `index.html`: aplicação completa e autónoma, pronta para servir como página principal.
- `README.md`: instruções de utilização, âmbito e publicação.
- `conteudo.json`: cópia estruturada e editável das lições e fichas.
- `sincronizar_conteudo.py`: atualiza os dados incorporados no HTML; requer Python 3, sem pacotes adicionais.
- `NOTAS_CLINICAS.md`: decisões editoriais e pontos de revisão para o instrutor.
- `.nojekyll`: permite servir o projeto como conteúdo estático sem processamento Jekyll.

O PDF fonte não está incluído. Não são acrescentados logótipos nem uma licença aberta sobre conteúdos de terceiros.

## Preparação para GitHub ou portal

O ZIP está pronto para ser carregado; **não cria um repositório remoto nem publica automaticamente num portal**.

1. Crie ou escolha um repositório GitHub.
2. Carregue os ficheiros descomprimidos na raiz. `index.html` deve ficar na raiz, não dentro de um ZIP.
3. Confirme as alterações no ramo que pretende publicar.
4. Se desejar uma página web, configure GitHub Pages para servir o ramo e a pasta que contêm `index.html`, de acordo com as opções da sua conta.
5. Guarde a cópia local para utilizar sem internet.

Num portal que aceite conteúdo estático, coloque `index.html` na pasta de publicação. A integração num portal existente depende do respetivo repositório, endereço e estrutura.

Não carregue registos de formandos, dados de doentes, credenciais ou o PDF do kit para um repositório público. Verifique as autorizações relativas a materiais adicionais antes de os publicar.

## Registos e privacidade

A aplicação utiliza `localStorage` quando o navegador o permite. No modo privado ou em ficheiros `file://`, o armazenamento pode ser limitado; a aplicação avisa se não conseguir guardar. Os registos desta versão utilizam uma chave própria PT-PT, distinta da versão espanhola.

Os dados não são transmitidos nem sincronizados. Podem perder-se ao apagar dados do navegador, mover o ficheiro ou mudar de navegador. Utilize iniciais quando adequado e exporte uma cópia no final.

O JSON exportado é uma cópia de segurança legível; esta versão não importa registos. O CSV inclui o estado de todas as fichas por formando e pode ser aberto numa folha de cálculo.

## Editar o conteúdo

Edite `conteudo.json` e execute na pasta do projeto:

```bash
python3 sincronizar_conteudo.py
```

O script verifica a estrutura básica, os identificadores e as referências às lições. Não valida a exatidão médica. Um instrutor qualificado deve rever alterações e testar a página antes de a distribuir. Para alterar o aspeto ou as funções, edite o HTML.

## Fontes e âmbito

Fonte principal: **NRP_9ed_Kit_Instructor_ES_COMPLETO(3).pdf**, fornecido pelo utilizador, com 86 páginas. As referências das fichas correspondem às páginas do ficheiro PDF, não à paginação interna reiniciada de cada secção.

| Material fonte | Páginas do PDF |
|---|---|
| Construtor de cenários | 9–10 |
| Instruções e modelo de cenários | 11–27 |
| Lição 2 | 28–32 |
| Lição 3 | 33–40 |
| Lição 4 | 41–52 |
| Lição 5 | 53–63 |
| Lição 6 | 64–69 |
| Lição 7 | 70–77 |

Consulta complementar utilizada na versão espanhola: [AHA/AAP, 2025 Guidelines, Part 5: Neonatal Resuscitation](https://cpr.heart.org/en/resuscitation-science/cpr-and-ecc-guidelines/neonatal-resuscitation), consultada a 6 de outubro de 2026.

Esta versão traduz e adapta a terminologia para Portugal, preservando doses, tempos e critérios da versão espanhola. As práticas são adaptações resumidas; as seis simulações estão identificadas como propostas originais. Não são formulários oficiais nem uma reprodução completa do ITK. O âmbito termina na lição 7 e não cobre todas as lições do manual.

NRP é uma marca da American Academy of Pediatrics. Material independente sem implicar aprovação pela AAP/AHA. Destina-se ao treino com manequim sob supervisão e não substitui o manual vigente ou os protocolos institucionais.

## Verificação desta entrega

Foram verificadas a sintaxe de JavaScript, a correspondência das 38 fichas, a preservação dos valores numéricos e a ausência de recursos de execução remotos. As funções principais da versão espanhola foram verificadas num ambiente DOM; não foi possível repetir essa verificação nesta tradução. A revisão visual num navegador real continua pendente; antes do primeiro curso, confirme os filtros, o guião do instrutor, o registo e a exportação no dispositivo que irá utilizar.

## Simulações do ITK acrescentadas · versão 1.1

O ITK exige simulação com debriefing no curso; não estabelece uma lista única de cenários obrigatórios por lição. A agenda permite reutilizar práticas selecionadas ou construir cenários segundo os objetivos. Os casos abaixo são **adaptações para simulação integrada das variantes de prática do kit**, não novos formulários oficiais. A aplicação contém agora **38 fichas: 6 de competências, 13 práticas, 6 simulações originais e 13 simulações ITK**.

| Lição | Variantes ITK para selecionar | Fichas | Páginas PDF |
|---|---|---:|---|
| 2 | Preparação de um nascimento de baixo risco / às 29 semanas | 2 | 28–32 |
| 3 | De termo vigoroso / mecónio e cianose / resposta aos passos iniciais / prematuro tardio em apneia | 4 | 33–40 |
| 4 | Ventilação com risco conhecido / apneia inesperada / máscara laríngea | 3 | 41–52 |
| 5 | Intubação / obstrução com necessidade de aspiração traqueal | 2 | 53–63 |
| 6 | Bradicardia persistente que exige compressões | 1 | 64–69 |
| 7 | Prolapso do cordão: CVU, adrenalina e opção de volume se indicada | 1 | 70–77 |

Selecione **Simulação ITK** no filtro Atividade. Cada nova ficha acrescenta objetivos, respostas às quatro perguntas prévias, referência ao documento, instruções de facilitação sem orientação, guião condicionado à atuação e debriefing.

A lição 2 adapta exercícios de preparação: o Construtor começa na lição 3. O caso de apneia da lição 3 deve continuar imediatamente para ventilação quando se realiza uma simulação integrada; o ponto de paragem da prática isolada não deve interromper cuidados reais. As opções de CPAP, sonda OG, volume, sangue e acesso intraósseo dependem dos objetivos e da indicação, não são obrigatórias em todos os cenários.

O Construtor sugere riscos adicionais por complexidade: lição 3, hipertensão/ausência de vigilância pré-natal/prematuridade; lição 4, pré-eclâmpsia/magnésio/restrição de crescimento/mecónio quando apropriado; lição 5, padrão fetal categoria III/febre/apresentação anómala; lição 6, eclâmpsia/extração por ventosa falhada/bradicardia fetal; lição 7, cesariana urgente e anestesia geral, acrescentando evidência plausível de perda sanguínea se pretende avaliar volume. Estes são exemplos de construção, não sinais que obrigam automaticamente a uma intervenção.

A simulação inclui competências comportamentais em todas as lições. O facilitador regista decisões e ações e guarda a análise para o debriefing. Fontes: pp. 1–5, 9–10 e 11–27, além das páginas de cada lição.

## Narrativa clínica em cada ficha · versão 1.2

As 38 fichas incluem agora uma narrativa clínica para preparar e apresentar o caso. A guia do instrutor acrescenta o estado inicial do recém-nascido, a evolução prevista, notas sobre os limites do caso e respostas às quatro perguntas prévias nas variantes do kit. As fichas de competência apresentam um caso de referência e botões para abrir as restantes variantes da lição. Os seis cenários originais mantêm essa identificação.

Os dados obstétricos devem ser fornecidos quando solicitados; os sinais neonatais são revelados na fase correspondente. Não acrescentar idade materna, peso, via do parto ou diagnóstico como se fossem dados do kit quando não estão especificados. A versão (3) do PDF fornecido contém o mesmo conteúdo da versão (2) utilizada anteriormente.

## Avaliação e certificados · versão 1.3

1. Selecione o formando e introduza o nome completo. Acrescente o instrutor avaliador, a entidade emissora e a data em «Métricas, progresso e certificados».
2. Indique a função individual. Pontue cada ação: **2 correta sem ajuda; 1 correta com ajuda; 0 incorreta**. «Não observado» mantém-se pendente. «Não aplicável» exige justificação. As caixas antigas são um registo de prática e não são convertidas automaticamente em classificações.
3. A classificação é `100 × pontos obtidos / (2 × ações aplicáveis)`. As ações não observadas mantêm-se no denominador. As exclusões justificadas são retiradas. A cobertura é a percentagem de ações aplicáveis já avaliadas. Não é possível certificar uma avaliação sem ações pontuáveis.
4. Conclusão satisfatória: classificação **≥80%**, cobertura **100%**, todos os pontos críticos aplicáveis com **2**, identificação, função e encerramento pelo instrutor. Uma avaliação insuficiente pode ser encerrada para conservar o registo; não disponibiliza um certificado. O limiar não é uma regra oficial do ITK/AAP/AHA nem uma escala validada. Os pontos críticos são uma seleção editorial visível na tabela.
5. Descarregue o certificado em **PDF direto**, sem ligação à internet nem dependências. A opção **HTML** inclui o detalhe de ações, pontuação, justificações e evidência, permitindo imprimir ou guardar como PDF no navegador.
6. Para a lição, utiliza-se a evidência **mais recente** de cada competência entre as rondas atuais, sem duplicar pontos. Todas devem ter pontuação observada numa avaliação encerrada. Uma ação «Não aplicável» num cenário não comprova a competência da lição. Complete-a na ficha de competência ou noutro caso. Não é necessário concluir todas as variantes.
7. Uma alteração da avaliação, função, nome do formando ou dados de emissão invalida o encerramento afetado até nova revisão. «Nova ronda» conserva a anterior no histórico do JSON. O certificado descreve a ronda atual e não certifica uma trajetória acumulada nem resultados de outros formandos.
8. Exporte o JSON como cópia de segurança (inclui grelha e histórico) e o CSV detalhado para rever ações e classificações. Os PDF/HTML descarregados são instantâneos: não são atualizados nem revogados automaticamente quando o registo local muda.

O certificado é uma **declaração educativa da EDUVESA**. Não constitui eCard, certificação NRP da AAP/AHA, acreditação como prestador avançado nem autorização clínica. Não inclui assinatura digital, autenticação de identidade ou consulta externa; o instrutor é responsável pela avaliação declarada.
