HTML Estrutura:

Temos uma estrutura básica HTML com uma div para conter o quiz, um parágrafo para exibir a pergunta, uma div para exibir as opções de resposta, um botão de envio e um div para exibir o resultado.
Estilo CSS:

Aplicamos um estilo mínimo usando CSS para melhorar a aparência do quiz.
JavaScript:

Começamos definindo um array chamado questions que contém objetos representando cada pergunta, suas opções e a resposta correta.

Em seguida, selecionamos os elementos HTML relevantes do DOM usando document.getElementById() e armazenamos em variáveis para facilitar o acesso posterior.

Inicializamos algumas variáveis como currentQuestionIndex (para controlar qual pergunta está sendo exibida) e score (para rastrear a pontuação do usuário).

Definimos a função showQuestion() que exibe a pergunta atual e suas opções de resposta. Para isso, iteramos sobre as opções de resposta de cada pergunta e criamos botões para cada uma delas. Adicionamos também um event listener para cada botão que chama a função checkAnswer() ao ser clicado.

A função checkAnswer() verifica se a opção selecionada pelo usuário corresponde à resposta correta. Se corresponder, incrementa a pontuação. Em seguida, avança para a próxima pergunta se houver, ou então exibe o resultado final.

A função showResult() esconde o contêiner do quiz e exibe a pontuação final do usuário.

Finalmente, chamamos a função showQuestion() para iniciar o quiz.
