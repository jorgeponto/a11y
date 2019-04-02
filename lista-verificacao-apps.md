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

<ul>
  <li>Dynamically generated content following user interaction MUST meet one of the following: assistive technology is automatically made aware of the new content OR the new content is the very next thing the assistive technology will encounter on the page.</li>
</ul>

#### Limites de tempo
<ul>
  <li>If there is a session time limit, users MUST be warned before the session ends and MUST be given time to save their data and/or extend the session.</li>
  <li>Incomplete data SHOULD be saved after a session timeout.</li>
</ul>

#### Alertas
<ul>
  <li>Alerts MUST include a title and description.</li>
</ul>

#### Caixas de diálogo

<ul>
  <li>Custom Dialogs MUST set <code>accessibilityViewIsModal</code> to "true" and the focus MUST be sent to the dialog.</li>
</ul>

### Elementos personalizáveis

#### Acordeons

<ul>
  <li>Accordion components MUST announce their accessible name and their expanded or collapsed state.</li>
</ul>

#### Auto-preenchimento
<ul>
  <li>VoiceOver users MUST be automatically made aware of the autocomplete suggestions when they appear.</li>
</ul>

#### Controlo de pontuação
<ul>
  <li>A rating control MUST always convey its current value, any visible information, and be operable by both VoiceOver and non-VoiceOver users.</li>
</ul>

#### Tabela ordenável
<ul>
  <li>If a table is sortable, the header cells' accessibility labels MUST dynamically update to correctly convey their sorted state each time the data order changes.</li>
</ul>

#### Interruptor ligado/desligado
<ul>
  <li>Toggle buttons MUST convey an accessible name with programmatically associated, visible labels and convey their state using the accessibility label.</li>
  <li>Image toggle buttons MUST have descriptive, accurate alternative text provided in the accessibility label.</li>
</ul>

### Validação e etiquetagem de formulários

#### Etiquetagem

<ul>
  <li>The label MUST be visible at all times.</li>
  <li>Labels MUST be programmatically associated with their corresponding control elements.</li>
  <li>A "hint" SHOULD be provided when the label doesn't sufficiently convey a control's purpose to VoiceOver users.</li>
</ul>

#### Agrupar etiquetagem
<ul>
  <li>For groups of related controls where the individual labels for each control do not provide a sufficient description, additional group labels MUST be provided.</li>
</ul>

#### Caixas de verificação
<ul>
  <li>Checkboxes MUST convey their selected or checked state to VoiceOver.</li>
  <li>Groups of checkboxes MUST provide a common group label as well as a unique label for each control via their accessibility label properties.</li>
</ul>

#### Campos de edição para recolha de dados do tipo datas
<ul>
  <li>A standard Date Picker control SHOULD be used instead of a text field in order to avoid forcing users to enter a date with a default keyboard.</li>
</ul>

#### Botões do tipo Rádio
<ul>
  <li>Radio buttons MUST provide a common group label as well as a unique label for each control via their accessibility labels and they MUST convey their selected state.</li>
</ul>

#### Select (UIPickerView) ??
<ul>
  <li>Controls using UIPickerView MUST be programmatically associated with their visible label in order to provide an accessible name.</li>
</ul>

#### Campos de edição do tipo texto
<ul>
  <li>Text fields MUST have programmatically associated, visible labels.</li>
</ul>

#### Validação e reporte de erros</h4>
<ul>
  <li>Efficient, intuitive, and clearly identified text based alerts MUST be provided to users for form validation cues and errors.</li>
  <li>If input errors are automatically detected, suggestions MUST be provided in text for fixing the input in a timely and accessible manner before the data is submitted to the server.</li>
</ul>

### Navegação

#### Títulos da página

<ul>
    <li>Screens MUST have meaningful titles.</li>
</ul>

#### Separadores e respetivos painéis
<ul>
    <li>Tabs MUST convey their role, their current state, and their order in the total number of tabs to VoiceOver users.</li>
</ul>

#### Menu
<ul>
    <li>Menu items MUST have the appropriate trait in order to convey their accessible role.</li>
    <li>The button that opens the menu MUST have a clear, descriptive title or accessibility label to accurately convey its purpose.</li>
    <li>VoiceOver users MUST be able to dismiss the menu.</li>
    <li>When the menu is closed, focus MUST return to the triggering button.</li>
  </ul>

### Orientação do Dispositivo
<ul>
  <li>The orientation of the content MUST not be locked to either landscape or portrait unless a specific orientation is essential for the functionality of the app.</li>
</ul>

### Estrutura semântica e significante

####Cabeçalhos
<ul>
    <li>Headings used to title or describe sections of content MUST use the header trait in order to convey their semantic purpose.</li>
</ul>

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
