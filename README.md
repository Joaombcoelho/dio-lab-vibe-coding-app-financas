# 💸 App de Finanças Pessoais Do João Manoel com Vibe Coding

PRD refinado no ChatGPT e usado para comparação Gemini.

```markdown
# PRD — FinanChat
## Organizador de Finanças Pessoais com Inteligência Artificial
**Versão:** 1.0
**Tipo de documento:** Product Requirements Document (PRD)
**Objetivo:** Planejamento de um MVP desenvolvido com Vibe Coding utilizando o Lovable.
**Idioma da aplicação:** Português brasileiro.
**Nome do produto:** FinanChat (provisório).
---
# 1. VISÃO GERAL DO PRODUTO

## 1.1. Contexto
O FinanChat será um aplicativo de organização de finanças pessoais que utiliza conversas em linguagem natural como principal forma de interação entre o usuário e um agente financeiro inteligente.
O projeto será desenvolvido com auxílio de ferramentas de inteligência artificial, utilizando a abordagem Vibe Coding para planejar, construir, testar e aprimorar a aplicação.
A proposta é simplificar o controle financeiro pessoal, permitindo que usuários registrem receitas e despesas, consultem seus gastos, acompanhem metas e recebam orientações educativas sem depender de planilhas ou formulários complexos.
O aplicativo deverá apresentar uma interface moderna, intuitiva, responsiva e acessível ao maior número possível de pessoas, seguindo os princípios de Design Universal.

## 1.2. Problema que queremos resolver
Muitas pessoas têm dificuldade em manter uma rotina de organização financeira porque os aplicativos tradicionais exigem muitos registros manuais, apresentam interfaces complexas e oferecem relatórios difíceis de interpretar.
O FinanChat pretende reduzir essas barreiras por meio de uma experiência conversacional simples, na qual o usuário possa organizar suas finanças utilizando a linguagem que já utiliza no dia a dia.

## 1.3. Proposta de valor
Permitir que qualquer pessoa tenha mais clareza sobre suas finanças pessoais conversando com um assistente inteligente, sem precisar dominar ferramentas financeiras ou preencher formulários extensos.

## 1.4. Público-alvo
O produto será direcionado principalmente a:
* Pessoas que estão começando a organizar suas finanças.
* Usuários que desejam controlar seus gastos de maneira prática.
* Pessoas com pouca experiência em aplicativos financeiros.
* Usuários que desejam criar metas e desenvolver hábitos financeiros melhores.
* Pessoas que preferem conversar em vez de preencher formulários.
A solução deverá considerar diferentes idades, níveis de alfabetização digital, habilidades e necessidades de acessibilidade.

## 1.5. Diferencial do produto
O chat deverá ser o centro da experiência, e não apenas um recurso adicional em um painel financeiro tradicional.
O agente deverá compreender solicitações, utilizar os dados registrados pelo usuário, executar operações autorizadas e apresentar resultados compreensíveis.
Exemplo:
Usuário: "Gastei R$ 32,50 no almoço hoje."
Agente: "Entendi! Você gastou R$ 32,50 com alimentação hoje. Deseja registrar essa despesa?"
Após a confirmação e a gravação bem-sucedida, o sistema deverá atualizar os indicadores financeiros e informar que o registro foi concluído.
Outro exemplo:
Usuário: "Quanto gastei com alimentação este mês?"
O agente deverá consultar as transações armazenadas e responder com os valores reais encontrados, sem inventar informações.
---

# 2. OBJETIVOS DO MVP
O MVP deverá demonstrar que uma experiência conversacional pode tornar o controle financeiro mais simples e acessível.
Os principais objetivos são:
1. Registrar receitas e despesas por meio de conversas.
2. Classificar transações automaticamente, permitindo correções.
3. Consultar informações financeiras utilizando linguagem natural.
4. Apresentar um resumo financeiro compreensível.
5. Criar e acompanhar metas de economia.
6. Fornecer recomendações educativas fundamentadas nos dados disponíveis.
7. Oferecer uma experiência consistente em dispositivos móveis e computadores.
8. Garantir que cada usuário tenha acesso somente aos próprios dados.
9. Validar a utilidade do produto com testes funcionais e, quando possível, usuários reais.
O MVP deverá priorizar poucos fluxos completos e confiáveis em vez de muitas funcionalidades parcialmente implementadas.
---

# 3. ESCOPO E PRIORIZAÇÃO DAS FUNCIONALIDADES
## 3.1. Funcionalidades essenciais — primeira versão
### F01. Autenticação e perfil
* Permitir cadastro, login e logout.
* Manter os dados associados ao usuário autenticado.
* Permitir acesso às informações pessoais somente mediante autorização.
* Oferecer uma experiência simples de primeiro acesso.
* Permitir encerrar a sessão com segurança.

### F02. Chat com o agente financeiro
* Disponibilizar uma interface de conversa como principal ponto de interação.
* Aceitar mensagens em português brasileiro.
* Interpretar solicitações relacionadas às finanças pessoais.
* Apresentar respostas claras e objetivas.
* Solicitar esclarecimentos quando faltarem informações necessárias.
* Exibir feedback sobre operações em andamento, concluídas ou com falha.
* Permitir consultar o histórico de conversas, quando disponível.

### F03. Registro de receitas e despesas

O sistema deverá interpretar mensagens como:

* "Gastei R$ 45 no supermercado."
* "Recebi R$ 2.500 de salário."
* "Paguei R$ 120 de energia ontem."
* "Gastei R$ 18,90 com transporte."
* "Recebi R$ 200 de um trabalho extra."

O agente deverá identificar:

* Tipo da transação: receita ou despesa.
* Valor monetário.
* Descrição.
* Data da transação.
* Categoria sugerida.
* Informações que ainda precisam ser confirmadas.

A transação somente será considerada registrada após a conclusão bem-sucedida da operação de gravação.

### F04. Categorização automática

Disponibilizar categorias iniciais, como:

* Alimentação.
* Moradia.
* Transporte.
* Saúde.
* Educação.
* Lazer.
* Compras.
* Contas e serviços.
* Salário.
* Renda extra.
* Outros.

As categorias deverão ser adequadas ao tipo de transação.

O usuário deverá conseguir corrigir uma classificação incorreta.

### F05. Dashboard financeiro

Apresentar um resumo com:

* Total de receitas do período.
* Total de despesas do período.
* Resultado financeiro do período.
* Quantidade de transações registradas.
* Distribuição de despesas por categoria.
* Progresso das metas financeiras.
* Atalho para iniciar uma conversa com o agente.

Os valores deverão ser calculados com base nas transações armazenadas.

O resultado financeiro do período será calculado pela diferença entre receitas e despesas daquele período. Não deverá ser apresentado como saldo bancário real.

### F06. Histórico de transações

Permitir:

* Visualizar receitas e despesas.
* Consultar transações por período.
* Filtrar por categoria e tipo.
* Consultar detalhes de uma transação.
* Editar transações.
* Excluir transações mediante confirmação.
* Atualizar os indicadores após alterações.

### F07. Metas financeiras

Permitir ao usuário:

* Criar uma meta com nome e valor desejado.
* Informar um prazo opcional.
* Acompanhar o progresso da meta.
* Consultar o valor restante para atingir o objetivo.
* Receber sugestões educativas para melhorar o planejamento.

O sistema deverá deixar claro que uma meta cadastrada não representa dinheiro efetivamente guardado em uma conta bancária.

### F08. Recomendações educativas

O agente poderá:

* Identificar categorias com despesas elevadas.
* Apresentar sugestões de economia.
* Ajudar o usuário a estabelecer metas realistas.
* Explicar conceitos financeiros básicos.
* Sugerir hábitos de organização financeira.

As recomendações deverão ser fundamentadas nos dados disponíveis.

Quando não houver dados suficientes, o agente deverá informar essa limitação e oferecer orientações gerais claramente identificadas como tais.

O agente não deverá inventar gastos, prometer resultados financeiros ou apresentar recomendações especulativas como certezas.

### F09. Relatórios simples

Permitir consultar:

* Receitas e despesas por período.
* Gastos por categoria.
* Comparação entre períodos, quando houver dados suficientes.
* Evolução das metas financeiras.

Os relatórios deverão incluir valores e descrições textuais, sem depender exclusivamente de gráficos.

### F10. Tratamento de erros

* Informar quando uma operação não puder ser concluída.
* Evitar confirmações falsas de gravação.
* Permitir que o usuário corrija informações.
* Impedir registros com valores inválidos.
* Tratar mensagens ambíguas de maneira segura.
* Oferecer uma alternativa clara quando a IA não compreender uma solicitação.

## 3.2. Funcionalidades futuras

As seguintes funcionalidades poderão ser consideradas após a validação do MVP:

* Transações recorrentes.
* Lembretes de vencimentos.
* Orçamentos mensais por categoria.
* Exportação de relatórios.
* Categorias personalizadas.
* Metas compartilhadas.
* Entrada por voz.
* Importação de extratos.
* Integração bancária autorizada.
* Aplicativo móvel nativo.
* Recursos adicionais de personalização e acessibilidade.

## 3.3. Fora do escopo inicial

Não deverão ser requisitos obrigatórios da primeira versão:

* Integração bancária automática.
* Movimentação de dinheiro.
* Pagamentos de contas.
* Compra e venda de investimentos.
* Concessão de crédito.
* Consultoria financeira profissional automatizada.
* Previsões financeiras apresentadas como garantias.
* Funcionalidades complexas de contabilidade.

---

# 4. TELAS E EXPERIÊNCIA DO USUÁRIO

## 4.1. Apresentação inicial

Objetivo: explicar o valor do FinanChat de maneira simples.

Componentes:

* Nome e identidade visual.
* Mensagem de apresentação.
* Benefícios principais.
* Botões de cadastro e login.
* Informações básicas sobre privacidade.

## 4.2. Autenticação

Objetivo: permitir o acesso seguro ao aplicativo.

Componentes:

* Campos de e-mail e senha.
* Opção de exibir a senha.
* Validação dos campos.
* Mensagens de erro acessíveis.
* Recuperação de senha, quando suportada.
* Links para cadastro e login.

## 4.3. Dashboard

Objetivo: oferecer uma visão rápida da situação financeira registrada.

Componentes:

* Saudação ao usuário.
* Seletor de período.
* Resumo de receitas e despesas.
* Resultado financeiro do período.
* Gastos por categoria.
* Metas em andamento.
* Transações recentes.
* Acesso destacado ao chat.

A tela deverá manter uma hierarquia visual clara, sem excesso de cartões ou informações concorrentes.

## 4.4. Chat financeiro

Objetivo: permitir que o usuário realize as principais operações por meio de linguagem natural.

Componentes:

* Histórico de mensagens.
* Campo de texto.
* Botão de envio.
* Sugestões de perguntas.
* Indicador de processamento.
* Resumos de transações identificadas.
* Controles de confirmação, correção e cancelamento.
* Mensagens de sucesso e erro.

Exemplos de sugestões:

* "Registrar uma despesa."
* "Quanto gastei este mês?"
* "Criar uma meta de economia."
* "Onde posso economizar?"

As sugestões deverão funcionar como atalhos, sem obrigar o usuário a utilizá-las.

## 4.5. Histórico de transações

Objetivo: permitir consultar e corrigir os registros financeiros.

Componentes:

* Lista de transações.
* Data, descrição, categoria e valor.
* Identificação visual de receitas e despesas.
* Filtros de período, categoria e tipo.
* Ações de edição e exclusão.
* Estado vazio com orientação para começar.

## 4.6. Metas financeiras

Objetivo: ajudar o usuário a acompanhar objetivos financeiros.

Componentes:

* Lista de metas.
* Nome e valor desejado.
* Prazo opcional.
* Progresso.
* Valor restante.
* Ação para criar ou editar uma meta.

O método utilizado para calcular o progresso deverá ser claramente explicado. Não deverá pressupor que uma meta possui depósitos reais vinculados se essa funcionalidade não existir.

## 4.7. Relatórios

Objetivo: facilitar a compreensão dos padrões de receitas e despesas.

Componentes:

* Seleção de período.
* Resumo dos valores.
* Despesas por categoria.
* Comparações disponíveis.
* Gráficos acessíveis.
* Descrições textuais dos resultados.

## 4.8. Configurações e perfil

Objetivo: permitir gerenciar preferências e informações da conta.

Componentes:

* Dados básicos do perfil.
* Preferências visuais disponíveis.
* Tema claro ou escuro, se implementado.
* Opções de acessibilidade.
* Informações de privacidade.
* Logout.

## 4.9. Fluxo principal de utilização

1. O usuário acessa o aplicativo.
2. Realiza o cadastro ou login.
3. Visualiza uma apresentação simples do FinanChat.
4. Abre o chat.
5. Envia uma mensagem relatando uma receita ou despesa.
6. O agente interpreta a mensagem.
7. O sistema apresenta os dados identificados.
8. O usuário confirma ou corrige as informações.
9. O backend registra a transação.
10. O sistema informa o resultado da operação.
11. O dashboard e os relatórios refletem os dados atualizados.

Esse fluxo deverá funcionar de ponta a ponta antes da expansão para funcionalidades secundárias.

---

# 5. COMPORTAMENTO DO AGENTE FINANCEIRO

## 5.1. Papel do agente

O agente financeiro deverá funcionar como um assistente educativo e operacional, auxiliando o usuário na organização de suas finanças pessoais.

Deverá compreender solicitações em linguagem natural, consultar informações autorizadas, propor classificações e executar operações de acordo com as regras do sistema.

## 5.2. Intenções reconhecidas

O agente deverá identificar, no mínimo:

* Registro de despesa.
* Registro de receita.
* Consulta de gastos.
* Consulta de receitas.
* Consulta do resultado financeiro.
* Consulta de gastos por categoria.
* Criação de meta.
* Consulta de metas.
* Solicitação de recomendações.
* Correção de transação.
* Exclusão de transação.
* Solicitação não financeira ou não compreendida.

## 5.3. Interpretação de mensagens

O agente deverá extrair informações estruturadas da mensagem.

Exemplo:

Mensagem: "Paguei R$ 85 de internet ontem."

Interpretação esperada:

* Tipo: despesa.
* Valor: R$ 85,00.
* Descrição: internet.
* Categoria sugerida: contas e serviços.
* Data: dia anterior, de acordo com a data local aplicável.
* Estado: aguardando confirmação, quando exigida pelo fluxo.

## 5.4. Informações incompletas

Se o usuário escrever "Gastei no mercado", o agente deverá perguntar qual foi o valor antes de tentar registrar a transação.

Se o valor estiver presente, mas houver dúvida sobre a data ou a natureza da operação, deverá solicitar esclarecimento quando essa informação for necessária.

Não deverá inventar dados ausentes.

## 5.5. Confirmação de operações

A interpretação da IA deverá ser separada da persistência dos dados.

O sistema deverá:

1. Interpretar a mensagem.
2. Validar os dados.
3. Apresentar a transação para confirmação, conforme as regras definidas.
4. Executar a gravação após a autorização necessária.
5. Verificar o resultado do backend.
6. Informar o sucesso somente após a confirmação da gravação.

A exclusão de registros deverá exigir confirmação explícita.

## 5.6. Consultas financeiras

O agente deverá consultar os dados armazenados e utilizar funções ou consultas controladas do backend para calcular os resultados.

Não deverá utilizar apenas o texto da conversa como fonte de verdade.

Quando não houver dados suficientes para responder, deverá explicar a limitação.

## 5.7. Tratamento de duplicidade

O sistema deverá reduzir o risco de registrar a mesma transação duas vezes por causa de reenvios ou repetições de uma solicitação.

Quando houver suspeita de duplicidade, deverá solicitar confirmação adicional ou utilizar mecanismos técnicos de idempotência adequados ao fluxo.

Não deverá excluir automaticamente registros apenas porque possuem valores semelhantes.

## 5.8. Limites do agente

O agente não deverá:

* Inventar transações.
* Afirmar que uma operação foi salva sem confirmação do backend.
* Confundir resultado financeiro calculado com saldo bancário real.
* Acessar dados de outros usuários.
* Executar ações destrutivas sem a autorização necessária.
* Prometer que determinada estratégia garantirá economia.
* Apresentar informações financeiras incertas como fatos.

---

# 6. REGRAS DE NEGÓCIO

## RN01. Tipos de transação

Cada transação deverá ser identificada como receita ou despesa.

## RN02. Valores monetários

Os valores deverão ser positivos e armazenados utilizando um tipo numérico adequado à precisão monetária, evitando erros de ponto flutuante.

A moeda inicial será o real brasileiro (BRL).

## RN03. Datas

As datas deverão ser interpretadas no contexto local do usuário, utilizando o fuso horário configurado para a aplicação.

O sistema deverá evitar interpretações incorretas de expressões como "hoje", "ontem" e "semana passada".

## RN04. Categorias

Cada transação deverá possuir uma categoria válida, com possibilidade de classificação inicial como "Outros" quando não houver informação suficiente.

O usuário poderá corrigir a categoria.

## RN05. Resultado financeiro

O resultado do período será calculado pela seguinte fórmula:

Resultado financeiro = receitas registradas no período - despesas registradas no período.

Esse indicador não deverá ser apresentado como saldo bancário real.

## RN06. Atualização dos indicadores

Toda criação, edição ou exclusão de transação deverá refletir corretamente no dashboard, no histórico e nos relatórios.

## RN07. Metas

Cada meta deverá possuir um identificador, um nome, um valor desejado e, opcionalmente, um prazo.

O progresso deverá ser calculado conforme um método definido e comunicado ao usuário.

## RN08. Isolamento de dados

Cada usuário deverá acessar somente as próprias transações, metas, perfil e conversas privadas.

Essa regra deverá ser aplicada no backend e no banco de dados, e não apenas na interface.

## RN09. Exclusão

A exclusão de transações deverá solicitar confirmação e atualizar os indicadores após a conclusão bem-sucedida da operação.

## RN10. Integridade

As operações deverão validar os dados antes da gravação.

O sistema deverá apresentar mensagens claras quando houver falha de validação, indisponibilidade da IA ou erro de persistência.

---

# 7. DESIGN UNIVERSAL, ACESSIBILIDADE E USABILIDADE

## 7.1. Diretriz principal

O FinanChat deverá seguir os princípios de Design Universal (Design for All), buscando oferecer uma experiência de uso eficiente, intuitiva, confortável e acessível ao maior número possível de pessoas.

O objetivo é permitir que pessoas com diferentes idades, habilidades, níveis de alfabetização digital, condições de acesso e necessidades individuais utilizem o aplicativo com autonomia.

A acessibilidade deverá ser considerada desde a concepção da interface e da arquitetura, e não apenas como acabamento visual.

## 7.2. Simplicidade e linguagem

* Utilizar linguagem cotidiana e objetiva.
* Evitar termos financeiros desnecessariamente técnicos.
* Explicar conceitos quando necessário.
* Manter a navegação previsível.
* Reduzir etapas desnecessárias.
* Apresentar instruções claras.
* Evitar exigir comandos específicos no chat.

## 7.3. Acessibilidade visual

* Utilizar contraste adequado entre texto e fundo.
* Manter tipografia legível.
* Oferecer hierarquia visual consistente.
* Permitir ampliação do conteúdo sem perda de funcionalidades.
* Não utilizar somente cores para representar estados.
* Diferenciar receitas, despesas, erros e alertas por texto, ícones ou outros indicadores complementares.

## 7.4. Leitores de tela e tecnologias assistivas

* Utilizar elementos semânticos apropriados.
* Disponibilizar nomes acessíveis para controles interativos.
* Incluir textos alternativos em imagens relevantes.
* Garantir que campos de formulário possuam rótulos.
* Preservar a ordem lógica de leitura.
* Anunciar mensagens importantes de sucesso e erro quando aplicável.
* Evitar componentes personalizados que impeçam a navegação assistida.

## 7.5. Navegação por teclado

* Permitir navegar pelas funcionalidades principais sem mouse.
* Garantir foco de teclado visível.
* Manter uma ordem lógica de navegação.
* Permitir utilizar e enviar mensagens no chat por teclado.
* Evitar elementos inacessíveis ou dependentes exclusivamente de gestos.

## 7.6. Acessibilidade motora

* Oferecer áreas de toque confortáveis em dispositivos móveis.
* Evitar exigir movimentos excessivamente precisos.
* Não depender exclusivamente de arrastar e soltar.
* Disponibilizar alternativas para interações complexas.
* Evitar operações destrutivas acionadas acidentalmente.

## 7.7. Design responsivo

A aplicação deverá oferecer boa experiência em:

* Celulares.
* Tablets.
* Notebooks.
* Computadores de mesa.

O layout deverá adaptar-se aos diferentes tamanhos de tela sem ocultar funcionalidades essenciais ou exigir rolagem horizontal desnecessária.

## 7.8. Inclusão de diferentes perfis

O projeto deverá considerar especialmente:

* Pessoas idosas.
* Pessoas com baixa visão.
* Pessoas com daltonismo.
* Pessoas com dificuldades motoras.
* Pessoas com pouca familiaridade com tecnologia.
* Pessoas com diferentes níveis de compreensão de leitura.
* Usuários que acessam o aplicativo em dispositivos com telas pequenas.

Esses perfis deverão orientar as decisões de design sem presumir que todas as pessoas de um mesmo grupo possuem as mesmas necessidades.

## 7.9. Feedback e prevenção de erros

* Informar quando uma operação estiver em andamento.
* Confirmar quando uma transação tiver sido registrada.
* Apresentar mensagens de erro compreensíveis.
* Oferecer orientações para corrigir problemas.
* Permitir revisar dados antes da confirmação.
* Solicitar confirmação antes de exclusões.
* Preservar as informações digitadas quando ocorrer uma falha recuperável.

## 7.10. Personalização

Quando viável para o MVP, disponibilizar:

* Tema claro e escuro.
* Ajustes úteis de apresentação.
* Redução de animações.
* Preferências persistentes do usuário.

Esses recursos não deverão aumentar desnecessariamente a complexidade do aplicativo.

## 7.11. Visualização de dados

* Apresentar valores monetários de forma clara.
* Utilizar títulos e legendas nos gráficos.
* Disponibilizar descrições textuais dos principais resultados.
* Evitar gráficos excessivamente complexos.
* Não depender apenas de cores para transmitir informações.
* Manter os dados compreensíveis em telas pequenas.

## 7.12. Referência de acessibilidade

Utilizar as Diretrizes de Acessibilidade para Conteúdo Web (WCAG) 2.2 como referência, buscando o nível AA quando aplicável.

Não declarar conformidade integral sem realizar verificações e testes adequados.

## 7.13. Critérios de validação do design

Verificar se:

* As principais funcionalidades podem ser utilizadas por teclado.
* Os controles possuem identificação acessível.
* O foco de navegação é visível.
* O contraste e a legibilidade são adequados.
* Os gráficos possuem alternativas textuais.
* A aplicação funciona em diferentes tamanhos de tela.
* As mensagens são claras e compreensíveis.
* As transações podem ser corrigidas sem reiniciar todo o fluxo.
* Os componentes não dependem exclusivamente de cores, gestos ou animações.
* A experiência é compreensível para pessoas iniciantes em tecnologia.

Não adicionar recursos de acessibilidade apenas de maneira decorativa. Os recursos implementados deverão ser funcionais e testáveis.

---

# 8. IDENTIDADE VISUAL

A identidade visual deverá transmitir confiança, clareza, simplicidade e acolhimento.

## Diretrizes

* Estilo moderno e profissional.
* Layout organizado e consistente.
* Paleta de cores equilibrada.
* Tipografia legível.
* Ícones compreensíveis.
* Espaçamento adequado.
* Hierarquia visual clara.
* Componentes reutilizáveis.
* Animações discretas e não essenciais.
* Ausência de poluição visual.

Evitar um dashboard genérico composto por muitos cartões, gráficos e números sem hierarquia.

O chat deverá ter destaque visual e funcional, reforçando a proposta de organização financeira por conversas.

A aplicação deverá utilizar:

* Português brasileiro.
* Valores monetários em reais.
* Formatação consistente de moeda.
* Datas no padrão brasileiro.
* Mensagens e instruções claras.

---

# 9. ARQUITETURA E TECNOLOGIAS

## 9.1. Diretriz geral

Recomendar uma arquitetura simples, segura e compatível com o desenvolvimento utilizando Lovable.

A escolha das tecnologias deverá considerar rapidez de implementação, manutenção, segurança, custos e possibilidade de evolução.

## 9.2. Interface

Desenvolver uma aplicação web responsiva, priorizando a experiência em dispositivos móveis e mantendo boa usabilidade em computadores.

A interface deverá utilizar componentes reutilizáveis e uma estrutura consistente.

## 9.3. Backend e banco de dados

Avaliar a utilização do Supabase como backend, incluindo:

* PostgreSQL.
* Autenticação.
* Persistência das transações.
* Persistência das metas.
* Armazenamento do histórico de conversas, quando necessário.
* Políticas de Row Level Security (RLS).
* Regras de acesso por usuário.

A escolha final deverá ser justificada com base nos requisitos do MVP.

## 9.4. Integração com IA

A aplicação poderá utilizar um modelo de linguagem para interpretar mensagens e produzir respostas.

A integração deverá:

* Manter chaves de API fora do código público do frontend.
* Utilizar mecanismos seguros de acesso ao provedor.
* Validar os dados retornados pelo modelo.
* Separar interpretação de execução.
* Utilizar operações controladas para consultar e modificar dados.
* Não permitir que o modelo ignore as regras de autorização do backend.
* Informar quando o serviço de IA estiver indisponível.

## 9.5. Segurança

* Implementar autenticação adequada.
* Isolar os dados dos usuários.
* Aplicar políticas de acesso no banco de dados.
* Validar dados no backend.
* Evitar exposição de segredos.
* Tratar erros sem revelar informações sensíveis.
* Restringir o acesso às operações financeiras.
* Evitar registrar dados pessoais desnecessários em logs.

## 9.6. Privacidade e LGPD

O aplicativo deverá considerar os princípios da Lei Geral de Proteção de Dados Pessoais (LGPD).

Deverá:

* Explicar quais dados são armazenados e para qual finalidade.
* Limitar a coleta ao necessário para o funcionamento.
* Restringir o acesso às informações pessoais.
* Evitar compartilhar dados financeiros com serviços externos sem necessidade e transparência.
* Considerar os direitos dos titulares dos dados.
* Prever formas apropriadas de exclusão de dados pessoais.
* Documentar as dependências externas que processam informações.

As medidas específicas deverão ser avaliadas conforme a arquitetura e os serviços efetivamente utilizados.

## 9.7. Custos e dependências

Antes da implementação, identificar:

* Necessidade de plano pago.
* Limites dos serviços utilizados.
* Custos potenciais de chamadas à IA.
* Dependência de provedores externos.
* Recursos disponíveis nos planos escolhidos.
* Alternativas para desenvolvimento e demonstração com baixo custo.

Não presumir que integrações ou funcionalidades pagas estarão disponíveis gratuitamente.

## 9.8. Dados demonstrativos

Quando necessário, utilizar dados fictícios claramente identificados.

Esses dados deverão ser separados das informações reais do usuário e não poderão ser apresentados como registros financeiros verdadeiros.

O MVP não deverá depender de integração bancária real.

---

# 10. PLANO DE IMPLEMENTAÇÃO

A implementação deverá ocorrer em etapas pequenas, verificáveis e priorizadas.

## Etapa 1 — Planejamento e arquitetura

Objetivo: validar o escopo, as tecnologias e as principais decisões do produto.

Entregáveis:

* Estrutura de telas.
* Fluxos de navegação.
* Arquitetura recomendada.
* Modelo de dados inicial.
* Regras de negócio.
* Identidade visual preliminar.

Critério de conclusão: plano aprovado antes de iniciar a implementação completa.

## Etapa 2 — Interface e navegação

Objetivo: criar a estrutura visual da aplicação.

Entregáveis:

* Apresentação inicial.
* Autenticação.
* Dashboard.
* Chat.
* Histórico.
* Metas.
* Relatórios.
* Configurações.

Critério de conclusão: navegação consistente, responsiva e acessível entre as principais telas.

## Etapa 3 — Backend e autenticação

Objetivo: implementar persistência e isolamento de dados.

Entregáveis:

* Banco de dados.
* Autenticação.
* Tabelas e relacionamentos.
* Políticas de acesso.
* Validação das operações.

Critério de conclusão: cada usuário consegue acessar e modificar somente os dados autorizados.

## Etapa 4 — Transações financeiras

Objetivo: implementar os fluxos de receitas e despesas.

Entregáveis:

* Criação de transações.
* Edição e exclusão.
* Categorias.
* Validação.
* Atualização dos indicadores.

Critério de conclusão: as operações funcionam corretamente e os dados permanecem consistentes após recarregar a aplicação.

## Etapa 5 — Agente financeiro

Objetivo: integrar o chat ao backend.

Entregáveis:

* Interpretação de mensagens.
* Identificação de intenções.
* Extração de informações.
* Confirmação de operações.
* Consultas financeiras.
* Tratamento de erros.
* Mensagens de feedback.

Critério de conclusão: o agente executa corretamente os fluxos prioritários utilizando os dados persistidos.

## Etapa 6 — Metas e relatórios

Objetivo: permitir acompanhamento e interpretação dos dados financeiros.

Entregáveis:

* Criação de metas.
* Cálculo de progresso.
* Relatórios por categoria.
* Consultas por período.
* Recomendações educativas.

Critério de conclusão: os resultados são consistentes com as transações registradas.

## Etapa 7 — Acessibilidade e qualidade

Objetivo: verificar usabilidade, acessibilidade e estabilidade.

Entregáveis:

* Revisão responsiva.
* Verificação de contraste.
* Testes de teclado.
* Testes de leitores de tela quando possível.
* Revisão das mensagens.
* Testes de regras de negócio.
* Correção dos problemas encontrados.

Critério de conclusão: os fluxos essenciais passam pelos testes definidos e os problemas identificados são documentados.

## Etapa 8 — Validação do MVP

Objetivo: verificar se a solução resolve o problema proposto.

Entregáveis:

* Roteiro de testes.
* Evidências dos testes.
* Feedback dos participantes, quando disponível.
* Lista de melhorias.
* Resumo dos resultados observados.

Critério de conclusão: relatório que diferencia resultados reais, limitações conhecidas e hipóteses ainda não validadas.

---

# 11. PLANO DE VALIDAÇÃO INICIAL

## 11.1. Hipóteses

H1: registrar transações por conversa é mais simples para o público-alvo do que preencher formulários tradicionais.

H2: o usuário consegue compreender os principais indicadores financeiros sem orientação técnica.

H3: o agente consegue interpretar corretamente mensagens comuns de receitas e despesas.

H4: uma interface acessível e previsível reduz as dificuldades de uso.

H5: os usuários compreendem a diferença entre resultado financeiro calculado e saldo bancário real.

Essas hipóteses deverão ser testadas. Não devem ser apresentadas como resultados já comprovados.

## 11.2. Participantes

Quando possível, convidar pessoas com diferentes níveis de familiaridade com tecnologia e organização financeira.

Buscar diversidade de idade e necessidades de acessibilidade, respeitando a participação voluntária e a privacidade.

## 11.3. Tarefas de teste

Solicitar aos participantes que:

1. Acessem o aplicativo.
2. Registrem uma despesa por conversa.
3. Registrem uma receita.
4. Consultem gastos por categoria.
5. Corrijam uma transação.
6. Criem uma meta financeira.
7. Consultem o progresso da meta.
8. Localizem o resumo financeiro mensal.

## 11.4. Perguntas de avaliação

* Foi fácil entender como utilizar o aplicativo?
* O registro por conversa foi intuitivo?
* As respostas do agente foram claras?
* Você conseguiu corrigir informações?
* Os indicadores financeiros foram compreensíveis?
* Alguma etapa causou confusão?
* Você utilizaria esse aplicativo para organizar suas finanças?
* O que deveria ser melhorado primeiro?

## 11.5. Indicadores

Medir, quando aplicável:

* Percentual de tarefas concluídas.
* Tempo necessário para concluir cada tarefa.
* Quantidade de erros.
* Quantidade de solicitações que exigiram ajuda.
* Percepção de facilidade de uso.
* Problemas de acessibilidade identificados.
* Precisão das interpretações do agente em um conjunto de testes definido.

Os resultados deverão ser registrados somente após os testes serem realizados.

## 11.6. Testes funcionais

Criar cenários para:

* Registro de receitas.
* Registro de despesas.
* Valores inválidos.
* Mensagens ambíguas.
* Datas relativas.
* Tentativas de duplicação.
* Edição de transações.
* Exclusão de transações.
* Falha na gravação.
* Indisponibilidade da IA.
* Isolamento de dados entre usuários.
* Atualização dos indicadores.
* Criação e acompanhamento de metas.

---

# 12. CRITÉRIOS DE ACEITAÇÃO DO MVP

O MVP será considerado funcional quando os seguintes critérios forem atendidos:

CA01. O usuário consegue realizar autenticação.

CA02. O usuário consegue registrar uma despesa por meio de uma conversa.

CA03. O usuário consegue registrar uma receita por meio de uma conversa.

CA04. O agente identifica corretamente valor, tipo, descrição, data e categoria quando as informações estão disponíveis.

CA05. O agente solicita esclarecimentos quando faltam informações essenciais.

CA06. A transação só é apresentada como registrada após confirmação da gravação.

CA07. O usuário consegue consultar receitas e despesas por período.

CA08. O usuário consegue consultar gastos por categoria.

CA09. O usuário consegue editar e excluir transações.

CA10. Os indicadores são atualizados após as alterações.

CA11. O usuário consegue criar e acompanhar uma meta financeira.

CA12. O agente utiliza os dados persistidos para responder às consultas financeiras.

CA13. O sistema apresenta mensagens claras quando uma operação falha.

CA14. Os dados de usuários diferentes permanecem isolados.

CA15. As telas principais funcionam em dispositivos móveis e computadores.

CA16. As funcionalidades essenciais podem ser utilizadas por teclado.

CA17. Os componentes interativos possuem identificação acessível.

CA18. As informações financeiras não dependem exclusivamente de cores ou gráficos.

CA19. O usuário consegue corrigir informações interpretadas incorretamente.

CA20. O sistema não apresenta dados fictícios como se fossem registros reais.

CA21. Os principais fluxos possuem testes funcionais documentados.

CA22. As limitações conhecidas do MVP são identificadas.

---

# 13. PRINCIPAIS RISCOS E MITIGAÇÕES

## Risco 1 — Chat superficial

Problema: o chat responde de maneira genérica, mas não executa operações reais.

Mitigação: implementar ferramentas controladas que conectem o agente ao backend e testar fluxos completos.

## Risco 2 — Interpretações incorretas

Problema: o agente identifica valores, datas ou categorias incorretamente.

Mitigação: validar os dados, apresentar resumos para confirmação e permitir correções.

## Risco 3 — Inconsistência financeira

Problema: dashboard, histórico e relatórios apresentam valores diferentes.

Mitigação: utilizar dados persistidos como fonte de verdade e centralizar as regras de cálculo.

## Risco 4 — Falhas de segurança

Problema: usuários conseguem acessar informações de outras contas.

Mitigação: implementar autenticação, autorização e políticas de acesso no backend e no banco de dados.

## Risco 5 — Acessibilidade insuficiente

Problema: pessoas com necessidades diferentes encontram barreiras para utilizar a aplicação.

Mitigação: adotar Design Universal desde o início, realizar testes de acessibilidade e corrigir os problemas identificados.

---

# 14. ORIENTAÇÕES PARA O LOVABLE

Durante o desenvolvimento:

1. Trabalhe em etapas pequenas e verificáveis.
2. Preserve as funcionalidades que já estiverem funcionando.
3. Antes de modificar estruturas importantes, explique brevemente o impacto da alteração.
4. Não considere uma funcionalidade concluída apenas porque a interface foi criada.
5. Verifique a persistência real dos dados.
6. Não simule sucesso quando uma operação falhar.
7. Priorize segurança, integridade dos dados e acessibilidade.
8. Utilize componentes reutilizáveis.
9. Evite adicionar dependências desnecessárias.
10. Informe limitações técnicas e dependências externas.
11. Não invente resultados de testes.
12. Corrija erros encontrados antes de ampliar desnecessariamente o escopo.
13. Mantenha a interface em português brasileiro.
14. Utilize dados fictícios apenas quando claramente identificados.
15. Não implemente integrações bancárias reais nesta etapa.

Se uma decisão técnica importante não estiver definida, apresente a opção recomendada e uma justificativa objetiva antes de implementá-la.

---

# 15. RESULTADO ESPERADO

Ao final do desenvolvimento do MVP, esperamos ter uma aplicação funcional que permita ao usuário organizar suas finanças pessoais por meio de conversas naturais.

O produto deverá reunir:

* Uma interface simples e acessível.
* Um agente financeiro conectado aos dados reais da aplicação.
* Registro e consulta de receitas e despesas.
* Categorização de transações.
* Dashboard financeiro.
* Histórico editável.
* Metas de economia.
* Relatórios simples.
* Recomendações educativas.
* Autenticação e isolamento de dados.
* Critérios documentados de qualidade e acessibilidade.

O sucesso do MVP deverá ser avaliado pela capacidade de executar os fluxos essenciais com consistência, pela facilidade de uso e pelos resultados efetivamente observados nos testes.

---

# 16. PRÓXIMOS PASSOS

Antes de iniciar a construção completa:

1. Analise este PRD e identifique eventuais inconsistências, dependências ou decisões que ainda precisam ser tomadas.
2. Apresente a arquitetura recomendada, o modelo de dados inicial e a sequência de implementação.
3. Identifique os requisitos essenciais de segurança, privacidade e Design Universal.
4. Sugira critérios para validar a primeira entrega.
5. Aguarde a aprovação do planejamento antes de implementar todas as funcionalidades.

A prioridade é construir primeiro um fluxo funcional de ponta a ponta: o usuário envia uma mensagem, o agente interpreta os dados, o usuário confirma a operação, o sistema registra a transação e os indicadores são atualizados corretamente.

A partir desse fluxo, o produto deverá evoluir de maneira incremental, mantendo a proposta central do FinanChat: tornar a organização financeira mais simples, inclusiva e acessível por meio de conversas naturais.
```
Interaçoes com o Lovable

> Crie um App de Finanças Pessoais com base no seguinte PRD (Product Requirements Document): (PRD)

  
- Prints ou pequenos vídeos das interações com a IA;  

> Sobre o projeto
O FinanChat é um aplicativo de organização de finanças pessoais desenvolvido com o objetivo de tornar o controle financeiro mais simples, intuitivo e acessível. A proposta é permitir que os usuários registrem receitas e despesas por meio de conversas em linguagem natural com um agente financeiro inteligente, reduzindo a necessidade de preenchimentos manuais e planilhas complexas.

A aplicação busca facilitar o acompanhamento dos gastos, a categorização das transações, a criação de metas financeiras e a visualização de relatórios, além de oferecer recomendações educativas para ajudar os usuários a compreender melhor suas finanças e identificar oportunidades de economia.

O projeto também prioriza o Design Universal, buscando proporcionar uma experiência inclusiva, responsiva e acessível para pessoas com diferentes idades, habilidades e níveis de familiaridade com a tecnologia.

Desenvolvido com o apoio de ferramentas de inteligência artificial por meio da abordagem Vibe Coding, o FinanChat faz parte de um desafio da DIO e tem como foco demonstrar como a IA pode auxiliar na criação de soluções digitais práticas para problemas do cotidiano.

- Uma breve **reflexão sobre o processo**:
  - O que funcionou bem?  
  - O que não funcionou como o esperado?  
  - O que aprendeu sobre conversar com IAs?

> [!TIP]
> Publique seu repositório e compartilhe o link na plataforma da DIO! Sua entrega é a prova de que você domina o raciocínio de Vibe Coding, mesmo sem escrever uma única linha de código.

## 💬 Conclusão

Vibe Coding é sobre clareza, curiosidade e criatividade, não sobre perfeição técnica. O verdadeiro objetivo aqui é aprender a pensar junto com a IA, transformando ideias em conceitos reais e enxergando a tecnologia como uma extensão do seu raciocínio criativo. Cada interação é um experimento, quanto mais clara for sua intenção, mais surpreendente será o resultado.
