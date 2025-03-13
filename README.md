# Ebac Platformer Task

Jogo feito no cursos Ebac, nesse curso eu aprendi a desenvolver game utilizando Unity 3D.

# Menu

O Menu do jogo terá três opções: um play para entrar cena gameplay e outro exit para sair do jogo e credits.
Utilizamos o HorizontalLayoutGroup para organizar os botões.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Menu.gif" width="530" height="450"/></td>
      <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Grid_HorizontalLayoutGroup.png" width="430" height="500"/></td>
    </tr>
</table>

# Managers

O gameManager vai gerenciar aspectos do jogo como prefab do player e inimigos, referências e animação.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_GameManager.png" width="430" height="300"/></td>

<table border="0">
   <tr>
        <td>O ItemManager vai gerenciar moedas do jogo. <img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ItemManager.png" width="460" height="100"/></td>
        <td>O UIinGameManager vai gerenciar Interface Gráficas do jogador. <img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_UIinGameManager.png" width="460" height="100"/></td>
    </tr>
</table>

O PauseManager vai gerenciar sistema pause do jogo.

<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_PauseManager.png" width="500" height="100"/>

# Player 

O personagem poderá movimentar para todos os lados e pular no cenário, o script HealthBase vai fazer a parte vida do player e todos inimigo do jogo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Movimentação.gif" width="530" height="450"/></td>
        <td>Scripts: Player and HealthBase<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Player_HealthBase.png" width="430" height="500"/></td>
    </tr>
</table>

O Sorting Group vai cuidar ordena renderização dos renderers do cenário, quando o player levar um hit me bisca quem vai fazer ele piscar e o script FlashColor.
Quando o personagem morre ele vai ser destruído o script PlayerDestroyHelper que vai fazer isso acontecer.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_sortingGroup_FlashColor_PlayerDestroyHelper.png" width="430" height="450"/></td>
 
# Animação

O animador do player com as animações e as transições e os parâmetros run que é um Trigger, o death e um Bool.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Animation_Player.png" width="1160" height="364"/></td>

O animator do player
<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_animator.png" width="489" height="191"/></td>

# skinning


# Itens e inimigos


# scriptable objects


# VFX


# Adicionando Som
