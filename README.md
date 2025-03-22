# Livro: Sistemas Operacionais Modernos 4° edição, de ANDREW.S e HERBERT. 
<span style="color:cyan">
Resumo Cap.1: Introdução
</span>





**1.1** O que é um sistema operacional?

Um sistema operacional é difícil de definir, pois ele opera diretamente em uma máquina (hardware) com o intuito de facilitar a vida do usuário/programador. Operar diretamente através do hardware é uma tarefa extremamente complexa, pois ele é complicado, pouco intuitivo e sensível. Para solucionar esse problema, foram criados os sistemas operacionais, que facilitam o uso e o gerenciamento da máquina.

Imagine o Windows, que, caso não conheça, é um dos sistemas operacionais mais utilizados. Assim que instalado, ele tem acesso total ao hardware da máquina, como o disco rígido, que é um componente muito complexo para se manipular diretamente. O sistema operacional permite que, por meio de uma interface gráfica (no caso do Windows, a shell), você possa gerenciá-lo facilmente. Um bom exemplo disso são as pastas que criamos para organizar arquivos.

Em resumo, um sistema operacional abstrai tudo o que é complexo e pouco intuitivo no hardware, tornando-o acessível e fácil de usar para o usuário.

#

**1.3** Revisão sobre hardwares de computadores

Um sistema operacional está sempre diretamente ligado a um hardware, como os processadores ou CPU, que é o cérebro do computador. É ele que comanda e controla tudo o que ocorre entre os hardwares, como a memória, o teclado, o mouse, o monitor, entre outros. A CPU é sobrecarregada de tarefas assim que é ligada junto com a máquina e só "descansa" quando tudo é desligado. O processador armazena muitas variáveis e resultados temporários através de registradores gerais.

Além dos registradores gerais, existem os registradores especiais, que ajudam o processador a se organizar e a garantir que nenhum processo seja perdido ou esquecido. Um exemplo interessante são os processos de E/S (Entrada e Saída). Quando iniciados, eles interrompem vários outros processos e, para que o processador não se perca, existe um registrador especial chamado PSW (Program Status Word), que guarda o estado do processador, permitindo que, após o processo de E/S, ele retome a tarefa anterior. 

Junto aos processadores, há as memórias, que são partes essenciais para o funcionamento do processador. As memórias têm hierarquia, sendo as mais rápidas as primeiras, como os registradores da CPU. O cache, que também é muito rápido, fica próximo à CPU com o propósito de agilizar alguns processos e armazenar informações como caminhos de pastas, palavras, conteúdos em URLs, entre outros. Todas essas informações armazenadas no cache geralmente são dados muito repetidos.

A memória RAM (Random Access Memory) ocupa a próxima posição na hierarquia e é conhecida como memória principal. Ela possui capacidade de vários gigabytes e serve para armazenar todos os processos que a CPU não consegue guardar diretamente.


No último nível da hierarquia estão os discos magnéticos, conhecidos como HDs (discos rígidos), e os SSDs (discos de estado sólido). Apesar do nome, os SSDs não utilizam discos físicos. O espaço de armazenamento dos HDs é mais barato em comparação ao espaço das CPUs ou RAMs, porém sua velocidade é muito menor. Ainda assim, podem alcançar vários terabytes de capacidade. Os HDs utilizam um ou mais discos internos que, quando o dispositivo está ligado, permanecem em movimento. Assim como um disco de vinil, há um cabeçote que se desloca sobre os discos para armazenar e acessar informações quando requisitado.

Ao ligar um PC, a BIOS (Sistema Básico de Entrada e Saída) é inicializada logo em seguida. A BIOS é um sistema que normalmente vem integrado à placa-mãe (componente que conecta todos os dispositivos do computador). Ela realiza um check-up da memória RAM e de todos os dispositivos conectados ao PC. Além disso, possui uma pequena quantidade de armazenamento para registrar dispositivos conhecidos. Após verificar se está tudo em ordem, a BIOS inicia o processo de boot do sistema operacional. Se o sistema já estiver instalado, ele será carregado a partir do HD ou SSD. Caso contrário, será necessário conectar um CD ou pendrive USB contendo o instalador do sistema operacional para realizar a instalação.

#

**1.4** O zoológico dos sistemas operacionais

Existem inúmeros tipos de sistemas operacionais, considerando que eles existem há mais de meio século. No topo, estão os sistemas operacionais para computadores de grande porte. Esses computadores são usados por empresas que trabalham com dados massivos e são conhecidos como mainframes. Eles possuem milhares de discos, com milhões de gigabytes de armazenamento, além de capacidades massivas de processamento. Atualmente, também são muito utilizados para servidores web.

Outro tipo de computador potente são os computadores paralelos, que nada mais são do que vários computadores conectados em paralelo, com múltiplas CPUs funcionando simultaneamente. Sistemas operacionais para esse tipo de computador precisam ser especiais para garantir uma boa comunicação entre as máquinas. Eles são conhecidos como sistemas operacionais de multicomputadores. Inclusive, hoje em dia, sistemas comuns já possuem suporte para processadores multinúcleo, porém não no mesmo nível desses sistemas especiais.

E, claro, não poderiam faltar os sistemas operacionais comuns, que usamos no dia a dia, como Windows e Linux. Esses sistemas dão suporte a multitarefas e buscam melhorar a experiência do usuário. São utilizados principalmente para pesquisas na web, edições de texto, planilhas, jogos, etc.

Descendo ainda mais, encontramos os sistemas operacionais portáteis, como Android e iOS. Esses sistemas são pequenos, mas já possuem suporte para multinúcleos e costumam incluir mais sensores, como tela sensível ao toque, câmeras, etc.

Os sistemas operacionais embarcados são aqueles que não podem ser alterados e não permitem a instalação de softwares externos pelo usuário, como, por exemplo, os de um micro-ondas ou uma geladeira. Esses sistemas já vêm com softwares pré-instalados na memória ROM.

Existem computadores minúsculos conhecidos como sensores, que funcionam em conjunto. Eles são muito utilizados para fins geográficos. Esses computadores possuem baterias, CPUs, RAM e ROM, com foco principal na economia de energia. Por isso, utilizam sistemas operacionais simples para reduzir o consumo de RAM e bateria. Outro tipo de computador minúsculo são os smartcards, que possuem sistemas operacionais de cartões inteligentes. Eles contam com ROM e pequenas reservas de memória. São do tamanho de um chip de cartão de crédito e podem ter diferentes funções. Alguns realizam apenas uma tarefa, como pagamentos ou autenticação de senhas de acesso, enquanto outros possuem múltiplas funções.

Por fim, os sistemas operacionais de tempo real, ou tempo real crítico, são muito usados na área industrial. Os não críticos são empregados em situações onde o tempo é uma ferramenta importante, mas eventuais atrasos não causam grandes problemas. Já nos sistemas críticos, o tempo é crucial e não pode haver nenhum atraso sequer. Um exemplo disso é o processo de montagem de um carro, onde qualquer atraso de um robô ou máquina pode comprometer a produção e danificar o veículo.

#
**1.5** Conceitos de Sistemas Operacionais

Começando pelos processos, eles são um conceito muito importante que ocorre enquanto um programa é executado. Sua principal função é manter esse programa em ordem. Ao lado dos processos, existem os espaços de endereçamento, que são listas com posições de memória que permitem ao processo ler e escrever.

Os dados do programa, o endereço e todas as informações relacionadas ao programa fazem parte do processo. Uma função importante do processo é preservar o estado em que o programa se encontra, mesmo que ele seja temporariamente interrompido, o que acontece com frequência quando há inúmeros processos ativos.

Dentro do sistema operacional, existe a tabela de processos, que armazena os endereços dos processos e suas informações.

As chamadas mais comuns a que os processos estão sujeitos são as chamadas de término ou criação. Além disso, um processo pode criar outros processos, conhecidos como processos filhos, que também podem gerar novos processos. Em casos como esses, forma-se uma árvore de processos, onde ocorre intensa comunicação entre os processos para garantir a cooperação.

Os espaços de armazenamento ficam na memória, em uma área acessível aos processos. Cada processo tem seu próprio endereço, o que evita conflitos entre os programas.

Existem dois tipos de espaço de endereçamento: o físico e o virtual. O físico corresponde à memória RAM, enquanto o virtual transfere parte dos dados para o disco, permitindo que programas usem mais memória do que está fisicamente disponível.


Um conceito encontrado em todos os sistemas operacionais são os arquivos. Assim como foi visto que os sistemas operacionais utilizam interfaces para esconder a complexidade do hardware, eles também têm formas de facilitar o uso dos discos. Um exemplo disso são os diretórios ou pastas, que servem para agrupar os arquivos.

Além disso, existem as chamadas necessárias para criar, editar, mover e deletar esses diretórios. Assim como os processos, esses diretórios podem ter uma estrutura hierárquica, com diretórios filhos, e essa hierarquia pode durar por longos períodos de tempo — ao contrário dos processos, onde as hierarquias são temporárias, durando apenas alguns segundos.

A proteção é essencial para um sistema operacional, afinal, quem escolheria usar um sistema operacional mal protegido? Cabe ao sistema garantir a segurança dos dados do usuário, como logins, documentos e até contra invasões e diversos tipos de malwares. Para isso, inúmeros sistemas costumam utilizar códigos de proteção, criptografia, permissões restritas a usuários administrativos, entre outras medidas.

#
**1.7** Estrutura de sistemas operacionais


Começando pelo mais comum, o sistema monolítico opera em modo núcleo e tem controle total do hardware. O sistema é capaz de chamar qualquer procedimento, e qualquer procedimento também pode chamar outros, se necessário e útil. Por conta disso, ele se torna rápido e eficiente, porém, mais difícil de gerenciar e mais sensível a falhas em suas rotinas.

O primeiro sistema operacional em camadas foi o THE (Technische Hogeschool Eindhoven), em 1968. Ele possuía seis camadas, e cada uma tinha uma função específica.

A camada 0 era responsável pela alocação do processador e oferecia a multiprogramação básica da CPU. Programadores que usavam esse sistema não precisavam se preocupar com a forma como os múltiplos processos eram gerenciados.

A camada 1 era responsável pela alocação de memória e mantinha espaços para alocar a memória principal em um tambor magnético de 512K palavras, utilizado para armazenar partes dos processos que não cabiam na memória principal. Nessa camada, não era necessário saber onde os processos eram armazenados, pois as páginas eram devolvidas à memória quando necessário e removidas quando não eram mais usadas.

A camada 2 era responsável pela comunicação entre todos os processos e o console principal. Nessa camada, cada processo tinha seu próprio console de operação.

A camada 3 era encarregada dos dispositivos de E/S, armazenando os fluxos de informações que vinham desses dispositivos. Nessa camada, cada processo podia lidar com dispositivos de E/S de forma abstrata e mais acessível.

Por fim, a camada 4 era onde ficavam os programas dos usuários, que não precisavam se preocupar com o gerenciamento das camadas anteriores. A camada 5 era onde ficava o processo operador.

Os micronúcleos têm como principal função atingir alta confiabilidade, dividindo o sistema operacional em módulos pequenos e bem definidos. Eles são executados em modo núcleo, enquanto o restante dos módulos são executados como processos de usuário comum, quase sem poder.

Outra variação do micronúcleo é o modelo cliente-servidor, onde o servidor presta algum serviço e o cliente consome esse serviço. A comunicação entre esses dois ocorre principalmente por mensagens. Grande parte da web opera dessa maneira, com grandes servidores conectados aos clientes por redes.
