# Ebac Platformer Task

Jogo feito no cursos Ebac, nesse curso eu aprendi a desenvolver game utilizando Unity 2D.

# Menu

O Menu do jogo terá três opções: um play para entrar cena gameplay e outro exit para sair do jogo e credits.
Utilizamos o HorizontalLayoutGroup para organizar os botões.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Menu.gif" width="530" height="450"/></td>
      <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Grid_HorizontalLayoutGroup.png" width="495" height="371"/></td>
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

<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_PauseManager.png" width="491" height="49"/>

# Player 

O personagem poderá movimentar para todos os lados e pular no cenário, o script HealthBase vai fazer a parte vida do player e todos inimigo do jogo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Movimentação.gif" width="530" height="450"/></td>
        <td>Scripts: Player and HealthBase<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Player_HealthBase.png" width="430" height="500"/></td>
    </tr>
</table>

O ataque que o player pode fazer é tirar bola do inimigo e ele pode atirar para todos os lados e atira no pulo e o tiro atinge o inimigo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Attack_Cannon.gif" width="530" height="450"/></td>
        <td>Scripts: GunBase<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_script_GunBase.png" width="497" height="171"/></td>
    </tr>
</table>

O Sorting Group vai cuidar ordena renderização dos renderers do cenário, quando o player levar um hit me bisca quem vai fazer ele piscar e o script FlashColor.
Quando o personagem morre ele vai ser destruído o script PlayerDestroyHelper que vai fazer isso acontecer.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_sortingGroup_FlashColor_PlayerDestroyHelper.png" width="430" height="450"/></td>
 
# Animação Player

O animador do player com as animações e as transições e os parâmetros run que é um Trigger, o death e um Bool.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Animation_Player.png" width="1160" height="364"/></td>

O animator do player
<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_animator.png" width="489" height="191"/></td>

# Animação Enemy

O animador do enemy com as animações e as transições e os parâmetros attack que é um Trigger, o death e um Trigger.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Animation_Enemy.png" width="1160" height="364"/></td>

O animator do enemy
<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Animator_Enemy.png" width="489" height="191"/></td>

# skinning

No Skinning Editor pode criar ossos no sprite para poder manipular o sprite e fazer animações.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_SkinningEditorCreateBone.png" width="1153" height="594"/></td>

O Skinning Editor tem um funções para gerar automaticamente geometria para animar objeto 2d, e animação vai seguir essa formatação dessa geometria.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_SkinningEditor.png" width="1153" height="594"/></td>

O objeto precisa do sprite Skin para funcionar os ossos do objeto.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_SpriteSkin_Satellite.png" width="495" height="371"/></td>

Aqui como ficou personagem e objetos da cena como skinning.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/record_player_bone.gif" width="320" height="210"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/record_enemy_bone.gif" width="320" height="210"/></td>
    </tr>
</table>

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/record_Satellite_bone.gif" width="320" height="210"/></td>

# Itens e inimigos

O item que o jogo vai ter moedas que o player poderá pegar é cada um que o jogador pegar vai adicionar um valor na interface do game.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Coins.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_CircleCollider2d_ItemCollectable.png" width="495" height="371"/></td>
    </tr>
</table>

O inimigo vai poder ser atingido pelos tiros do player e morrer se ele perder toda sua vida, e o inimigo dá uma piscada quando for atingido por causa do script FlashColor.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Enemy.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_EnemyBase_HealthBase_FlashColor.png" width="495" height="371"/></td>
    </tr>
</table>

# scriptable objects

O scriptable objects e o script de configurações dos valores que os scripts vão utilizar, assim os animadores e artistas poderão modificar os valores do script.

<td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_SO_Player_01.png" width="455" height="352"/></td>

# VFX

O VFX da moeda quando jogador pega moedas vai aparecer particle system que vai criar várias moedas por uns segundos.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Coins.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_coins_Emisson.png" width="499" height="596"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_coins_Shape_SizeOverLifetime.png" width="495" height="470"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_coins_Collision.png" width="492" height="303"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_coins_Renderer.png" width="494" height="388"/></td>
    </tr>
</table>

O vfx do pulo do player quando o jogador pular vai aparecer particle system no chão onde jogador pulou.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Movimentação.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_jump_Emisson.png" width="499" height="596"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_jump_Shape_ColorOverLifetime.png" width="495" height="470"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_jump_Collision.png" width="492" height="303"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_jump_Renderer.png" width="494" height="388"/></td>
    </tr>
</table>

Quando o personagem correr vai aparecer uma fumaça nos pés do player o particle system ficar no pé do personagem.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Movimentação.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_walk_Emisson.png" width="499" height="596"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_walk_Shape_ColorOverLifetime.png" width="495" height="470"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_walk_Size-over-Lifetime_Collision.png" width="492" height="303"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_walk_Renderer.png" width="494" height="388"/></td>
    </tr>
</table>

Os vagalumes vão perseguir o player no cenário e o particle system ficar dentro do personagem.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_Movimentação.gif" width="530" height="450"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_firefly_Emisson.png" width="499" height="596"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_firefly_Shape_ColorOverLifetime.png" width="495" height="470"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_firefly_Size-over-Lifetime_Noise.png" width="492" height="303"/></td>
    </tr>
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_firefly_Collision.png" width="494" height="388"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_ParticleSystem_coins_Renderer.png" width="494" height="388"/></td>
    </tr>
</table>

# Som do game

<h4>Som Coins</h4>

O script ItemCollectableCoin que vai estar selecionado Audio Source que vai tocar áudio quando o player pegar moeda e imagem do AudioSource e suas configurações.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioSource_Coins.png" width="495" height="470"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_script_ItemCollectableCoin.png" width="495" height="199"/></td>
    </tr>
</table>

<h4>Audio Player</h4>

O audioPlayHelper serve para testar áudio do player, já o audioRandomPlayAudioClips vai play vários áudio para não ficar tocando os mesmos áudios.
Criamos 3 AudioSource para pode tocar um 1 por vez, vai tem 3 AudioSource um primeiro que vai mudar os áudios dos passo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioPlayHelper.png" width="495" height="480"/></td>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioRandomPlayAudioClips.png" width="495" height="430"/></td>
    </tr>
</table>

Aqui animation selecionada com animação ANIM_Astronaut_Run.

<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_animation_Run_PlayRandom.png" width="1100" height="360"/>

Aqui o mesmo script que faz tocar vários áudio para não ficar tocando o mesmo áudio quando o player ficar atirando.

<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_Shoot_AudioRandomPlayAudioClips.png" width="495" height="253"/>

<h4>Audio Pause</h4>

O menu pause tem as configurações áudios sfx que vão controlar volume de áudios dos efeitos no jogo como tiros e moedas no game, 
e também poder controlar o volume de áudios música do jogo. A transição vai mudar a configuração dos áudios no mixer.

Para modificar volume do jogo tem um slider que jogador pode puxar para direita e esquerda assim o volume poderá ser aumentado ou diminuindo.

O script AudioTransition que vai esta no botao Transition.

O script AudioChangeVolume estará no SliderSFX e SliderAmbience ele foi add nos dois slides que vai dizer qual volume ele vai manipular
e variavel do script Float Param que foi criada no audio mixer: audio source que está no audio mixer clicando audio source e na janela inspector e clicando volume em expose.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/Recordings/Movie_MenuPause%20Audios.gif" width="530" height="450"/></td>
        <td>
            <img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioTransition.png" width="495" height="90"/>
            <img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioChangeVolume.png" width="495" height="90"/>
            <img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioTriggerTransition.png" width="500" height="111"/>
        </td>
    </tr>
</table>

<h4>Audio Mixer</h4>

O Audio Mixer onde ficam todas configurações áudio source e snapshots que são configurações do botões transições e grupos onde ficam todas áudio source e 
exposed parameters onde está a variáveis que sliders vão utilizar para poder modificar volume.

<img src="https://github.com/guiardev/Ebac-platformer-exercicio/blob/develog/Assets/imgs/img_AudioMixer.png" width="1155" height="365"/>
