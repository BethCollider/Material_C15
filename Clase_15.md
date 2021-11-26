# Bug y errores en el script 

### Codigo para cambiar imagen de trex runner a trex collider

Declarar variable de objeto con imagen

`var trex_collider;`

Cargar la imagen en function `preload(){}`

`trex_collider = loadImage ("trex_collided.png");`

Cargar la imagen en diseño del trex `function set up (){}`

`trex.addImage ("collid", trex_collider);`

Cambiar imagen en la condicional `GameState === END`

`trex.changeAnimation ("collid", trex_collider);`

### Codigo para deterner los grupos de objetos al estar en GS END

Codigo para deterner a los grupos de objetos al cambiar de `GS PLAY` a `GS END`

`sprite_Group.setLifetimeEach(-1);`

Detener a trex en `GS END`

`trex.velocityY = 0;`

### Codigo para incluir mensage de GameOver y restrar

Declarar variable con objetos de imagen de GameOver y restart

`var gameover, gameoverImg;`

`var restart, restartImg;`

Cargar imagen en `function preload (){}`

`gameoverImg = loadImage ("gameOver.png");`

`restartImg = loadImage ("restart.png");`

crear objeto que se animara con gameover y restart en `function set up() {}`

`gameover = createSprite();`

`restart = createSprite();`

Cargar imagen de gameover y restart 

`gameover.addImage(gameoverImg);`

`restart.addImage(restartImg);`

Cambiar escala de los objetos

`sprite.scale =  ;`

Definir objeto invicible en GS PLAY

`sprite.visible = false;`

Definir objeto visible en GS END

`sprite.visible = true;`









