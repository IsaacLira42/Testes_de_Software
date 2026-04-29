# Documentação de Problemas Encontrados: Home Page (Metodologia 2.5A)

## 📍 Sessão Hero

| ID      | Descrição do Problema                                          | Localização                                          | Sugestão de Melhoria                                                                 | Gravidade | Esforço |
| :------ | :------------------------------------------------------------- | :--------------------------------------------------- | :----------------------------------------------------------------------------------- | :-------- | :------ |
| **7.1** | Baixo contraste entre texto branco e imagem clara (FM11, AC4). | Título principal da Hero.                            | Aplicar um _overlay_ escurecido na imagem ou _text-shadow_ no título.                | Alta      | Leve    |
| **7.2** | Falta de texto alternativo em imagem complexa (AC1).           | Imagem de fundo da Hero.                             | Adicionar atributo `alt` descritivo da "viagem paradisíaca".                         | Média     | Leve    |
| **7.3** | Conflito de hierarquia entre botões (FM2).                     | Botões "Entrar" (topo) e "Crie uma viagem" (centro). | Reduzir o peso visual do botão "Entrar" (usar apenas contorno).                      | Média     | Leve    |
| **7.4** | Ambiguidade no termo "Viagem rápida" (CO1, CO3).               | Botão de call-to-action central.                     | Alterar para "Começar Roteiro Agora" para melhorar a _affordance_.                   | Baixa     | Leve    |
| **7.5** | Ausência de indicador de foco no menu (AC9, AC2).              | Links do cabeçalho flutuante.                        | Garantir que o estado `:focus` seja visualmente distinto para navegação via teclado. | Alta      | Leve    |

## 📍 Roteiros da Comunidade e Lugares Famosos

| ID      | Descrição do Problema                                | Localização                                     | Sugestão de Melhoria                                                             | Gravidade | Esforço  |
| :------ | :--------------------------------------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------- | :-------- | :------- |
| **8.1** | Falsa interatividade/Falso positivo (CO3, AF1).      | Cards que se movem mas não executam ação.       | Remover animação de _hover_ e cursor 'pointer' enquanto não houver link.         | Alta      | Leve     |
| **8.2** | Quebra de consistência interna de componentes (FM6). | Cards da Home (estáticos) vs Fluxo (clicáveis). | Padronizar o comportamento: se visualmente é um card de item, deve ser clicável. | Média     | Moderado |
| **8.3** | Microinteração de "curtida" sem feedback (CO2, AC9). | Ícone de coração nos cards.                     | Implementar mudança de cor (vermelho) e incremento numérico ao clicar.           | Média     | Leve     |
| **8.4** | Seção meramente decorativa sem exploração (PU5).     | Roteiros da Comunidade.                         | Vincular os perfis e cards a páginas de detalhes dos roteiros.                   | Média     | Grande   |

## 📍 Banner "Viaje da Melhor Forma" (CTA Final)

| ID      | Descrição do Problema                           | Localização                             | Sugestão de Melhoria                                                    | Gravidade | Esforço |
| :------ | :---------------------------------------------- | :-------------------------------------- | :---------------------------------------------------------------------- | :-------- | :------ |
| **9.1** | Botão de conversão inativo (AF1, CO3).          | Botão "Cadastre-se".                    | Vincular à rota de registro ou abrir modal de cadastro.                 | Alta      | Leve    |
| **9.2** | Uso de texto _placeholder_ (Lorem Ipsum) (CO6). | Descrição do banner de cadastro.        | Substituir por texto real que venda o valor e benefícios da plataforma. | Média     | Leve    |
| **9.3** | Espaçamento visual e vazio na composição (FM2). | Alinhamento de texto e botão no banner. | Centralizar ambos os elementos para manter o foco do olhar do usuário.  | Baixa     | Leve    |

## 📍 Sessão "O que estão dizendo" e Footer

| ID       | Descrição do Problema                                  | Localização                                      | Sugestão de Melhoria                                                      | Gravidade | Esforço  |
| :------- | :----------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------ | :-------- | :------- |
| **10.1** | Links estáticos em áreas de navegação (AF1, NA5).      | Link "Ver mais" e todos os links do rodapé.      | Implementar redirecionamentos funcionais para as páginas citadas.         | Alta      | Moderado |
| **10.2** | Falha de transparência em seções sensíveis (PS2, CO6). | Textos de "Privacidade" e "Segurança" no rodapé. | Substituir textos genéricos por políticas reais de proteção de dados.     | Alta      | Leve     |
| **10.3** | Ícones sociais vazios e sem identificação (AC1, FM4).  | Seção "Onde estamos" no Footer.                  | Inserir logotipos das redes e atributos `aria-label` para acessibilidade. | Média     | Leve     |

# Documentação de Problemas Encontrados (Metodologia 2.5A)

## 📍 Etapa 1: Planejamento Inicial

| ID      | Descrição do Problema                                          | Localização                                         | Sugestão de Melhoria                                           | Gravidade | Esforço |
| :------ | :------------------------------------------------------------- | :-------------------------------------------------- | :------------------------------------------------------------- | :-------- | :------ |
| **1.1** | Baixo contraste em textos de suporte e descrições (FM11, AC4). | "Planejando uma nova viagem" e descrição dos cards. | Escurecer o tom do cinza para atingir o índice 4.5:1.          | Alta      | Leve    |
| **1.2** | Falta de convite à ação (CTA) claro nos cards (CO3, CO2).      | Cards de categorias (Hospedagem, Lazer, etc).       | Adicionar botão "Selecionar" ou efeito de _hover_ destacado.   | Média     | Leve    |
| **1.3** | Área de toque da _stepper_ reduzida para mobile (PD5).         | Ícones redondos de progresso no topo.               | Aumentar o espaçamento e a área clicável entre ícones.         | Média     | Leve    |
| **1.4** | Indicador de foco por teclado pouco visível (AC2, AC9).        | Cards e campos de entrada.                          | Implementar um contorno (:focus) visualmente distinto via CSS. | Alta      | Leve    |

## 📍 Etapa 2: Hospedagens

| ID      | Descrição do Problema                                                 | Localização                               | Sugestão de Melhoria                                                  | Gravidade | Esforço  |
| :------ | :-------------------------------------------------------------------- | :---------------------------------------- | :-------------------------------------------------------------------- | :-------- | :------- |
| **2.1** | Ambiguidade em ícones de filtro e ordenação (FM4).                    | Barra de pesquisa superior.               | Adicionar rótulos de texto ou indicação de filtro ativo.              | Baixa     | Leve     |
| **2.2** | Truncamento de nomes de estabelecimentos (FM1, FM2).                  | Títulos nos cards de hotéis.              | Permitir quebra de linha ou reduzir fonte para evitar ocultar o nome. | Média     | Moderado |
| **2.3** | Avaliações sem suporte para leitores de tela (AC1, AC9).              | Estrelas de avaliação nos cards.          | Incluir etiqueta numérica (ex: "4.5") ou Alt Text descritivo.         | Alta      | Leve     |
| **2.4** | Proximidade excessiva entre ações primárias e secundárias (AF9, PD5). | Modal: Botões "Selecionar" e "Favoritar". | Aumentar o distanciamento físico entre os botões.                     | Alta      | Leve     |
| **2.5** | Sobrecarga cognitiva por múltiplas barras de rolagem (FM1, NA5).      | Modal: Seção de avaliações dos usuários.  | Remover scroll interno individual; usar expansão ou scroll único.     | Média     | Moderado |

## 📍 Etapa 3: Lazer e Passeios

| ID      | Descrição do Problema                                         | Localização                                | Sugestão de Melhoria                                    | Gravidade | Esforço  |
| :------ | :------------------------------------------------------------ | :----------------------------------------- | :------------------------------------------------------ | :-------- | :------- |
| **3.1** | Instrução de tarefa ambígua (CO3, NA1).                       | Texto "Selecione como deseja se divertir". | Especificar se a seleção é única ou múltipla.           | Média     | Leve     |
| **3.2** | Falta de feedback sobre a composição do orçamento (CO2, AF1). | Orçamento necessário (topo direito).       | Adicionar detalhamento (ex: "Hospedagem + Passeio").    | Baixa     | Moderado |
| **3.3** | Ícone de progresso descontextualizado (FM5, CO6).             | Ícone de roda-gigante na _stepper_.        | Usar ícone mais genérico de lazer (ex: câmera ou mapa). | Baixa     | Leve     |
| **3.4** | Fluxo de navegação sem confirmação explícita (NA5, AF9).      | Final da listagem de lazer.                | Incluir botão "Confirmar e Próximo".                    | Alta      | Leve     |

## 📍 Etapas 4 e 5: Gastronomia e Transporte

_Nota: Estas etapas apresentam padrões de interface idênticos às etapas 2 e 3, replicando os seguintes problemas:_

| ID      | Descrição do Problema                          | Localização                                                 | Sugestão de Melhoria                                                               | Gravidade | Esforço  |
| :------ | :--------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------- | :-------- | :------- |
| **4.1** | Reincidência de baixo contraste (FM11, AC4).   | Valores de preços e textos descritivos dos pratos/veículos. | Escurecer o tom do cinza para garantir leitura em ambientes externos.              | Alta      | Leve     |
| **4.2** | Persistência de nomes truncados (FM1, FM2).    | Títulos nos cards de restaurantes e frotas.                 | Ajustar o CSS para permitir nomes completos ou usar _tooltips_.                    | Média     | Moderado |
| **4.3** | Ambiguidade no fluxo de seleção (CO3, NA1).    | Telas de listagem de gastronomia e transporte.              | Clarificar se o usuário está escolhendo uma refeição/ticket ou montando um pacote. | Média     | Leve     |
| **4.4** | Falta de botão de avanço explícito (NA5, AF9). | Rodapé das listagens.                                       | Incluir botão "Confirmar Seleção" para evitar dependência exclusiva da _stepper_.  | Alta      | Leve     |

## 📍 Etapa 6: Salvamento e Encerramento (Final)

| ID      | Descrição do Problema                             | Localização                            | Sugestão de Melhoria                                                    | Gravidade | Esforço |
| :------ | :------------------------------------------------ | :------------------------------------- | :---------------------------------------------------------------------- | :-------- | :------ |
| **6.1** | Privacidade sem transparência textual (PS1, PS2). | Switch de "Visibilidade".              | Adicionar os rótulos "Público" e "Privado" de forma visível.            | Alta      | Leve    |
| **6.2** | **Inversão crítica de botões** (FM5, PD5, AF9).   | Botões "Salvar" e "Descartar".         | Mover "Salvar" para a direita e "Descartar" para a esquerda.            | Alta      | Leve    |
| **6.3** | Hierarquia visual confusa no sucesso (NA5, FM2).  | Modal de encerramento.                 | Destacar o botão "Ver Viagem" como ação principal (preenchido).         | Média     | Leve    |
| **6.4** | Ícone de conclusão inconsistente (FM5).           | Botão "Ver Viagem" com ícone de check. | Substituir por ícone de "Olho" ou "Seta", condizentes com visualização. | Baixa     | Leve    |
