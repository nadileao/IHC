# Avaliação de Acessibilidade

Avaliação de acessibilidade do sistema **Lucid** (editor de diagramas online), com base nas diretrizes da **WCAG 2.2**.

## Escopo da avaliação

Foram selecionadas as seguintes telas para inspeção:

1. **Tela de Login**
2. **Tela Inicial** (Dashboard)
3. **Tela de Edição** (Editor)
4. **Tela de Templates** (Modelos Prontos)
5. **Tela de Compartilhar**

## Processo utilizado

A avaliação foi feita em três etapas: **detecção**, **coleção** e **discriminação**.

**1. Detecção.** Quatro avaliadores ([Marcos](https://app.notion.com/p/520d4fd66fdb838e9a9e01b68dcc5dc9?v=ef9d4fd66fdb8216a72c8807f21f077a), [Nádia](https://app.notion.com/p/196d4fd66fdb83ff9b9c81fcdc5b6b93?v=514d4fd66fdb82659a04887955b94883), [Matheus](https://app.notion.com/p/c62d4fd66fdb83a6928881c9c0731989?v=74ad4fd66fdb83b78de5885647c22e86) e [Kevily](https://app.notion.com/p/4e1d4fd66fdb83668a44019b73cac496?v=78dd4fd66fdb82ef9c03885cb259c231)) inspecionaram as telas de forma independente. Cada um registrou os problemas encontrados, com o processo utilizado, a tela, a frequência e o critério WCAG violado. Foram usados:
- navegação apenas pelo teclado (Tab / Shift+Tab);
- leitor de tela (NVDA) e simulação por árvore de acessibilidade;
- ferramentas automáticas (WAVE, axe DevTools e Accessibility Insights);
- simulação visual (Funkify);
- zoom de 200% e 400%;
- inspeção do código (por exemplo, o atributo `lang`).

No total foram registrados **31 problemas**.

**2. Coleção.** Os registros dos quatro avaliadores foram reunidos em uma única tabela. Registros que descrevem o mesmo problema (mesma causa, mesmo em telas ou avaliadores diferentes) foram agrupados. Para cada grupo foi mantido o registro que melhor descrevia o problema, e a ocorrência foi classificada como **única** (1 registro) ou **repetida** (2 ou mais registros). O resultado foi **19 problemas**: 7 repetidos e 12 únicos.

[Confira aqui o Notion da Coleção](https://app.notion.com/p/834d4fd66fdb827e8d69016032cd1c94?v=f88d4fd66fdb8341883d082c979c2040)

**3. Discriminação.** Cada problema foi classificado como **defeito** ou **falso positivo**. Resultaram **17 defeitos** e **2 falsos positivos**:
- o contraste das fontes finas, observado só com o simulador Funkify, sem medição da razão de contraste;
- a hierarquia de títulos, que o axe trata como boa prática e não como falha direta da WCAG.

[Confira aqui o Notion da Discriminação](https://app.notion.com/p/77cd4fd66fdb838786a581bc34f529c9?v=d3ad4fd66fdb83d9a4f488c18875ca3d)

As tabelas a seguir apresentam apenas os **defeitos**.

## Resultados da inspeção

### Síntese dos problemas encontrados

A tabela lista os 17 defeitos confirmados, com o critério WCAG relacionado, a tela onde ocorreram e a frequência observada. A maior frequência é a de campos sem rótulo associado (13 ocorrências), seguida dos rótulos órfãos (6) e dos botões do menu sem contorno de foco (4).

| Problema | Critério WCAG | Tela/Página | Frequência |
|---|---|---|---|
| Forma inserida pelo teclado não é exposta ao leitor de tela (canvas sem alternativa em texto) | 1.1.1 - Conteúdo não textual | Tela de Edição | 1 |
| Rótulo de formulário órfão (texto do rótulo não vinculado ao campo) | 1.3.1 - Informações e relações | Tela Inicial e Tela de Edição | 6 |
| Opção de ativar/desativar link não tem função compreensível | 1.3.1 - Informações e relações | Tela de Compartilhar | 1 |
| Sem contorno de foco nos botões do menu (+Novo, Home, Documento, Integrações) | 1.4.4 - Redimensionar texto | Tela Inicial | 4 |
| Elementos do topo ("Enter Join ID" e "View all plans") não acessíveis pelo teclado | 2.1.1 - Teclado | Tela de Login | 2 |
| Editor não permite redimensionar/editar elementos apenas com o teclado | 2.1.1 - Teclado | Tela de Edição | 1 |
| Botões com nome não descritivo ("Imagem clicável de estado vazio") | 2.4.6 - Cabeçalhos e rótulos | Tela Inicial | 2 |
| Página sem idioma definido (`<html>` sem atributo `lang`) | 3.1.1 - Idioma da página | Tela de Edição | 1 |
| Trecho em inglês sem `lang="en"` em página pt-BR | 3.1.2 - Idioma das partes | Tela de Templates | 1 |
| Rótulo de formulário ausente (Missing form label) | 3.3.2 - Rótulos ou instruções | Tela de Login e Tela Inicial | 13 |
| Com zoom de 400% não é possível rolar a página | 3.3.2 - Rótulos ou instruções | Tela Inicial | 1 |
| Botão sem texto acessível (seletor de fonte em canvas sem `aria-label`) | 4.1.2 - Nome, função, valor | Tela Inicial e Tela de Edição | 3 |
| Diálogo (`role="dialog"`) sem nome acessível | 4.1.2 - Nome, função, valor | Tela de Templates e Tela de Compartilhar | 2 |
| Referência ARIA corrompida (Broken ARIA reference) | 4.1.2 - Nome, função, valor | Tela Inicial | 2 |
| Parada de foco extra no avatar "KO" (Tab foca duas vezes o mesmo controle) | 4.1.2 - Nome, função, valor | Tela Inicial | 1 |
| Com zoom de 200% o botão "Upgrade" desaparece | 4.1.2 - Nome, função, valor | Tela Inicial | 1 |
| Sem retorno falado ao inserir, apagar ou alterar formas no editor | 4.1.3 - Mensagens de status | Tela de Edição | 1 |

### Critérios WCAG violados

A tabela mostra os 10 critérios da WCAG 2.2 envolvidos nos defeitos, agrupados por princípio. O princípio **Robusto** concentra o maior número de problemas (6), principalmente por causa do critério 4.1.2. Depois vêm **Perceptível** (4) e **Compreensível** (4), e por último **Operável** (3).

| Princípio | Diretriz | Critério violado | Nível |
|---|---|---|---|
| Perceptível | 1.1 Alternativas em texto | 1.1.1 Conteúdo não textual | A |
| Perceptível | 1.3 Adaptável | 1.3.1 Informações e relações | A |
| Perceptível | 1.4 Discernível | 1.4.4 Redimensionar texto | AA |
| Operável | 2.1 Acessível por teclado | 2.1.1 Teclado | A |
| Operável | 2.4 Navegável | 2.4.6 Cabeçalhos e rótulos | AA |
| Compreensível | 3.1 Legível | 3.1.1 Idioma da página | A |
| Compreensível | 3.1 Legível | 3.1.2 Idioma das partes | AA |
| Compreensível | 3.3 Assistência de entrada | 3.3.2 Rótulos ou instruções | A |
| Robusto | 4.1 Compatível | 4.1.2 Nome, função, valor | A |
| Robusto | 4.1 Compatível | 4.1.3 Mensagens de status | AA |

## Considerações sobre os resultados

Foram confirmados 17 defeitos de acessibilidade nas cinco telas avaliadas. A **Tela Inicial** concentra a maioria deles, e o **Editor** traz os problemas mais críticos para quem usa apenas teclado ou leitor de tela.

Três pontos se destacam:
- **Falta de nome e rótulo acessíveis.** Campos sem rótulo, botões sem texto e diálogos sem nome (critérios 3.3.2, 1.3.1 e 4.1.2) são a causa mais frequente. Eles impedem que o leitor de tela informe a função dos controles.
- **Uso do teclado.** Os botões do cabeçalho do Login, o redimensionamento no Editor e o contorno de foco no menu da Tela Inicial prejudicam a navegação sem mouse.
- **Idioma e zoom.** A ausência de `lang` e a perda de elementos com zoom de 200% e 400% afetam leitores de tela e pessoas com baixa visão.

Os 2 falsos positivos descartados mostram a importância de confirmar os resultados de ferramentas e simuladores. Em especial, o contraste das fontes finas não foi medido; vale uma nova verificação com um medidor de contraste (por exemplo, o WebAIM Contrast Checker).

Como limitação, a avaliação cobre cinco telas e quatro avaliadores, então outros problemas podem existir em telas não inspecionadas.
