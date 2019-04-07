## Lista de verificação de Acessibilidade para Aplicações Móveis

### Interação com o Utilizador

#### Tamanho do alvo de toque
- O tamanho do alvo de toque/clique DEVE ser suficientemente grande (sem usar ampliação) para que seja fácil de usar com um dedo, sem correr o risco de ativar um botão ou uma hiperligação adjacente.</li>

#### Espaçamento entre alvos de toque e agrupamento de alvos de toque
- Os alvos de toque NÃO PODEM sobrepôr-se.
- Os alvos de toque NÃO DEVEM estar adjacentemente colados uns aos outros.
- Os elementos adjacentes ativados com o mesmo alvo de toque DEVEM ser agrupados num só alvo de toque.

#### Despoletar a ação apenas ao libertar
- Os controlos de toque NÃO PODEM despoletar a ação assim que o item é tocado pela primeira vez. A ação é despoletada não quando o item é pressionado mas quando é libertado.

#### Motricidade/Acelerómetro
- Uma aplicação NÃO PODE depender apenas dos movimentos motores (detetados pelo acelerómetro).
- O utilizador DEVE ser capaz de desativar as funcionalidades sensíveis ao movimento.

#### Voz
- Uma aplicação NÃO PODE depender apenas do controlo pela voz.

#### Gestos
- Uma aplicação NÃO PODE depender apenas do controlo por gestos.
- Sempre que possível, as ações DEVEM ser mapeadas para os correspondentes gestos por defeito do dispositivo (iOS, Android).

### Controlos da Interface de Utilizador

#### Botões
- Um botão TEM sempre de transmitir o seu papel (role) usando a conceção correta que o objeto botão dispõe para o efeito.
- Uma imagem usada como um botão TEM de transmitir o papel (role) correto.
- Quando um botão está desativado, ele TEM de transmitir o seu estado (state).

#### Hiperligações
- O papel (role) e o propósito de uma hiperligação TEM de ser claramente transmitido aos utilizadores de leitores de ecrã (VoiceOver, Talks, ...).</li>

#### Barras de progresso
- As barras de progresso TÊM de transmitir o seu nome (name) aos leitores de ecrã (VoiceOver, talks) através de uma etiqueta única e descritiva.
- As roletas de progresso (spinners) TÊM de transmitir o texto alternativo correto ou receber imediatamente o foco de modo a transmitir um nome (name) acessível aos utilizadores de leitores de ecrã (VoiceOver no caso do iOS, Talks no caso do Android, ...).</li>

#### Controlos deslizantes (slider)
- Os controlos deslizantes TÊM de ter uma etiqueta visível que seja programaticamente associada usando a propriedade de acessibilidade etiqueta.

#### Interruptores (switch)
- Os controlos Interruptor (Switch) TÊM de ter uma etiqueta visível que seja programaticamente associada usando a propriedade de acessibilidade etiqueta.

### Notificações

#### Notificar os utilizadores do que acabou de ser modificado

- Conteúdo gerado dinamicamente que surge após interação do utilizador TEM de cumprir uma das seguintes permissas: a tecnologia de apoio é automaticamente informada do novo conteúdo OU o novo conteúdo é a coisa que a tecnologia de apoio vai encontrar imediatamente a seguir na página.</li>

#### Limites de tempo

- Se existe uma sessão limitada pelo tempo, os utilizadores TÊM de ser avisados antes da sessão terminar e TEM de ser dado tempo para guardar os seus dados e/ou estender a sessão.
- Os dados incompletos DEVEM ser guardados depois da sessão terminar.

#### Alertas

- Os alertas TÊM de incluir um título e uma descrição.</li>

#### Caixas de diálogo

- As caixas de diálogo personalizáveis TÊM de ter configurado o <code>accessibilityViewIsModal</code> para "true" e o foco TEM de ser enviado para o interior da caixa de diálogo.

### Elementos personalizáveis

#### Acordeons

- As componentes do tipo acordeon TÊM de disponibilizar o seu nome acessível e o seu estado expandido ou comprimido.

#### Auto-preenchimento

- Os utilizadores do VoiceOver TÊM de ficar conscientes da existência das sugestões de auto-preenchimento assim que elas surgem. 

#### Controlo de pontuação

- Os controlos de pontuação TÊM sempre de transmitir o seu valor atual, qualquer informação visível, e ser operável quer pelos utilizadores do VoiceOVer quer pelos utilizadores que não usam VoiceOver.

#### Tabela ordenável

- Se uma tabela dispõe de colunas ordenável, as etiquetas de acessibilidade das células cabeçalho TÊM de se atualizar dinamicamente para revelar corretamente o estado da ordem cada vez que a ordem da informação é alterada.

#### Interruptor ligado/desligado

- Os botões de interruptor TÊM de transmitir um nome acessível programaticamente associado com etiquetas visíveis e transmitir o seu estado usando a etiqueta acessível.
- Os botões imagem interruptor TÊM de ter um texto alternativo descritivo, disponível na etiqueta de acessibilidade.

### Validação e etiquetagem de formulários

#### Etiquetagem

- A etiqueta DEVE ser sempre visível.</li>
- As etiquetas DEVEM ser associadas programaticamente com os respetivos elementos de controlo.
- DEVE ser adicionada uma "dica" sempre que a etiqueta não transmita suficientemente o propósito do controlo para os utilizadores do VoiceOver.

#### Etiquetas de grupo

- Para grupos de controlos relacionados em que as etiquetas de cada controlo não forneça uma descrição suficiente, DEVE ser adicionada etiquetas de grupo.

#### Caixas de verificação

- As caixas de verificação DEVEM transmitir o seu estado verificado ou selecionado para o VoiceOver.
- Os grupos de caixas de verificação TÊM de fornecer um grupo comum etiquetado assim como uma etiqueta única para cada controlo através da sua etiqueta de acessibilidade existente nas propriedades.

#### Campos de edição para recolha de dados do tipo data

- Um campo de edição padrão para recolha de dados do tipo data DEVE ser usada em vez de um campo de texto de forma a evitar que os utilizadores sejam forçados a introduzir uma data com um teclado por defeito.

#### Botões do tipo Rádio

- Os botões de rádio TÊM de disponibilizar uma etiqueta de grupo comum assim como um etiqueta única para cada controlo das etiquetas de acessibilidade e TEM de transmitir o seu estado selecionado.

#### Select (UIPickerView)

- Os controlos que usam UIPickerView TÊM de estar programaticamente associados às respetivas etiquetas visíveis de forma a disponibilizar um nome acessível.

#### Campos de edição do tipo texto

- Os campos de texto TÊM de ter etiquetas visíveis, programaticamente associadas.

#### Validação e reporte de erros</h4>

- Na validação de formulários, as mensagens de erro e de informação adicional disponibilizada aos utilizadores DEVE ser composta por texto eficiente, intuitivo, claramente identificado baseado em alertas.
- Se os erros de entrada são automaticamente detetados, DEVEM ser disponibilizadas sugestões em texto para retificar a entrada rapidamente e de forma acessível antes da informação ser submetida ao servidor.

### Navegação

#### Títulos da página

- Os ecrãs TEM de ter títulos com significado.

#### Separadores e respetivos painéis

- Os separadores TÊM de transmitir aos utilizadores do VoiceOver o seu papel (role), o seu estado atual e a sua posição relativa no total dos separadores.

#### Menu

- Os itens do Menu TÊM de ter o perfil apropriado por forma a transmitir apropriadamente o seu papel (role) acessível.
- O botão que abre o menu TEM de ter um título claro, descritivo ou uma etiqueta de acessibilidade para transmitir apropriadamente o seu propósito.
- Os utilizadores de VoiceOver TÊM de ser capazes de ultrapassar o menu.
- Quando o menu é fechado, o foco TEM de voltar ao botão interruptor de abrir/fechar.

### Orientação do Dispositivo

- A orientação do conteúdo não PODE ser trancada à orientação retrato ou paisagem a não ser que uma orientação específica seja essencial para a funcionalidade da aplicação.

### Estrutura semântica e significante

#### Cabeçalhos

- Os cabeçalhos para titular ou descrever secções de conteúdo TÊM de usar o perfil de cabeçalho por forma a transmitir o seu propósito semântico.

#### Tabelas
<ul>
    <li>Data tables MUST have the correct reading order, MUST convey the row and column header text for each data cell, and MUST correctly associate the data cell with the header cell in the accessibility label.</li>
</ul>

#### Ordem de leitura e ordem de focagem
<ul>
    <li>The reading order of a screen as conveyed by VoiceOver MUST be logical and intuitive.</li>
    <li>When content is added or deleted from a screen, VoiceOver focus MUST be managed logically and never be lost.</li>
  </ul>

### Cor e Contraste

#### Cores que transmitem informação
<ul>
  <li>Any information conveyed by color MUST be accompanied by a programmatically-discernible text alternative.</li>
  <li>The text alternative for information conveyed by color MUST accurately convey the same information without color.</li>
  <li>Any information conveyed by color MUST be accompanied by a visible alternative (text, image, etc.) that does not depend on color for meaning.</li>
  <li>Color alone MUST NOT be used to distinguish links from surrounding text unless the color contrast between the link and the surrounding text is at least 3:1. An additional differentiation (e.g. underline, outline, etc.) SHOULD BE provided as well.</li>
</ul>

#### Contraste
- Texto pequeno (inferior a 18 pontos ou 14 pontos para texto em negrito) TEM de ter um rácio de contraste com o fundo de, no mínimo, 4.5 para 1.
- Texto grande e imagens de texto grande (superior ou igual a 18 pontos ou 14 pontos a negrito) TÊM de ter um rácio de contraste com o fundo de, pelo menos, 3 para 1.
- O contraste das margens dos controlos da Interface de Utilizador em comparação com as áreas adjacentes DEVEM ser suficientes (3 para 1 para as margens de controlo da IU que meçam, pelo menos, 3px por 3px, e 4.5 para 1 para todos os outros controlos da IU) de forma a que os controlos sejam distinguíveis das áreas adjacentes.

### Animações e Movimento
#### Paralaxe e Animações derivadas do acelerómetro
<ul>
  <li>Moving the physical device SHOULD NOT cause non-essential visual motion or animations (e.g. parallax effects)</li>
  <li>Users MUST be able to disable any non-essential motion-sensitive visual effects.</li>
</ul>

#### Movimentar ou esconder conteúdo
<ul>
  <li>Automatically moving, blinking, or scrolling content that lasts longer than 5 seconds MUST be able to be paused, stopped, or hidden by the user.</li>
</ul>

### Áudio e Vídeo
#### Legendagem
- Todo o vídeo pré-gravado TEM de ter legendagem sincronizada.
- Todo o multimédia de eventos ao vivo (vídeo mais áudio) que contenham diálogos e/ou narração TÊM de ser acompanhados por legendagem sincronizada.
- Áudio de eventos ao vivo que no essencial seja composto por diálogos e/ou narração DEVE ter legendagem sincronizada.

#### Transcrições
- Todo o vídeo e áudio pré-gravado TEM de ter transcrições em texto.

### Texto

#### Identificar idioma
- O idioma da página TEM de ser programaticamente identificável.
- O idioma das secções de conteúdo diferentes do idioma principal da aplicação TEM de ser marcado/identificado de forma a que possa ser descodificado pelas tecnologias de apoio.

#### Alterar o tamanho do texto
- O ecrã TEM de ser legível e funcional quando o texto é ajustado para os 200% em relação ao seu tamanho inicial.

#### Emojis
- Os Emojis PODEM ser usados no corpo do texto.
- Os emojis personalizáveis em teclados personalizáveis TÊM de ter texto alternativo.

### Imagens

#### Texto alternativo
- Imagens que transmitam informação TÊM de ter uma etiqueta descritiva que sirva o mesmo propósito e apresente a mesma informação.
- Imagens que sejam ativas (hiperligações, botões) TÊM de ter uma etiqueta que descreva o o propósito ou função da imagem.</li>
- Imagens que sejam demasiado complexas para serem descritas num texto alternativo curto TÊM de ter o seu propósito descrito através de um texto altenativo extenso.</li>
- Imagens que não transmitam conteúdo, que sejam decorativa, ou com conteúdo já veiculado pelo texto NÃO PODEM ter um texto alternativo que seja exposto às tecnologias de apoio. Por exemplo em HTML corresponde a um alt="" (vazio).

#### Texto nas imagens
- Uma imagem NÃO PODE incluir texto informativo se se pode optar por texto real para a representar.
