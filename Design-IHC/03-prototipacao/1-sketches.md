# Sketches: ItAluga


Os sketches são protótipos de **baixa fidelidade**, sem cores e sem interação, que representam o início do design visual do ItAluga. Cada tela deriva de uma cena dos [diagramas MoLIC](../02-ideacao/5-molic.md) e das tarefas dos [HTAs](../02-ideacao/4-htas.md). Foram feitos no Draw.io.

Os sketches cobrem seis fluxos, distribuídos em **11 imagens**. Para o fluxo de **Criar conta**, foram feitas duas versões alternativas (A e B), e a equipe escolheu a **versão A**.

## Relação entre os fluxos, imagens e modelos

| **#** | **Fluxo** | **Imagem** | **MoLIC** | **HTA** |
| ----- | --------- | :--------: | --------- | ------- |
| 1 | [Criar conta](#1-criar-conta) (versões A e B) | 2 | [1.1 Cadastro](../02-ideacao/5-molic.md#11-criar-minha-conta-cadastro) | [HTA 1](../02-ideacao/4-htas.md#hta-1-criar-minha-conta) |
| 2 | [Recuperar senha](#2-recuperar-senha) | 2 | [1.3 Recuperar senha](../02-ideacao/5-molic.md#13-recuperar-minha-senha) | [HTA 2](../02-ideacao/4-htas.md#hta-2-entrar-na-minha-conta) |
| 3 | [Entrar e ajustar acessibilidade](#3-entrar-e-ajustar-acessibilidade) | 1 | [1.2 Acesso](../02-ideacao/5-molic.md#12-entrar-no-sistema-e-ajustar-acessibilidade-acesso) | [HTA 2](../02-ideacao/4-htas.md#hta-2-entrar-na-minha-conta) |
| 4 | [Buscar e alugar equipamento](#4-buscar-e-alugar-equipamento) | 2 | [3.1 Buscar e alugar](../02-ideacao/5-molic.md#31-buscar-e-alugar-equipamento) | [HTA 5](../02-ideacao/4-htas.md#hta-5-encontrar-um-equipamento), [HTA 6](../02-ideacao/4-htas.md#hta-6-alugar-um-equipamento) |
| 5 | [Anunciar equipamento](#5-anunciar-equipamento) | 3 | [2.1 Anunciar](../02-ideacao/5-molic.md#21-anunciar-equipamento) | [HTA 3](../02-ideacao/4-htas.md#hta-3-colocar-um-equipamento-para-alugar) |
| 6 | [Gerenciar anúncios e pedidos](#6-gerenciar-anúncios-e-pedidos) | 2 | [2.2 Gerenciar](../02-ideacao/5-molic.md#22-gerenciar-anúncios-e-pedidos) | [HTA 4](../02-ideacao/4-htas.md#hta-4-gerenciar-meus-anúncios-e-pedidos) |

---

## 1. Criar conta

Fluxo de cadastro: o usuário parte do login, informa seus dados, confirma o telefone com um código e define a senha. Ao final, volta ao login para entrar com a conta nova.

### Versão A (escolhida)

<div align="center">
  <a href="imagem/SKETCHES%201(tela%20A).png">
    <img src="imagem/SKETCHES%201(tela%20A).png" alt="Sketch: Criar conta, versão A" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Login | Logo, telefone, senha, **Entrar**, links *Criar conta* e *Recuperar senha* | Identificar-me |
| Cadastro | Nome completo, telefone, caixa *Aceito os termos*, **Continuar** | Informar meus dados |
| Confirmar contato | Quatro campos para o código, **Confirmar código**, link *Reenviar código* | Confirmar meu contato |
| Definir senha | Nova senha, confirmar senha, regras da senha (mínimo de 8 caracteres, 1 maiúscula, 1 número), **Continuar** | Definir minha senha |
| Conta criada | Ícone de confirmação, mensagem *Conta criada!* e **Entrar** | Cadastro concluído com sucesso, seguido de Identificar-me |

### Versão B (alternativa)

<div align="center">
  <a href="imagem/SKETCHES%201(tela%20B).png">
    <img src="imagem/SKETCHES%201(tela%20B).png" alt="Sketch: Criar conta, versão B" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

A versão B reúne o cadastro e a definição da senha em **uma única tela**, o que reduz o fluxo de cinco para quatro telas.

### Por que a versão A foi escolhida

| Critério | Versão A | Versão B |
| :--- | :--- | :--- |
| Correspondência com o MoLIC | Três telas de preenchimento, uma para cada cena (Informar dados, Confirmar contato, Definir senha) | Junta duas cenas em uma, e o diagrama precisaria ser alterado |
| Usabilidade | Poucos campos por tela, com um objetivo por vez | Seis elementos de preenchimento na mesma tela, com as regras da senha e os termos juntos |
| Comunicabilidade | As regras da senha aparecem na tela em que ela é criada | As regras ficam no meio do formulário, longe do campo a que se referem |
| Experiência do usuário | O progresso é visível passo a passo, o que passa segurança a quem tem pouca familiaridade com aplicativos | Mais rápida, mas a tela fica mais carregada |

---

## 2. Recuperar senha

Fluxo para quem esqueceu a senha: o usuário informa o telefone, confirma o código recebido e define uma nova senha. Ao final, volta ao login.

<div align="center">
  <a href="imagem/SKETCHES%202.png">
    <img src="imagem/SKETCHES%202.png" alt="Sketch: Recuperar senha" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Recuperar senha | Texto explicativo, campo de telefone, **Enviar código** | Identificar minha conta |
| Confirmar contato | Aviso do destino do código, campos do código, **Prosseguir**, links *Reenviar código* e *Alterar telefone* (volta à tela anterior) | Confirmar meu contato |
| Nova senha | Regras da senha, nova senha, confirmar senha, **Redefinir senha** | Definir nova senha |
| Senha redefinida | Ícone de confirmação, mensagem e **Entrar** (leva ao login) | Senha redefinida com sucesso, seguido de Identificar-me |

### Mensagens de erro

<div align="center">
  <a href="imagem/SKETCHES%203.png">
    <img src="imagem/SKETCHES%203.png" alt="Sketch: Recuperar senha, mensagens de erro" width="900">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

Cada erro previsto no MoLIC aparece em um aviso fixo no topo da tela em que ocorreu, com ícone de alerta e fundo cinza, e o usuário permanece na mesma tela para corrigir.

| Tela | Mensagem | Transição do MoLIC |
| :--- | :--- | :--- |
| Recuperar senha | Telefone não cadastrado ou falha no envio | **d:** informa e volta |
| Confirmar contato | Código incorreto ou expirado | **d:** informa e volta |
| Nova senha | As senhas não são iguais ou fogem das regras | **d:** informa e volta |

---

## 3. Entrar e ajustar acessibilidade

Fluxo de login com os recursos de apoio. No primeiro acesso, o usuário decide se quer adaptar a tela. Se já tiver uma preferência definida, o fluxo segue direto para a lista de equipamentos.

<div align="center">
  <a href="imagem/SKETCHES%205.png">
    <img src="imagem/SKETCHES%205.png" alt="Sketch: Entrar e ajustar acessibilidade" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Login | Logo, telefone, senha, **Entrar**, links *Criar conta* e *Recuperar senha* | Identificar-me |
| Acessibilidade | Lista dos recursos disponíveis, **Adaptar a tela** e **Manter padrão** | Decidir sobre acessibilidade |
| Recursos de apoio | Caixas de seleção: alto contraste, texto ampliado e leitura por voz, e **Aplicar recursos** | Escolher recursos de apoio |
| Prévia | Exemplo de texto com os recursos ativos, botão *Ouvir*, **Aprovar e continuar** e link *Alterar recursos* | Conferir layout adaptado |
| Equipamentos | Busca, categorias, lista de equipamentos e botão **Aa** no topo | Pesquisar equipamentos |

O botão **Aa** no topo da última tela representa o acesso ubíquo do MoLIC, que permite abrir a acessibilidade a qualquer momento. As setas rotuladas mostram os caminhos *Preferência já definida*, *Manter padrão* e *Alterar recursos*.

---

## 4. Buscar e alugar equipamento

Fluxo do locatário: busca o equipamento, vê os resultados, examina o anúncio, confirma a identidade e envia a solicitação ao locador. Foram feitas duas versões alternativas (A e B).

### Versão A

<div align="center">
  <a href="imagem/SKETCHES%204.png">
    <img src="imagem/SKETCHES%204.png" alt="Sketch: Buscar e alugar equipamentos, versão A" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Busca | Campo de busca, categorias (Construção, Manutenção, Outros), filtros, **Buscar** e menu inferior | Pesquisar equipamentos |
| Resultados | Quantidade de resultados e lista com foto, diária, nota e favoritar | Examinar resultados da busca |
| Detalhe do equipamento | Fotos, nota, diária, descrição e regras de uso, disponibilidade e **Solicitar aluguel** | Examinar anúncio |
| Confirme sua identidade | Foto do RG/CNH, reconhecimento facial e comprovante de residência | Confirmar minha identidade |
| Aluguel solicitado | Confirmação, resumo do pedido (período, produto, total) e **Voltar pro início** | Pedir aluguel, seguido de Acompanhar resposta do locador |

### Versão B

<div align="center">
  <a href="imagem/sketches versao b.png">
    <img src="imagem/sketches versao b.png" alt="Sketch: Buscar e alugar equipamentos, versão B" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

A versão B reúne a busca e os resultados em **uma única tela**, o que reduz o fluxo de cinco para quatro telas. O resumo do pedido passa para a tela de confirmação de identidade, e a tela final fica só com a confirmação.

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Buscar | Campo de busca, categorias (Construção, Manutenção, Outros), quantidade de resultados, **Filtros**, lista com foto, diária, nota e favoritar, e menu inferior | Pesquisar equipamentos e Examinar resultados da busca |
| Detalhe do equipamento | Fotos, favoritar, nota, descrição e regras de uso, disponibilidade, diária e **Solicitar aluguel** | Examinar anúncio |
| Confirme sua identidade | Detalhes do pedido (período, produto, total), foto do RG/CNH, reconhecimento facial, comprovante de residência e **Prosseguir** | Confirmar minha identidade |
| Aluguel solicitado | Ícone de confirmação, mensagem *Seu pedido foi enviado para o locador* e **Voltar pro início** | Pedir aluguel, seguido de Acompanhar resposta do locador |
---

## 5. Anunciar equipamento

Fluxo do locador: descreve o equipamento, define preços e regras, confirma a identidade (só se ainda não foi validada), aguarda a aprovação e publica o anúncio.

### Parte 1 de 2

<div align="center">
  <a href="imagem/SKETCHES%206.png">
    <img src="imagem/SKETCHES%206.png" alt="Sketch: Anunciar equipamento, parte 1" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Meu equipamento | Campos numerados: categoria, fotos (câmera ou arquivo), título e descrição, estado de conservação | Mostrar equipamento e seu estado |
| Preços e regras | Valor da diária, prazo máximo de locação, valor da caução, bairro ou local de retirada | Definir preços e regras do aluguel |
| Confirme sua identidade | Foto do RG/CNH, reconhecimento facial e comprovante de residência | Confirmar identidade |

As anotações mostram a bifurcação do MoLIC: com a identidade **já validada**, o fluxo vai direto a *Revisar anúncio*. Caso contrário, passa pela confirmação de identidade.

### Parte 2 de 2

<div align="center">
  <a href="imagem/SKETCHES%207.png">
    <img src="imagem/SKETCHES%207.png" alt="Sketch: Anunciar equipamento, parte 2" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Documentos em análise | Situação de cada documento (documento, selfie e comprovante) | Aguardar aprovação |
| Revisar anúncio | Resumo (categoria, fotos, preço e retirada), **Confirmar e ativar** e link *Alterar informações* | Revisar e publicar anúncio |
| Anúncio ativo | Confirmação, prévia do anúncio e **Concluir** | Ver anúncio ativo |

### Mensagens de erro

<div align="center">
  <a href="imagem/SKETCHES%208.png">
    <img src="imagem/SKETCHES%208.png" alt="Sketch: Anunciar equipamento, mensagens de erro" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Mensagem | Transição do MoLIC |
| :--- | :--- | :--- |
| Meu equipamento | Dados incompletos | **d:** informa e volta |
| Preços e regras | Valor ou prazo inválido | **d:** informa e volta |
| Confirmar identidade | Documento ilegível ou divergente. Envie de novo | **d:** informa e volta |
| Revisar anúncio | Falha ao publicar o anúncio. Tente de novo | **d:** informa e volta |

---

## 6. Gerenciar anúncios e pedidos

Painel do locador: mostra anúncios, aluguéis em andamento e solicitações recebidas, e permite editar ou excluir um anúncio.

### Parte 1 de 2

<div align="center">
  <a href="imagem/SKETCHES%209.png">
    <img src="imagem/SKETCHES%209.png" alt="Sketch: Gerenciar anúncios e pedidos, parte 1" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | Elementos principais | Cena do MoLIC |
| :--- | :--- | :--- |
| Meus anúncios | Anúncios ativos com status, aluguéis em andamento e solicitações recebidas com o botão **Abrir** | Acompanhar anúncios e aluguéis |
| Meu anúncio | Foto, título, status, condições, solicitações do anúncio, **Editar anúncio** e **Excluir anúncio** | Gerenciar anúncio ativo |
| Editar anúncio | Fotos, título, descrição, condições do aluguel (diária, prazo, caução, retirada) e **Salvar alterações** | Editar anúncio |

O botão **Abrir** de uma solicitação leva ao diagrama *Responder solicitação de aluguel*, indicado no sketch como cena de referência.

### Parte 2 de 2

<div align="center">
  <a href="imagem/SKETCHES%2010.png">
    <img src="imagem/SKETCHES%2010.png" alt="Sketch: Gerenciar anúncios e pedidos, parte 2" width="1000">
  </a>
  <br>
  <sub>Clique na imagem para abri-la em tamanho original.</sub>
</div>

| Tela | O que mostra | Transição do MoLIC |
| :--- | :--- | :--- |
| Confirmar exclusão | Diálogo sobre a tela escurecida: *Excluir anúncio?*, **Confirmar exclusão** e *Cancelar* | Confirmar exclusão |
| Não é possível excluir | Aviso de que há aluguel em andamento, com o botão **Entendi** | **d:** informa e impede |
| Anúncio excluído | Faixa de confirmação no topo da lista | **d: Anúncio excluído** |
| Dados incompletos | Aviso no topo da edição | **d:** informa e volta |

---

## Princípios de design aplicados

| Princípio | Como aparece nos sketches |
| :--- | :--- |
| **Usabilidade** | Um objetivo por tela e botão principal sempre preenchido e na parte de baixo. Seta de voltar no topo das telas de etapa. Campos numerados em *Anunciar* para mostrar a ordem do preenchimento. Menu inferior fixo nas telas de busca. |
| **Comunicabilidade** | Títulos que dizem o que a tela faz (*Confirme sua identidade*, *Revisar anúncio*). Regras da senha visíveis antes do erro. Erros no topo da tela, com ícone de alerta, dizendo o que corrigir. Confirmação antes de excluir. |
| **Experiência do usuário** | Telas de sucesso com ícone e mensagem curta (*Conta criada!*, *Anúncio ativo!*). Fluxos curtos, para dar segurança a quem tem pouca familiaridade com aplicativos. Recursos de acessibilidade oferecidos no primeiro acesso e disponíveis a qualquer momento. |
