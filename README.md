# moveit
### Aplicação criada durante o evento #NLW04 (Next Level Week) da <a href="https://app.rocketseat.com.br/">Rocketseat</a>

 &nbsp;&nbsp;&nbsp;&nbsp;App de aplicação da <a href="https://pt.wikipedia.org/wiki/T%C3%A9cnica_pomodoro" target="_blank">Técnica de Pomodoro</a> para estudantes das mais diversas áreas que possuem dificuldade para reservar um tempo entre os estudos para se alimentar e até mesmo práticar algum exercício físico. Sua aplicação consiste em reservar 25min para estudo e 5min relaxamento/hidratação, neste caso é gerado um desafio que provoca o usuário a prática de exercicios fisicos, tudo isso com um contexto de gameficação.<br>
&nbsp;&nbsp;&nbsp;&nbsp;O método baseia-se na ideia de que pausas frequentes podem aumentar a agilidade mental.

### Conhecimento adquiridos
1. ##### Utilização do NextJS
    Motivo do surgimento e evolução do framework. Conceitos de Single Page Aplication (SPA), Server Side Rendering (SSR) e Static Site Generation (SSG) e pensar ao escolher entre o uso do ReactJS ou NextJS, estes foram alguns do ensimanetos introdutórios.
2. ##### Componentização
    Tudo é componente! Definitivamente esta frase define a ideia da ferramenta, neste momento passamos a planejar nosso projeto como pequenas peças que podem ser montadas individualmente, mas que se comunicam para formar um todo. Uma de suas principais vantagens é a reutilização de código, uma vez que um componente criado pode ser instanciado novamente sem que seja escrita uma linha de código a mais.
3. ##### Hooks (Ganchos)
    O Hook é uma feature introduzida no react que permite fazer uso de <i>estado</i> em funções que são componentes. Neste projeto utilizamos 3 hooks, são eles:
    1. ###### UseState      
        É uma forma de atualizar o estado de um componente, permitindo que apenas os campos que forem afetados pela mutação deste componente sejam atualizados, além de gerar um código limpo, gera efeciencia na renderização do componente, uma vez que ele apenas "recarrega" o que foi alterado e não toda sua interface.
    2. ###### UseEffect
        Como o próprio nome diz, ele gera efeitos colaterais, vamos lá! Dentre suas utilizades, podemos usá-lo para efetuar determinada ação caso algo aconteça em nossa aplicação, seja a mutação de um useState ou a ação de um, gerando assim o chamado efeito colateral.
    3. ###### UseContext
        Permite compartilhamento de informações entre os componentes, independente do grau de parentesco entre os mesmo, sempre que uma variável assinada pelo useContext é alterada, os componentes que consomem este valor são renderizados novamente.

### Processo de desenvolvimento
1. ##### ExperienceBar
    Basicamente criamos um ```<header>``` com um ```<span>``` que se move de acordo com o valor de um hook de estado, este hook mede a quantidade de XP do usuário, sempre que avançade a barra de experience enche.
2. ##### Countdown
    Criamos um contador que usa a função ```setTimeOut()``` do javascript para gerar o decréscimo no tempo, este contador ficou ao lado esquerdo da view sobre o botão de iniciar contagem, sempre que a contagem do tempo de estudo chegava ao fim, era disparo um evento via useEffect e este por sua vez encadeava a função de gerar um challenge.
3. ##### ChallengeBox
    A caixa de desafios era responsável por receber o disparo do ```useEffect``` e gerar uma dinâmica aleatória, o usuário tem 5min para executar e clicar no botão de finalizado ou cancelado, em caso de resposta positiva, é gerado um modal parabenizando o estudante, os pontos referente ao desafio são somados à barra de experiencia do usuário e o contador retorna à 0.
4. ##### Profile
    Este componente é responsável por exibir a imagem do usuário, coletada da api do <a href="https://github.com/"> Github</a>, informar a quantidade de desafios já responsidios pelo usuário e seu nível de experiência.
5. ##### Cosiderações finais
    Foram implementados outros componentes adicionais, como: CompletedChallenges, LevelUpModal, sem falar no uso do useContext, que em minha opinião foi a cereja do bolo.
<br>

#### Se ficou interessado no projeto, tem interesse em alguma feature ou quer simplesmente trocar uma ideia, segue <a href="https://github.com/Gleydson07/moveit">link</a> do repositório e logo abaixo as redes sociais onde estou presente.

### Contato
[ <img src="https://lh3.googleusercontent.com/EViPU9FCAUhSgZR7hnFJRlSL4gkhL_ye0n4VldsEZA_yUlslnHk-3BgQKXnArQzb14OO" height="25px"/>](https://app.rocketseat.com.br/me/gleydson-albuquerque-07782) :link:  &nbsp; &nbsp;&nbsp;  [ <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/LinkedIn_Logo.svg/1280px-LinkedIn_Logo.svg.png" height="25px"/>](https://www.linkedin.com/in/gleydson07/) :link:  &nbsp; &nbsp;&nbsp; &nbsp;&nbsp; :email: gassantos.dev@gmail.com :email: 
 <br>
### Resultado obtido

[ <img src="2.png" style="height:400px"/>](https://move-dev-btf95uopw-gleydson07.vercel.app/)
