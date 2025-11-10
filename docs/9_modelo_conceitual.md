1) **Cenários de Interação**
> **_NOTE:_**: destacar em negrito o texto alterado entre Cenário Problema e Cenário de Interação

### Cenário de interação A: Usuário Passageiro (Matheus)
Matheus, 17 anos, aluno recém ingressado no Centro Universitário FEI, não possui emprego e nem carteira de motorista. Costumava ir a pé para o ensino médio, porém como mora no Rudge Ramos isso é inviável. Matheus precisa frequentar o campus todo os dias para assistir suas aulas [1]. Ele possui uma mesada que recebe dos pais, esta mesada deve cobrir todos os seus gastos do mês. Matheus percebe que o transporte público é a opção mais acessível, porém considera ele desconfortável e lento. Especialmente considerando que seu deslocamento do campus ocorre em horário de pico [3].

Matheus **então decide utilizar o aplicativo vou pra FEI, ele realiza seu cadastro pelo email institucional e o sistema retorna para ele um formulário para cadastrar sua rotina de viagens, inserindo seus endereços, horários e dias da semana desejados. Uma vez concluido, o sistema exibe para Matheus sugestões de viagens que vão de encontro com sua rotina[5]. Matheus repara que uma aluna chamada Fernanda está saindo da chacará inglesa, a 1.5 km de distancia da sua casa, também no horario noturno. Matheus clica na viagem criada por Fernanda e o sistema exibe, além das informações presentes na tela anterior, a quantidade de vagas disponiveis na viagem e em quais dias. Matheus então solicita para entrar em seu grupo, selecionando todos os dias que deseja.**

**Após um tempo, o aplicativo notifica Matheus que Fernanda aceitou sua participação no grupo e agora possui viagem garantida para todos os dias da semana[4][3]. Garantindo a presença constante de Matheus nas aulas[1][2] e conforto em seus deslocamentos.** 

### Cenário de interação B: Usuário motorista (Fernanda)
Fernanda, 21 anos, Já possui estágio e carteira de motorista. Fernanda utiliza seu carro para ir para a faculdade, costuma dar carona para sua vizinha, que lhe ajuda com os custos da gasolina. Fernanda acha muito conveniente a ajuda de custo e estaria disposta a levar mais pessoas, **Fernanda então acessa o aplicativo VOU PRA FEI, ao selecionar a tela de grupos disponiveis o sistema retorna para ela sugestões de viagens que vão de encontro com sua rotina, Fernanda então clica em criar viagem e o sistema pergunta se ela deseja criar uma viagem baseada em alguma de suas rotinas ou se deseja criar uma viagem do zero, Fernanda então seleciona criar uma viagem baseada na sua rotina, confirmando sua viagem com 3 vagas disponiveis. Após um tempo, Fernanda recebe solicitações de entradas em sua viagem[5], o sistema permite que ela aprove ou recuse os novos integrantes. Como a localização de todas as solicitações era próxima, Fernadna aprova todas as solicitações e agora viaja com seu carro cheio.**


2) **Design Centrado na Comunicação**

**Nome do Cenário: Entrar em uma viagem existente (Matheus)**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Encontrar viagem | U: Preciso encontrar uma viagem para que eu possa participar |
| \> cadastro de rotina  | D: Sua viagem é de ida, volta ou ambos? Quais endereços de ida ou volta? Quais horários? Quais dias da semana? <br> U: Minha viagem é de Ida e volta, meu endereço de ida e volta é (...), saio de casa 18:00 e quero voltar 23:00, todos os dias da semana <br> D: Ok sua rotina foi cadastrada|
| \> sugestões de viagem | D: Baseados na sua rotina, encontrei duas viagens próximas abertas uma pertence a Fernanda, ela é motorista, a 1,5km de você, os horarios são similares e todos os dias da semana batem. Também encontrei a viagem de Lucas, a 2,3 Km de você, ele deseja encontrar passageiros para Uber/99 |
| \> Verificar grupo | U: Quero mais informações sobre a viagem de fernanda <br> D: Ok, além das informações que ja viu na tela anterior, Fernanda possui 3 vagas em seu carro. Fernanda possui uma outra passageira que se encontra na mesma rua cadastrada como partida e retorno da corrida. Na descrição da corrida Fernanda menciona que repartilhar o custo de viagem é bem vindo|
| \> Solicitar entrada no grupo | D: Quero solicitar entrada no grupo de Fernanda, <br> D: Certo, para quais dias da semana você quer participar dessa corrida? <br> U: Todos os dias <br> D: Perfeito, Fernanda recebeu sua solicitação. |


**Nome do Cenário: Criar uma viagem existente (Fernanda)**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
|Criar viagem | U: Quero criar uma viagem |
| \> Criação de viagem  | D: Ok, você deseja importar uma rotina já existente ou criar uma nova do zero? <br> U: importar já exisente <br> D: Certo, você importou a rotina (...), quantas vagas possui para essa viagem? <br> U: 3 Vagas <br> D: Perfeito, sua viagem esta criada |
| \> Aprovar solicitações | D: Você recebeu uma solicitação de entrada no grupo <br> U: qual a solicitação? <br> D: Matheus, a 1,5 km, deseja frequentar o grupo todos os dias. Aprovar? <br> U: Sim <br> D: Agora Matheus faz parte da viagem |

3) **Mapa de Objetivos**
> **_NOTE:_**: cada um coloca seu mapa de objetivos e deverá ter um diagrama de consolidação
<img width="857" height="722" alt="image" src="https://github.com/user-attachments/assets/c591e4ad-c346-43e1-8868-ed7b5a7d207e" />


4) **Esquema Conceitual de Signos**

> **_NOTE:_**: fazer a junção das 3 tabelas abaixo em uma única

| Usuario da aplicação (UA) | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção / recuperação** |
| + id_usuário | domínio | Identificador único do usuário. | texto | não pode ser nulo, único | GUID gerado pela aplicação | n/a|
| email_institucional | Dominio | Email institucional da FEI | texto | o dominio deve ser obrigatoriamente @fei.edu.br | example@fei.edu.br | PP: Campo obrigatório + PA: Validação de formatação |
| Primeiro nome | Dominio | Primeiro nome do usuário | texto | Não pode ser nulo | N/A | PP: Campo obrigatório + PA: Validação de formatação |
| sobrenome | Dominio | sobrenome do usuário | texto | Não pode ser nulo | N/A | PP: Campo obrigatório + PA: Validação de formatação |
| senha | Aplicação | senha para acesso ao perfil | texto | Não pode ser nulo, deve conter caracter especial. Minimo 8 Caracteres | N/A | PP: Campo obrigatório + PA: Validação de força de senha (mínimo 8 caracteres, caractere especial obrigatório)|
| + Rotina (R) R.[id rotina] | Aplicação | Uma rotina no contexto da aplicação se trata dos padrões de viagem de um usuário, obrigatório pelo mneos uma  | Referencia multipla | pelo menos uma referencia é obrigatória | N/A | PP: campo obrigatório + validação de integridade referencial|

| Rotina (R) | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção / recuperação** |
| + id_rotina | domínio | Identificador único da rotina. | texto | não pode ser nulo, único | GUID gerado pela aplicação | n/a|
| Endereço de viagem | Dominio | Endereço da viagem (além do campus) | texto | Endereço localizavel via google maps | -- | PP: Campo obrigatório + PA: Validação de endereço (via API de geolocalização) |
| Horários | Dominio | Horários previstos para ida e volta da viagem | seletor de horário | não será possivel agendar horarios na madrugada | 12:00 | PP: seletor de horário limitado |
| Dias da semana | Dominio | Dias da semana em que a viagem se repete | seleção circular de didas | Domingo não está incluso como opção | nenhum dia selecionado | PP: domingo indisponivel |

| Grupo | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção / recuperação** |
| + id_grupo | domínio | Identificador único do grupo criado. | texto | não pode ser nulo, único | GUID gerado pela aplicação | N/A |
| + rotina (R) | Aplicação |  Um grupo poder ser baseado em uma rotina para sua criação | referencia | N/A | N/A | PP: Apenas rotinas existentes são exibidas para criação do grupo |
| + Usuários participantes (UA) UA.'['id_usuário']'| Aplicação | Usuários que participam do grupo | Referencia multipla| N/A | nenhum | PP: Apenas usuários validos podem participar do grupo |
| Vagas dispinveis | Dominio | Quantas vagas o grupo possui | Numero | Valor numérico que não pode exceder a capacidade do veiculo |  | PP: Campo obrigatório + PA: Não é possivel convidar nem solicitar entrada em um grupo onde a capacidade foi excecida |
| Meio de transporte | Dominio | A modalidade de transporte da viagem | Seleção simples e unica | motorista de aplicativo, carro, moto | | PP: Apenas modalidades suportadas exibidas|






