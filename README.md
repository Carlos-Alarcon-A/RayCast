# Projeto-Raycast<br>
# Carlos Alarcon e Ruan Pablo<br>
Neste projeto fizemos um mini game para salvar o Luva de Pedreiro, destruindo as cataporas que nascem aleatoriamente lançando um Raycast nelas com o clique do mouse. Se o raycast atingir a catapora, ela é destruída e o placar a cima atualiza.<br>
# Como montamos<br>
![image](https://github.com/Carlos-Alarcon-A/RayCast/assets/128370700/d8574c3e-5d32-4408-85bf-a216684ec32d)
Adicionamos um cubo com material da foto do Luva de Pedreiro, outro cubo azul para ficar de fundo e criamos um prefab da esfera vermelha (catapora) para conseguirmos gerá-las aleatoriamente. Criamos um Raycast que será lançado no clique do botão esquerdo do mouse onde o ponteiro estiver apontando, e se o objeto atingido for a catapora, ela será destruída e será somado um ao placar a cima. E a cada clique do mouse ativa uma fala do Luva de Pedreiro. <br>
# Script<br>
![image](https://github.com/Carlos-Alarcon-A/RayCast/assets/128370700/610f5b51-e8ff-4135-9117-8f876e814047)
Este script em C# é um componente Unity que controla um sistema de raycasting para detectar e destruir Prefabs de "cataporas" quando clicados com o mouse. Ele começa definindo variáveis para o Prefab a ser instanciado, limites para a posição aleatória desse Prefab, uma array de áudios para tocar quando um objeto é clicado, um AudioSource para reproduzir os áudios, e variáveis para contar os cliques do mouse e o número de "cataporas" destruídas.<br>
No método Start(), ele inicia uma rotina que instancia o Prefab aleatoriamente e obtém o componente AudioSource associado ao GameObject. A rotina SpawnPrefab() instancia o Prefab em posições aleatórias dentro dos limites definidos, a cada segundo.<br>
No método Update(), ele verifica se o botão do mouse foi pressionado. Se sim, cria um raio a partir da posição do mouse na tela em direção ao mundo 3D. Se esse raio atingir um objeto, o script verifica se esse objeto tem a tag "alvo". Se tiver, o objeto é destruído, o contador de "cataporas" destruídas é incrementado e o texto é atualizado para mostrar o número de "cataporas" destruídas.<br>
# Vídeo GamePlay (ative o som!)<br>


https://github.com/Carlos-Alarcon-A/RayCast/assets/128370700/95187d65-3217-4e0f-8fa0-0f1d1af031d0


