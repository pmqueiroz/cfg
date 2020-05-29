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
<p align="center">
    <img src="https://user-images.githubusercontent.com/54639269/77382583-8346d700-6d5f-11ea-8156-bf9609d9dc77.gif" alt="keybinds" width="400px">
</p>
