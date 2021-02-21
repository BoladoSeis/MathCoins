BATALHA CRIPTOANALÍTICA NA ERA DIGITAL
Seis Bolado
seisbolado@gmail.com

Resumo

A tecnologia computacional clássica nos trouxe a o que somos hoje criptograficamente falando, mas ela mesma pode nos tirar a privacidade (ou dar informações secretas) por meio de um novo tipo de moeda, ou até mesmo a computação quântica e seus fótons. Este artigo foi produzido com o fruto de pesquisas, portanto apesar de ser o que considero mais verdadeiro no momento, não posso afirmar que está completo de razão. 

Palavras-chave: Criptografia, Criptomoeda, Era Digital, Computação

Introdução

Desde o início dos tempos, levar informação não foi uma tarefa fácil. Hoje em dia, como a tecnologia RSA está mais fácil ainda, mas não é garantia que será assim amanhã. Muitas tecnologias estão sendo desenvolvidas para acirrar esta batalha, e garantir (ou não) a sua segurança e privacidade.

Breve histórico

A criptografia é a ciência de ocultar uma mensagem, enquanto a criptoanálise é a ciência de obter a mensagem a partir do código criptografado. Ambas são ciências complementares, de forma que o desenvolvimento de uma tende a acontecer apenas pela evolução da outra. 
    Ao longo da história humana várias cifras foram fortemente usadas por não terem sido amplamente criptoanalisadas na época, como a cifra de César e as cifras monoalfabéticas, que foram quebradas pelo método de análise de frequência. No século XV a cifra de Vigenère foi altamente utilizada, até que no século XIX Charles Babbage com seu proto computador (uma máquina de adição e subtração) desvendou esta cifra. Na Segunda Grande Guerra os alemães desenvolveram o enigma, uma máquina eletromecânica que revestia um novo algoritmo encriptador, até que Alan Turing, com um dos primeiros computadores conseguiu ler as mensagens germânicas.
  A velocidade entre a criação de um algoritmo e sua criptoanálise vem diminuindo em proporção ao desenvolvimento da matemática e de máquinas de calcular. Atualmente as cifras proeminentes são baseadas em um algoritmo protocolado por um trio há 43 anos.[1],[2]

RSA

A criptografia RSA é um método de criptografia na qual se utiliza uma chave privada (p,q,d) para a reversão da criptografia, e uma chave pública (e,n) para a codificação. Este método com duas chaves se chama criptografia assimétrica, pois o método de cifragem é assimétrico ao método de decifragem.
    Os números p e q são dois números primos, que para um nível aceitável de segurança hoje, devem ter ao menos 100 dígitos. O produto de "p" e "q" é "n". Para "e", temos um valor menor que φ(n) é coprimo a "n", sendo φ a função totiente de Euler. Por fim, "d" é o inverso multiplicativo de "e" em (mod φ(n)).
   O objetivo de um criptoanalista de RSA é descobrir a dupla (p,q) a partir de n, pois com isso a tripla (p,q,d) é revelada. Para aumentar a segurança da RSA, um criptógrafo deve tomar ciência sobre primos colossais. 
    Para aumentar a potência de um algoritmo decodificador, um desvendador de cifras deve tomar ciência da função Sigma (soma dos divisores), que por sua vez tem como maior dificuldade computacional descobrir os quocientes entre um número e seus coprimos, esta descoberta que chamarei de método A.
        O método A nos ajuda a calcular as somas de Ramanujan, a função de Möbius, e a função totiente de Euler.
    Para saber com alguma precisão os valores de (p,q), necessitamos saber os valores do método A até  no mínimo n, porque como o método soma dos divisores é calculado como a soma infinita das somas de Ramanujan (cx(n)) no monômio( π²/6*n*cx(n)/x²), basta saber as somas de Ramanujan até o valor de c√n(n), pois então o monômio ficaria (π²/6*c√n(n)), o que tende a ser desprezível para n grande. 
     Para formar um banco de dados sólido e verificável, um codificador deve testar a primalidade de cada número e guardar os valores essenciais, método este chamado método B.[1],[3],[4]

Segurança da informação na era digital

Analisando durante as décadas desde a primeira implementação, várias tentativas de ataques foram feitas e, a respeito das que atacaram a criptografia em si (não o protocolo e a engenharia social), os ataques, estudados pelo artigo Twenty Years of Attacks on the RSA Cryptosystem, foram efetuados baseados numa má implementação do protocolo, onde número (p,n) não suficientemente grandes são escolhidos, e, nenhum ataque foi bem sucedido contra uma boa implementação. Isso nos indica que a hipótese "um ataque de força bruta é uma boa solução" está no caminho correto.
    O maior problema deste tipo de ataque, e de uma procura por primos à força bruta, é o tempo computacional para executá-los, que costuma ser enorme. 
  O tempo computacional para calcular o método A recursivamente para todos os números abaixo de n é: O(n(log n)²log( log(n))[13]
    E para o método B para um intervalo entre x e y é: O ( k · log 3 n ), onde k é a acurácia que queremos, determinada pelo minerador.[4]
  Nem sempre se soube valores primos tão grandes como os atuais, e atualmente não se têm ciência de números primos que ainda estamos a conhecer. A segurança da RSA está evoluindo, e a potência dos métodos de decifragem, especialmente do método A, também. Com isso, é perceptível que, com um certo delay, pode se criptoanalisar um código antigo. Inclusive, com o aumento da potência computacional que vem se desenrolando nesta última metade de século, o tempo de ininteligibilidade do código tende a cair, o que pode levar a uma exposição de informação ainda em tempo com valor de mercado. 
    Inclusive, este avanço computacional pode ser aumentado pelo desenvolvimento de computadores quânticos, que já são uma realidade hoje em dia, apesar de suas limitações práticas. O potencial quântico de força bruta é incrível, e pode tornar estes algoritmos ainda mais viáveis, considerando os fundamentos da física quântica.[5]

Futuro Quântico

O fim da segunda década do novo milênio foi recheada de declarações a respeito da computação quântica, em principal, recheado de anúncios de supremacia quântica atingida, que foi primeiramente declarada pelo Google, em 23/10/2019, e pela China em 3/12/2020. O grande diferencial da computação quântica é forma do processamento que o hardware utiliza, que são qbit, bits probabilísticos, e que portanto abrem possibilidade para, quando usados em série, ter potência exponencial: a cada novo qbit adicionado a série, o processamento dobra de potência.
   Por ter esta característica fundamental de exponenciação, algoritmos de força bruta são um bom alvo para estes computadores, pois tem tempo polinomial exponencial.
   Explorando a física quântica, pela visão de um criptógrafo, pode-se aproveitar a polarização do fóton para transmitir informações entre um emissor e um receptor, e detectar se houve uma escuta na linha. Com isso, pode-se criar uma transmissão criptografada inviolável. (The Code Book, chapter 7)
    No entanto, a tecnologia quântica é muito sensível e ainda se sabe muito pouco a respeito, de forma que dificuldades como superaquecimento, interferências eletrônicas e espetáculos inesperados atrapalham a implementação prática hoje em dia.[8],[9]

MathCoins: Especulações na batalha

No limbo entre o desenvolvimento da RSA e a aplicação prática da tecnologia quântica, estamos com uma vitória dos criptógrafos. Desde o início da história criptográfica, tanto a criptografia quanto a criptoanálise desempenharam papéis econômicos importantes, com incentivos para seus trabalhos, mas vindos massivamente de investimentos coercitivos, de forma que o desenvolvimento das tecnologias pode, ou não, ter tido uma oferta reduzida artificialmente. Com o enriquecimento da população, investimentos em privacidade (e criptoanálise) pessoal aumentaram, fato demonstrado pelo uso da internet criptografada para transmissão e pesquisa deste artigo. 
    Portanto, parece haver uma demanda por um meio de investir em tecnologia de criptografia, e é isto que as MathCoins DecryptoCoin e CryptoCoin buscam suprir, de acordo com seu White Paper. Segundo o mesmo, com as mesmas taxas de incentivos aos mineradores que o Bitcoin, utilizando a tecnologia do blockchain do livro APRENDA BLOCKCHAIN ESCREVENDO UMA, as criptomoedas tem seus códigos fonte em um repositório git e se baseiam em manter uma moeda digital, livre de fraudes, e que mantém seus mineiros trabalhando respectivamente em soluções para os métodos A e B.
    A segurança das criptomoedas são baseadas em criptografias assimétricas, de forma que aparentemente a tecnologia é um risco para si mesma. No entanto, os usuários podem usar as chaves privadas que quiserem, e então à medida que a potência criptoanalista aumenta, a segurança pessoal pode também. Estas criptomoedas também podem ser o berçário para a utilização de um computador quântico para a quebra da RSA, pois pode ser inclusa a máquina em uma "pool", o que geraria resultados mesmo sem a eficiência máxima necessária para o uso solo. Isto também faz dos computadores quânticos um investimento mais lucrativo, já que agora eles podem minerar ativos, e assim se precifica a tecnologia.
    Com a possibilidade de especulação sobre o meio criptográfico da RSA, haverá a precificação da informação, protegida e descriptografada, pelo mercado, além de uma tendência de apoio governamental à DecryptoCoin. O criador, que responde pelo nome da organização Seis Bolado, quando perguntado sobre quem, em sua opinião, é o público alvo das moedas, afirma que:" A população em geral tem mais a ganhar investindo na DecryptoCoin, pois estes não tem nada a perder como informações altamente confidenciais. Já grandes empresas, ou principalmente estados, têm segredos de estado, e principalmente a ideia de propriedade intelectual a proteger. Com a quebra da RSA, monopólios seriam quebrados, e a população poderia se libertar do estado." Ele afirma também, quando perguntado a respeito da propriedade intelectual, que:" Propriedade existe apenas para alocar recursos escassos. Ideias, pensamentos, códigos, artigos e imagens não são escassos, não podem ter um dono". Com isto ele acredita que o trabalho dos criptoanalistas é legítimo, porque não está interferindo na propriedade de outrem.
     As principais características técnicas destas criptomoedas são: 21 milhões de unidades; halving (distância temporal na qual os mineiros ganham apenas metade da recompensa) de 4 em 4 anos; livre mineração (qualquer um pode oferecer sua capacidade computacional para ganhar algumas moedas de recompensa); blockchain público (o livro-razão da moeda, que é escrito de forma imutável, que contém os resultados das operações matemáticas (algoritmo A e B) é acessível a todos); Não existe órgão regulador, ou dono do sistema.
    As MathCoins, grupo de criptomoedas da CryptoCoin, são um tipo de moeda que efetuam operações matemáticas. Elas podem ser muito úteis para solução de problemas de alto nível computacional.[10],[11],[12]

Conclusão

A batalha criptoanalista na era digital vem se desenrolando na forma de um ativo no mercado, sujeito a incentivos positivos e negativos, e vem usando tecnologias de ponta com resultados que são surpreendentes, tanto do lado criptográfico, quanto do lado criptoanalítico, e, considerando um futuro próximo, os criptógrafos e criptoanalistas tem uma batalha que envolve o todo o mercado global, e num futuro distante, tende-se que os criptógrafos efetuem um método de troca de informações segura com a tecnologia quântica.
