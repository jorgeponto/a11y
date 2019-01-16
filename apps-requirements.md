
## Notas sobre plataformas iOS

### Tamanho do alvo de toque

Área alvo mínima:

- Recomendação Apple 44pt x 44pt
- Recomendação W3C 44px CSS x 44 px CSS (11,44mm = 1,144cm)

### Sobreposição de alvos
- Os alvos de toque não se devem sobrepor.

### Uma área compacta de alvos de toque
- alvos de toque precisam de ter uma folga entre eles

### Alvos de toque adjacentes para um mesmo destino
- precisam de ser agrupados

### Outros requisitos

- Os controlos de toque não devem ser ativados até que o utilizador retire o dedo ou outra parte do corpo, a caneta, etc. Os controlos nativos por defeito funcionam desta forma.
- Uma aplicação não pode apoiar-se somente nos movimentos cinéticos (detetados pelo acelerómetro).
- Uma aplicação não pode apoiar-se somente no controlo por voz.
- Uma aplicação não pode apoiar-se somente nos gestos.
- O utilizador deve ser capaz de desativar as funcionalidades sensíveis ao movimento.
- Teclados físicos em dispositivos móveis
- Sempre que possível, as ações devem ser mapeadas para os correspondentes gestos por defeito do iOS.
- Um botão deve sempre transmitir o seu papel usando um traço/perfil correto.
- O papel e o propósito de uma hiperligação têm de ser claramente transmitido pelo VoiceOver.
- As barras de progresso têm de transmitir o seu nome visível aos utilizadores do VoiceOver com uma legenda acessível descritiva e única.
- Os spinners (indicadores giratórios de atividade) de progresso têm de dizer o texto alternativo correto ou receber o focus imediatamente por forma a transmitir um nome acessível aos utilizadores do VoiceOver.
- Os controlos slider têm de ter uma legenda visível que seja programaticamente associada usando a propriedade acessível label (legenda).
- Os controlos Switch (interruptor) têm de ter uma legenda visível que esteja programaticamente associada usando a propriedade acessível label (legenda).
- O conteúdo dinamicamente gerado a seguir à interação de utilizador tem de satisfazer um dos seguintes requisitos: a tecnologia de apoio é automaticamente informada do novo conteúdo OU o novo conteúdo é a próxima coisa que a tecnologia de apoio irá encontrar na página.

