## Compra Rápida

Estes são os códigos para "bindar" (dar uma função a uma tecla) o teclado número para facilitar na compra de armas e equipamentos dentro de uma partida, o comando principal neste campo é o "bind" que define para alguma tecla outro comando que será automaticamente executado no console apertando a tecla.

Sintax do comando bind:

*bind [tecla] [comando]*


**Importante:**
Os valores **devem** estar entre aspas duplas para evitar possíveis conflitos.
Dentro do seu arquivo .cfg você poderá escrever comentários para por exemplo ajudar lembrar o que o comando faz mas para isso deve escrever "//" antes do comentário.

**Atenção:** os números citados são apenas do teclado numérico e funcionam independente do Num Lock está ativado ou não.

### Minha compra rápida

```
bind "kp_ins" "buy deagle;"
bind "kp_del" "buy tec9; buy fiveseven;"
bind "kp_enter" "buy decoy;"
bind "kp_end" "buy ak47; buy m4a1;"
bind "kp_downarrow" "buy ssg08;"
bind "kp_pgdn" "buy awp;"
bind "kp_leftarrow" "buy famas;"
bind "kp_5" "buy ump45;"
bind "kp_rightarrow" "buy sg556;"
bind "kp_home" "buy vesthelm;"
bind "kp_uparrow" "buy vest;"
bind "kp_pgup" "buy defuser;"
bind "kp_plus" "buy hegrenade;"
bind "kp_minus" "buy flashbang;"
bind "kp_multiply" "buy smokegrenade;"
bind "kp_slash" "buy molotov; buy incgrenade;"
bind "home" "buy ak47; buy m4a1; buy vesthelm; buy defuser; buy flashbang; buy smokegrenade;" 
```
### Visualização gráfica das compras
<br />
<p align="left">
    <img src="https://user-images.githubusercontent.com/54639269/77382583-8346d700-6d5f-11ea-8156-bf9609d9dc77.gif" alt="keybinds" width="400px">
</p>

## Teclado e Mouse

Esta é a seção da cfg para dar funções a cada tecla do teclado, maioria dessas binds já são a configuração padrão do csgo e não é necessário está na cfg a menos que antes de tudo tenha o comando "unbindall", que é o caso.

Irei comentar apenas as não padrões:

### BindToggle

Começando pelas binds toggle, são binds para alternar o valor de uma variável de 0 para 1 ou vice-versa.

Desliga/Liga a HUD deixando apenas as informações de morte no canto superior direito.

`bindToggle "h" "cl_draw_only_deathnotices"`

Alterna entre a visão da arma na mão esquerda ou direita.

`bindToggle "t" "cl_righthand"`

### Incrementvar

Incrementvar é um comando que pode incremetar uma variável.

Alterna o volume entre 0.15 e 0.30. Perfeito para situação de clutch.

`bind "c" "incrementvar  volume  0.15 0.45 0.15"`

Aumenta o tamanho do crosshair para cobrir toda tela, ajudando na hora de fazer granadas em pixels específicos.`

`bind "MOUSE4" "incrementvar cl_crosshairsize 1.5 4000 3997"`

### Jump Throw

Uma função muito importante para quem joga competitivo é ter uma tecla para fazer as famosas granadas usando jump throw (pular e jogar). Dentro do game pular e jogar uma granada faz ela ganhar muito mais velocidade no ar, mas na maioria das vezes é preciso pular em um tempo especifico por isso é importante ter uma tecla para essas granadas.

`bind "n" "+jump;-attack;-jump"`

### Outras binds úteis

utras binds úteis
Desconecta da partida **!!cuidado com essa bind!!**

`bind "p" "disconnect"`

Mais por diversão, está bind funciona para mandar mensagens para você (para mandar somente para o time o comando say será substituído por *say_team*).

`bind "j" "say nossa mermaum"`

### Minhas configurações de teclado e mouse

```
bind "0" "slot10"
bind "1" "slot1"
bind "2" "slot2"
bind "3" "slot3"
bind "4" "slot4"
bind "5" "slot5"
bind "6" "slot6"
bind "7" "slot7"
bind "8" "slot8"
bind "9" "slot9”
bind "a" "+moveleft"
bind "b" "buymenu"
bind "c" "incrementvar  volume  0.15 0.45 0.15"
bind "d" "+moveright"
bind "e" "+use"
bind "f" "+lookatweapon"
bind "g" "drop"
bindToggle "h" "cl_draw_only_deathnotices"
bind "j" "say nossa mermaum"
bind "k" "say puco"
bind "l" "say quem ta cego é corno"
bind "m" "teammenu"
bind "n" "+jump;-attack;-jump"
bind "p" "disconnect"
bind "q" "lastinv"
bind "r" "+reload"
bind "s" "+back"
bindToggle "t" "cl_righthand"
bind "u" "messagemode2"
bind "v" "holdpos"
bind "w" "+forward"
bind "y" "messagemode"
bind "z" "noclip"
bind "`" "toggleconsole"
bind "," "go"
bind "SPACE" "+jump"
bind "TAB" "+showscores"
bind "CapsLock" "+spray_menu"
bind "ESCAPE" "cancelselect"
bind "DEL" "mute"
bind "PAUSE" "pause"
bind "SHIFT" "+speed; r_cleardecals"
bind "CTRL" "+duck; r_cleardecals"
bind "F3" "autobuy"
bind "F4" "rebuy"
bind "F5" "jpeg"
bind "F6" "save quick"
bind "F7" "load quick"
bind "F10" "quit prompt"
bind "MOUSE1" "+attack"
bind "MOUSE2" "+attack2"
bind "MOUSE4" "incrementvar cl_crosshairsize 1.5 4000 3997"
bind "MOUSE5" "+voicerecord"
bind "MWHEELDOWN" "+jump" 
```

## Client

Essa seção fica bem pequeninha pois algumas opções do cliente estão distribuidas em outras seções.

### Cor
Definem sua cor dentro do jogo, as que aparecem no radar e placar.

`cl_color "1"`

***!esse comando não garante que sua cor será aplicada com 100% de sucesso dentro do jogo pois pode haver outro jogador que tenha escolhido a mesma cor e será sorteado pelo game!***

| Cor | Código
|-----|-------
|Amarelo | 0
|Roxo | 1
|Verde | 2
|Azul | 3
|Laranja | 4

### Evitando toxicidade
Como infelizmente é inevitável dentro comunidade de CS:GO existem muitas pessoas tóxicas e felizmente existe comandos para os inimigos dos outros times sempre estarem mutados. Isso pode evitar muitos estresses e te ajudar a jogar mais concentrado.

```
cl_mute_all_but_friends_and_party "1"
cl_mute_enemy_team "1"
```

### Texto de dano causado e recebido na tela
Muitos sabem que abrindo o Console é possível ver o dano causado e recebido dentro das partidas dos servidores oficiais:

<p align="left">
    <img src="https://steamuserimages-a.akamaihd.net/ugc/1013814107712751478/B2BBA3CB02DF89EB211474A3CC9C3AE16424689F/">
</p>

Porém poucos sabem que é possível ativar essa mensagem na tela por alguns segundos usando os comandos:
```
con_filter_text damage
con_filter_text_out Player:
con_filter_enable 2
developer 1
```
Aparecerá desta forma em cima do radar:

<p align="left">
    <img src="https://steamuserimages-a.akamaihd.net/ugc/1013814107712750684/B49005ADFFACC66C399A6F927D2CAD147D9683D8/">
</p>


### Minhas configurações de cliente
```
cl_color "1"
cl_mute_all_but_friends_and_party "1"
cl_mute_enemy_team "1"
cl_observercrosshair "1"
cl_playerspray_auto_apply "0"
sensitivity "2.2"
spec_show_xray "1"
con_filter_text damage
con_filter_text_out Player:
con_filter_enable 2
developer 1
```

