# Logica-game-adivinha
Logica-de-programaçao2
Esse código é um pequeno jogo em JavaScript onde o usuário precisa tentar adivinhar três números gerados aleatoriamente, sem repetição, de 1 a 10.

Aqui está o passo a passo de como o código funciona:

Define a codificação de caracteres como UTF-8 para garantir que os caracteres especiais sejam exibidos corretamente.
Cria um campo de entrada <input/> e um botão <button> com o texto "Compare com o meu segredo".
Em seguida, há uma seção de script contendo algumas funções:
A função sorteia() gera um número inteiro aleatório entre 0 e 10 usando Math.random() e Math.round().
A função sorteiaNumeros(quantidade) gera um array chamado segredos que contém uma quantidade específica de números aleatórios, sem repetição. Ela usa um loop while para preencher o array com valores únicos gerados pela função sorteia().
No caso, a variável quantidade é definida como 3, portanto, a função sorteiaNumeros(3) retornará um array com três números aleatórios entre 1 e 10.
A variável segredos é inicializada chamando a função sorteiaNumeros(3), armazenando os três números aleatórios gerados.
O console exibirá o array segredos, que contém os três números gerados aleatoriamente.
O campo de entrada (input) é selecionado usando document.querySelector("input"), e o foco é dado a ele usando input.focus().
A função verifica() é definida para ser executada quando o botão for clicado. Essa função verifica se o valor inserido no campo de entrada corresponde a um dos números gerados anteriormente (segredos). Se corresponder, o usuário acertou, e uma mensagem de alerta é exibida. Caso contrário, o usuário errou, e outra mensagem de alerta é mostrada.
O evento onclick é atribuído ao botão para chamar a função verifica() quando o botão for clicado.
Portanto, ao executar o código em um navegador, o usuário será desafiado a inserir um número no campo de entrada e clicar no botão "Compare com o meu segredo". O código verificará se o número inserido corresponde a um dos três números gerados aleatoriamente. Se o usuário adivinhar corretamente, uma mensagem "Você ACERTOU!" será exibida; caso contrário, uma mensagem "Você ERROU!" será mostrada. Após cada tentativa, o campo de entrada será limpo, e o foco retornará para ele, permitindo que o usuário insira um novo valor para a próxima tentativa.
