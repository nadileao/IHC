#  HTAs: ItaAluga
 

Os HTAs (*Hierarchical Task Analysis*) detalham como cada objetivo do [mapa de objetivos](./3-mapa-de-objetivos.md) é cumprido, decompondo a tarefa principal em subtarefas e planos de execução. Cada um dos **12 grupos do mapa** tem um HTA correspondente, apresentado lado a lado com o respectivo grupo para evidenciar a consistência entre o que foi planejado e o que foi detalhado.

## Visão Geral

| HTA | Objetivo (tarefa 0) | Papéis | Plano | Grupo no mapa |
| :---: | :--- | :---: | :---: | :--- |
| [1](#hta-1-criar-minha-conta) | Criar minha conta | LD, LT, UA | `1 > 2 > 3` | [Cadastro](./3-mapa-de-objetivos.md#1-cadastro) |
| [2](#hta-2-entrar-na-minha-conta) | Entrar na minha conta | LD, LT, UA | `1 / 2` | [Acesso](./3-mapa-de-objetivos.md#2-acesso) |
| [3](#hta-3-colocar-um-equipamento-para-alugar) | Colocar um equipamento para alugar | LD, UA | `1 > 2 > 3 > 4` | [Criação de Anúncios](./3-mapa-de-objetivos.md#3-criação-de-anúncios) |
| [4](#hta-4-gerenciar-meus-anúncios-e-pedidos) | Gerenciar meus anúncios e pedidos | LD, UA | `1 / 2` | [Gestão de Pedidos e Locações](./3-mapa-de-objetivos.md#4-gestão-de-pedidos-e-locações) |
| [5](#hta-5-encontrar-um-equipamento) | Encontrar um equipamento | LT, UA | `1 > 2` | [Busca de Equipamentos](./3-mapa-de-objetivos.md#5-busca-de-equipamentos) |
| [6](#hta-6-alugar-um-equipamento) | Alugar um equipamento | LT, UA | `1 > 2 > 3 > 4` | [Solicitação e Pagamento](./3-mapa-de-objetivos.md#6-solicitação-e-pagamento) |
| [7](#hta-7-realizar-a-entrega-do-equipamento) | Realizar a entrega do equipamento | LD, LT, UA | `1 > 2` | [Entrega do Equipamento](./3-mapa-de-objetivos.md#7-entrega-do-equipamento) |
| [8](#hta-8-concluir-a-devolução-do-equipamento) | Concluir a devolução do equipamento | LD, LT, UA | `1 > 2 > 3 > 4` | [Devolução do Equipamento](./3-mapa-de-objetivos.md#8-devolução-do-equipamento) |
| [9](#hta-9-resolver-um-problema-no-aluguel) | Resolver um problema no aluguel | LD, LT, UA | `((1 > 2) / 3) > 4 > 5` | [Problemas](./3-mapa-de-objetivos.md#9-problemas) |
| [10](#hta-10-analisar-e-resolver-disputas) | Analisar e resolver disputas | ST | `1 > 2 > 3` | [Mediação de Casos](./3-mapa-de-objetivos.md#10-mediação-de-casos) |
| [11](#hta-11-avaliar-e-ver-reputação) | Avaliar e ver reputação | LD, LT, UA | `1 / 2` | [Reputação e Avaliações](./3-mapa-de-objetivos.md#11-reputação-e-avaliações) |
| [12](#hta-12-pedir-e-prestar-ajuda) | Pedir e prestar ajuda | LD, LT, UA, ST | `1 / (2 > 3)` | [Ajuda e Suporte](./3-mapa-de-objetivos.md#12-ajuda-e-suporte) |

---

## Detalhamento dos HTAs

### HTA 1: Criar minha conta

<img src="imagem/HTA de cadastro.png" alt="Mapa de objetivos e HTA: Criar minha conta" width="900">

**Propósito.** Permitir que qualquer pessoa crie a conta única do ItaAluga, usada tanto para anunciar quanto para alugar equipamentos.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Informar meus dados básicos** | 1.1 Digitar o nome completo; 1.2 Digitar o número de telefone; 1.3 Aceitar os termos de uso | `1.1 + 1.2 + 1.3` |
| **2. Confirmar meu contato** | 2.1 Solicitar o envio do código (2.1.1 por SMS ou 2.1.2 por WhatsApp); 2.2 Digitar o código recebido | `2.1 > 2.2` e `2.1.1 / 2.1.2` |
| **3. Definir minha senha** | 3.1 Criar uma senha de acesso; 3.2 Confirmar a senha digitada; 3.3 Finalizar o cadastro | `3.1 > 3.2 > 3.3` |

**Decisões e fluxo.** O cadastro segue em sequência: dados básicos, confirmação do contato e definição da senha. A única decisão do usuário é o canal de recebimento do código (SMS ou WhatsApp). A confirmação do contato garante que o telefone informado na tarefa 1 pertence ao usuário, e a finalização do cadastro (3.3) encerra o fluxo e libera o acesso ao aplicativo.

---

### HTA 2: Entrar na minha conta

<img src="imagem/HTA de acesso.png" alt="Mapa de objetivos e HTA: Entrar na minha conta" width="900">

**Propósito.** Permitir que quem já tem cadastro acesse o aplicativo e, se esquecer a senha, consiga recuperá-la sem precisar de ajuda externa.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Fazer login no aplicativo** | 1.1 Informar o telefone cadastrado; 1.2 Digitar a senha; 1.3 Confirmar o acesso | `(1.1 + 1.2) > 1.3` |
| **2. Recuperar minha senha** | 2.1 Pedir a recuperação da senha; 2.2 Informar o telefone cadastrado; 2.3 Validar o código de verificação recebido; 2.4 Cadastrar uma nova senha | `2.1 > 2.2 > 2.3 > 2.4` |

**Decisões e fluxo.** A decisão central é escolher entre o login (1) e a recuperação de senha (2). No login, telefone e senha podem ser preenchidos em qualquer ordem e só depois o acesso é confirmado. Na recuperação, o código enviado ao telefone cadastrado comprova a identidade antes de a nova senha ser definida, e depois dela o usuário pode retomar o login.

---

### HTA 3: Colocar um equipamento para alugar

<img src="imagem/HTA de anunciar.png" alt="Mapa de objetivos e HTA: Colocar um equipamento para alugar" width="900">

**Propósito.** Guiar o locador na criação e publicação de um anúncio, apresentando o equipamento, definindo as condições do aluguel e confirmando sua identidade.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Mostrar o equipamento e seu estado** | 1.1 Iniciar o anúncio; 1.2 Escolher a categoria; 1.3 Adicionar fotos (1.3.1 abrir a câmera ou 1.3.2 escolher arquivo); 1.4 Escrever o título e a descrição; 1.5 Selecionar o estado de conservação | `1.1 > 1.2 > (1.3 + 1.4 + 1.5)` e `1.3.1 / 1.3.2` |
| **2. Definir preços e regras do aluguel** | 2.1 Informar o valor da diária; 2.2 Definir o prazo máximo de locação; 2.3 Definir o valor da caução; 2.4 Informar o bairro ou local de retirada | `2.1 + 2.2 + 2.3 + 2.4` |
| **3. Confirmar minha identidade** | 3.1 Fotografar o RG ou 3.2 Fotografar a CNH; 3.3 Tirar uma selfie para validação facial; 3.4 Enviar o comprovante de endereço (3.4.1 tirar foto ou 3.4.2 escolher arquivo) | `(3.1 / 3.2) > 3.3 > 3.4` e `3.4.1 / 3.4.2` |
| **4. Publicar o anúncio** | 4.1 Revisar o resumo das informações; 4.2 Confirmar e ativar o anúncio | `4.1 > 4.2` |

**Decisões e fluxo.** As tarefas ocorrem em sequência, e a confirmação de identidade (tarefa 3) só é pedida na primeira vez que o usuário anuncia ou solicita um aluguel; nas demais vezes, ela é pulada." O usuário decide a origem das fotos (câmera ou arquivo), o documento de identificação (RG ou CNH) e a forma de enviar o comprovante de endereço (foto ou arquivo). Os campos de cada etapa podem ser preenchidos em qualquer ordem. A confirmação de identidade (3) dá segurança a quem for alugar, e a revisão (4.1) evita publicar informações incorretas antes da ativação (4.2).

---

### HTA 4: Gerenciar meus anúncios e pedidos

<img src="imagem/HTA de gestão.png" alt="Mapa de objetivos e HTA: Gerenciar meus anúncios e pedidos" width="900">

**Propósito.** Permitir que o locador responda aos pedidos de aluguel que recebe e acompanhe seus anúncios e locações.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Decidir quem pode alugar meu equipamento** | 1.1 Abrir a solicitação de aluguel recebida; 1.2 Conferir o perfil e a reputação do locatário; 1.3 Aceitar o pedido; 1.4 Recusar o pedido; 1.5 Propor alteração de data, horário ou local | `1.1 > 1.2 > (1.3 / 1.4 / 1.5)` |
| **2. Acompanhar meus anúncios e aluguéis** | 2.1 Gerenciar anúncios ativos (2.1.1 editar ou 2.1.2 excluir); 2.2 Visualizar o status dos aluguéis em andamento | `2.1 / 2.2` e `2.1.1 / 2.1.2` |

**Decisões e fluxo.** O locador escolhe entre decidir um pedido (1) ou acompanhar o que já existe (2). Ao decidir, ele só chega à resposta depois de abrir a solicitação e conferir a reputação do locatário, e então escolhe uma de três respostas: aceitar, recusar ou propor uma alteração. A contraproposta (1.5) é a que chega ao locatário no [HTA 6](#hta-6-alugar-um-equipamento), tarefa 3.

---

### HTA 5: Encontrar um equipamento

<img src="imagem/HTA de busca.png" alt="Mapa de objetivos e HTA: Encontrar um equipamento" width="900">

**Propósito.** Ajudar o locatário a localizar um equipamento disponível e a decidir se confia no item e no dono antes de pedir o aluguel.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Pesquisar equipamentos disponíveis** | 1.1 Digitar o nome na barra de busca ou 1.2 Navegar pelas categorias; 1.3 Aplicar filtros (1.3.1 definir a faixa de preço e 1.3.2 escolher o bairro); 1.4 Selecionar um anúncio na lista de resultados | `(1.1 / 1.2) > 1.3 > 1.4` e `1.3.1 + 1.3.2` |
| **2. Conferir o item e a reputação do dono** | 2.1 Visualizar as fotos e o estado de conservação; 2.2 Ler a descrição e as regras de uso; 2.3 Verificar o valor da diária, a caução e o bairro de retirada; 2.4 Consultar as avaliações e a reputação do locador | `2.1 + 2.2 + 2.3 + 2.4` |

**Decisões e fluxo.** O usuário escolhe como procurar: por busca textual ou por categorias. Em seguida, refina por preço e bairro e seleciona um anúncio. A conferência (2) reúne em qualquer ordem as informações de que ele precisa para decidir, incluindo a reputação do locador, e prepara a solicitação do aluguel no [HTA 6](#hta-6-alugar-um-equipamento).

---

### HTA 6: Alugar um equipamento

<img src="imagem/HTA de Solicitar.png" alt="Mapa de objetivos e HTA: Alugar um equipamento" width="900">

**Propósito.** Conduzir o locatário da solicitação do aluguel até o pagamento, confirmando sua identidade e acompanhando a resposta do locador.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Pedir o aluguel do equipamento** | 1.1 Selecionar as datas e horários de retirada e devolução; 1.2 Conferir o resumo dos valores; 1.3 Solicitar o aluguel | `(1.1 + 1.2) > 1.3` |
| **2. Confirmar minha identidade** | 2.1 Fotografar o RG ou 2.2 Fotografar a CNH; 2.3 Tirar uma selfie para validação facial; 2.4 Enviar o comprovante de endereço (2.4.1 tirar foto ou 2.4.2 escolher arquivo) | `(2.1 / 2.2) > 2.3 > 2.4` e `2.4.1 / 2.4.2` |
| **3. Concluir o pedido** | 3.1 Ler a resposta do locador; 3.2 Responder à contraproposta de horário ou local; 3.3 Visualizar o endereço completo e o telefone do locador liberados; 3.4 Ver o código ou comprovante de retirada | `3.1 > (3.2 / 3.3) > 3.4` |
| **4. Realizar o pagamento** | 4.1 Escolher a forma de pagamento (4.1.1 Pix ou 4.1.2 cartão de crédito); 4.2 Confirmar o pagamento | `4.1 > 4.2` e `4.1.1 / 4.1.2` |

**Decisões e fluxo.** A tarefa 2 reaproveita o mesmo processo de verificação de identidade do [HTA 3](#hta-3-colocar-um-equipamento-para-alugar), para que locador e locatário passem pela mesma checagem. Ao concluir o pedido, a decisão depende da resposta do locador: se houver contraproposta, o locatário a responde (3.2); se o pedido foi aceito, ele visualiza o endereço e o telefone liberados (3.3). Em ambos os casos, termina com o código ou comprovante de retirada (3.4). No pagamento, o usuário escolhe entre Pix e cartão de crédito e confirma a transação.

---

### HTA 7: Realizar a entrega do equipamento

<img src="imagem/HTA de entrega.png" alt="Mapa de objetivos e HTA: Realizar a entrega do equipamento" width="900">

**Propósito.** Registrar o estado do equipamento no momento da entrega, criando uma prova que protege locador e locatário e marca o início do aluguel.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Registrar o estado do item na entrega** | 1.1 Abrir o aluguel ativo; 1.2 Tirar fotos atuais do equipamento; 1.3 Conferir acessórios e funcionamento na hora; 1.4 Marcar o estado de conservação; 1.5 Enviar o registro de vistoria inicial | `1.1 > (1.2 + 1.3 + 1.4) > 1.5` |
| **2. Confirmar o início do aluguel** | 2.1 Revisar o registro da entrega; 2.2 Validar a entrega presencialmente | `2.1 > 2.2` |

**Decisões e fluxo.** O registro (1) acontece primeiro: o usuário abre o aluguel, faz fotos, confere acessórios e funcionamento e marca a conservação em qualquer ordem, e só então envia a vistoria. A confirmação (2) vem depois, com revisão do registro e validação presencial, o que oficializa o início do aluguel. O registro feito aqui é a base da comparação no [HTA 8](#hta-8-concluir-a-devolução-do-equipamento) e das provas no [HTA 9](#hta-9-resolver-um-problema-no-aluguel).

---

### HTA 8: Concluir a devolução do equipamento

<img src="imagem/HTA de devolução.png" alt="Mapa de objetivos e HTA: Concluir a devolução do equipamento" width="900">

**Propósito.** Encerrar o aluguel com segurança, comparando o estado do equipamento antes e depois do uso.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Acompanhar o prazo de devolução** | Tarefa simples, sem subtarefas | n/a |
| **2. Registrar o estado do item na devolução** | 2.1 Abrir o aluguel a devolver; 2.2 Tirar fotos do equipamento na devolução; 2.3 Marcar o estado atual e os acessórios; 2.4 Enviar o registro da devolução | `2.1 > (2.2 + 2.3) > 2.4` |
| **3. Comparar o estado antes e depois do uso** | 3.1 Ver lado a lado o registro da entrega e o da devolução; 3.2 Confirmar que o equipamento voltou nas mesmas condições; 3.3 Sinalizar divergência ou dano | `3.1 > (3.2 / 3.3)` |
| **4. Encerrar o aluguel** | Tarefa simples, sem subtarefas | n/a |

**Decisões e fluxo.** O fluxo vai do acompanhamento do prazo ao registro do estado na devolução, à comparação e ao encerramento. A decisão principal está na comparação: se o equipamento voltou nas mesmas condições, o usuário confirma (3.2) e o aluguel pode ser encerrado; se houver diferença, ele sinaliza divergência ou dano (3.3), o que leva ao [HTA 9](#hta-9-resolver-um-problema-no-aluguel).

---

### HTA 9: Resolver um problema no aluguel

<img src="imagem/HTA de Problema.png" alt="Mapa de objetivos e HTA: Resolver um problema no aluguel" width="900">

**Propósito.** Permitir que locador ou locatário reporte, comprove e acompanhe um problema ocorrido no aluguel e receba uma decisão sobre ele.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Informar um problema** | 1.1 Iniciar o relato; 1.2 Selecionar o motivo (1.2.1 dano, 1.2.2 atraso, 1.2.3 defeito ou 1.2.4 não devolução); 1.3 Descrever o ocorrido | `1.1 > 1.2 > 1.3` e `1.2.1 / 1.2.2 / 1.2.3 / 1.2.4` |
| **2. Enviar provas do que aconteceu** | 2.1 Anexar fotos ou vídeos atuais do equipamento; 2.2 Anexar as fotos da entrega e da devolução; 2.3 Enviar o relato e as provas | `(2.1 + 2.2) > 2.3` |
| **3. Responder a um problema** | 3.1 Abrir a notificação recebida; 3.2 Ler o relato e as provas da outra parte; 3.3 Escrever a justificativa e anexar contraprovas; 3.4 Enviar a defesa dentro do prazo | `3.1 > 3.2 > 3.3 > 3.4` |
| **4. Acompanhar a análise do caso** | 4.1 Consultar o andamento do problema; 4.2 Enviar informações complementares | `4.1 > 4.2` |
| **5. Receber o resultado final** | 5.1 Ler a decisão e a justificativa do suporte; 5.2 Conferir o destino financeiro da garantia (5.2.1 liberação ou 5.2.2 retenção da caução) | `5.1 > 5.2` e `5.2.1 / 5.2.2` |

**Decisões e fluxo.** O plano `((1 > 2) / 3) > 4 > 5` separa dois caminhos de entrada: quem identifica o problema informa (1) e envia as provas (2); a outra parte, ao ser notificada, responde (3). Depois os dois caminhos convergem no acompanhamento da análise (4) e no resultado final (5). A decisão do usuário ao informar é o motivo do problema, e o resultado final define se a caução é liberada ou retida. Os casos são analisados pelo suporte no [HTA 10](#hta-10-analisar-e-resolver-disputas).

---

### HTA 10: Analisar e resolver disputas

<img src="imagem/HTA de mediação.png" alt="Mapa de objetivos e HTA: Analisar e resolver disputas" width="900">

**Propósito.** Descrever como o Suporte Técnico analisa um problema reportado, decide a solução e comunica o resultado às partes.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Analisar o caso e as provas** | 1.1 Abrir o caso; 1.2 Comparar as fotos da entrega e da devolução; 1.3 Ler os relatos e as provas das duas partes; 1.4 Pedir mais provas a uma das partes | `1.1 > (1.2 + 1.3) > 1.4` |
| **2. Decidir a solução do problema** | 2.1 Decidir devolver a garantia a quem alugou ou 2.2 Decidir indenizar o dono com a garantia; 2.3 Registrar o motivo da decisão; 2.4 Suspender a conta | `(2.1 / 2.2) > 2.3 > 2.4` |
| **3. Enviar a decisão às duas partes** | Tarefa simples, sem subtarefas | n/a |

**Decisões e fluxo.** O suporte abre o caso, confronta as fotos do [HTA 7](#hta-7-realizar-a-entrega-do-equipamento) e do [HTA 8](#hta-8-concluir-a-devolução-do-equipamento) com os relatos das duas partes e, se necessário, pede mais provas. A decisão central é como destinar a garantia: devolvê-la a quem alugou ou usá-la para indenizar o dono. O motivo é registrado para dar transparência, e a decisão é enviada às duas partes, que a recebem no passo 5 do [HTA 9](#hta-9-resolver-um-problema-no-aluguel).

---

### HTA 11: Avaliar e ver reputação

<img src="imagem/HTA de avaliação.png" alt="Mapa de objetivos e HTA: Avaliar e ver reputação" width="900">

**Propósito.** Construir confiança entre os usuários, permitindo avaliar quem participou de um aluguel e consultar a reputação de qualquer pessoa.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Avaliar a outra pessoa** | 1.1 Abrir o aluguel concluído; 1.2 Dar uma nota à pessoa; 1.3 Marcar critérios rápidos (1.3.1 pontualidade e 1.3.2 item bem cuidado); 1.4 Escrever um comentário; 1.5 Enviar a avaliação | `1.1 > (1.2 + 1.3 + 1.4) > 1.5` e `1.3.1 + 1.3.2` |
| **2. Consultar o histórico e notas** | 2.1 Acessar o perfil de um usuário; 2.2 Ver a média de estrelas e o número de aluguéis concluídos; 2.3 Ler os comentários deixados por outros usuários | `2.1 > (2.2 + 2.3)` |

**Decisões e fluxo.** O usuário escolhe entre avaliar (1) e consultar (2). A avaliação parte de um aluguel concluído, e a nota, os critérios rápidos e o comentário são preenchidos em qualquer ordem antes do envio. A consulta começa no perfil e mostra a média, o total de aluguéis e os comentários, que alimentam a conferência da reputação feita nos HTAs [4](#hta-4-gerenciar-meus-anúncios-e-pedidos) e [5](#hta-5-encontrar-um-equipamento).

---

### HTA 12: Pedir e prestar ajuda

<img src="imagem/HTA de Ajudar.png" alt="Mapa de objetivos e HTA: Pedir e prestar ajuda" width="900">

**Propósito.** Oferecer ao usuário caminhos para tirar dúvidas, sozinho ou com o suporte, e descrever como o Suporte Técnico atende os pedidos.

| Tarefa | Subtarefas | Plano |
| :--- | :--- | :---: |
| **1. Entender como usar cada etapa** | 1.1 Abrir a ajuda; 1.2 Consultar as perguntas frequentes ou 1.3 Ver os guias passo a passo | `1.1 > (1.2 / 1.3)` |
| **2. Iniciar o contato com o suporte** | 2.1 Escolher "Falar com o suporte"; 2.2 Selecionar o assunto; 2.3 Indicar o aluguel relacionado; 2.4 Descrever a dúvida; 2.5 Enviar o pedido; 2.6 Ler a resposta do suporte | `2.1 > 2.2 > (2.3 + 2.4) > 2.5 > 2.6` |
| **3. Atender os pedidos de ajuda** (ST) | 3.1 Abrir o pedido de ajuda; 3.2 Ler o pedido e conferir a conta ou o aluguel; 3.3 Enviar a orientação ou 3.4 Encaminhar para a mediação; 3.5 Marcar o atendimento como concluído | `3.1 > 3.2 > (3.3 / 3.4) > 3.5` |

**Decisões e fluxo.** O plano `1 / (2 > 3)` mostra que o usuário primeiro tenta resolver sozinho (1) ou, se não conseguir, aciona o suporte (2), que então atende o pedido (3). No lado do suporte, a decisão é entre orientar diretamente (3.3) ou encaminhar para a mediação (3.4), que leva ao [HTA 10](#hta-10-analisar-e-resolver-disputas). O pedido só é encerrado quando o atendimento é marcado como concluído (3.5).

---

## Consistência com o Mapa de Objetivos

Cada HTA parte do objetivo final de um grupo do mapa (tarefa 0), e as tarefas de nível 1 correspondem aos objetivos ligados a ele. Isso garante que as tarefas derivam dos objetivos definidos, sem lacunas nem desvios. As tarefas de identidade do [HTA 3](#hta-3-colocar-um-equipamento-para-alugar) e do [HTA 6](#hta-6-alugar-um-equipamento) seguem o mesmo processo de verificação, e os HTAs [7](#hta-7-realizar-a-entrega-do-equipamento), [8](#hta-8-concluir-a-devolução-do-equipamento), [9](#hta-9-resolver-um-problema-no-aluguel) e [10](#hta-10-analisar-e-resolver-disputas) formam o encadeamento entre vistoria, devolução e mediação de problemas.
