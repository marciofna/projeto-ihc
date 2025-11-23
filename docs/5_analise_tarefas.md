 # Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

1. HTA
2. GOMS
3. CTT

## 1. Cadastro de usuário

### HTA

<img width="1559" height="690" alt="image" src="https://github.com/user-attachments/assets/759e056f-9246-4d31-b9a1-9f7b4847d92b" />



| Objetivos/Operações                                                                      | Problemas e recomendações                                                                                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0\. Cadastro de usuário<br>1>2>3                                                         | Input: Formulário de criação de conta, Formulario de criação de rotina<br>Feedback: Usuário criado com sucesso<br>Plano: Seguir o fluxo de criação de conta e depois seguir o fluxo de criação de rotina                                                                     |
| 1\. Criação de conta<br>1 > 2                                                            | Plano: Preencher formuçario de cadastro de conta e depois confirar cadastro via email institucional                                                                                                                                                                          |
| 1.1 Informar email institucional                                                         | Recomendação: bloquear o campo de email para já incluir @fei.edu.br                                                                                                                                                                                                          |
| 1.2 Confirmar cadastro por email                                                         |                                                                                                                                                                                                                                                                              |
| 2\. Cadastro de rotinas<br>1 + 2                                                         | Plano: Preencher detalhes a partir do tipo de viagem e informar os dias em que a rotina se repete<br>Problema: Usuário não pode ter duas rotinas cadastradas para uma mesma data e horário<br>Recomendação: não permitir que o usuário cadastre uma rotina que obstrua outra |
| 2.1. Informar tipo de viagem (Ida, Volta, Ambos)<br>1/2/3                                |                                                                                                                                                                                                                                                                              |
| 2.1.1. Informar local de Saida, Horário de saida                                         | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 2.1.2. Informar local de Retorno, Horário de Retorno.                                    | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 2.1.3. Informar local de Retorno, Horário de saida, local de Retorno, Horário de Retorno | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 2.2. Informar dias em que a rotina se repete                                             |                                                                                                                                                                                                                                                                              |
| 3\. Validar se usuário desejesa cadastrar outra rotina<br>1/2                            | Plano: Cadastrar nova rotina OU encerrar o fluxo                                                                                                                                                                                                                             |
| 3.1 Informar sucesso no cadastro                                                         |                                                                                                                                                                                                                                                                              |

### GOMS
* **GOAL 0: Cadastro de usuário**
    * **GOAL 1: Criar conta de usuário**
        * OP. 1.1: Tocar no botão cadastro de usuário
        * OP. 1.2: Tocar no campo Email
        * OP. 1.3: Digitar apenas o inicio do email estudantil (@fei.edu.br obrigatório)
        * OP. 1.4: Tocar no campo de nome de usuário
        * OP. 1.5: Digitar o nome desejado
        * OP. 1.6: Tocar no campo de senha
        * OP. 1.7: Digitar a senha desejada
        * OP. 1.2: Tocar no campo de confirme sua senha
        * OP. 1.9: Digitar novamente a senha desejada
        * OP. 1.10: Clicar em confirmar cadastro)
        * OP. 1.11: Abrir provedor de email institucional
        * OP. 1.12: Abrir email recebido
        * OP. 1.13: Tocar no link para confirmar cadastro
        * OP. 1.14: Retornar para o aplicativo para concluir cadsatro 
          

    * **GOAL 2: Cadastro de rotina**
        * **METHOD 2.1.A:** Primeira rotina
            * (SEL. RULE: Usuário não possui nenhuma rotina cadastrada, a primeira rotina é obrigatória, sistema ira abrir sozinho o formulario)
        * **METHOD 2.1.B:** Nova rotina
            * (SEL. RULE: Usuário já possui pelo menos uma rotina)
            * OP. 2.1.B.1: Clicar em adicionar uma nova rotina.
        * OP. 2.2: Tocar em tipo de rota
        * OP. 2.3: No formulario suspenso, tocar no tipo de viagem
        * GOAL 2.4: Definir detalhes da rotina
          * **METHOD 2.4.A:** Rotina só de ida
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida só de ida)
             * OP 2.4.A.1: Tocar em endereço de ida
             * OP 2.4.A.2: Digitar o endereço de ida
             * OP 2.4.A.3: Tocar em horário de saída da ida
             * OP 2.4.A.4: Arrastar no relógio para definir horario de ida
             
          * **METHOD 2.4.B:** Rotina só de volta
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida só de volta)
             * OP 2.4.B.1: Tocar em endereço de volta
             * OP 2.4.B.2: Digitar o endereço de volta
             * OP 2.4.B.3: Tocar em horário de saída da volta
             * OP 2.4.B.4: Arrastar no relógio para definir horario de volta
               
          * **METHOD 2.4.C:** Rotina de ida e volta
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida de ida e volta)
             * OP 2.4.C.1: Tocar em endereço de ida
             * OP 2.4.C.2: Digitar o endereço de ida
             * OP 2.4.C.3: Tocar em endereço de volta
             * OP 2.4.C.4: Digitar o endereço de volta
             * OP 2.4.C.5: Tocar em horário de saída da ida
             * OP 2.4.C.6: Arrastar no relógio para definir horario de ida
             * OP 2.4.C.7: Tocar em horário de saída da volta
             * OP 2.4.C.8: Arrastar no relógio para definir horario de volta
  
        * OP. 2.5: Clicar nos botões dos dias da semana dessa rotina
        * OP. 2.6: Clicar na modalidade de transporte utilizada
        * OP. 2.7: Confirmar o cadastro de rotina
### CTT
<img width="2471" height="1031" alt="image" src="https://github.com/user-attachments/assets/c52b7ce7-27c5-438f-aa4c-5866393451db" />


## 2. Criação de grupo

### HTA

<img width="1973" height="1081" alt="image" src="https://github.com/user-attachments/assets/f639916a-fcc4-470b-8346-117557380b83" />



| Objetivos/Operações                                                                      | Problemas e Recomendações                                                                                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0\. Criar um grupo                                                                       | Input: Rotina do usuário, Detalhes do grupo<br>Feedback: Grupo criado com sucesso<br>Plano: Informar a rotina que o grupo irá se basear, depois Informar detalhes do grupo e depois confirmar a criação do grupo                                                             |
| 1.Informar rotina que será usada no grupo<br>1/2                                         | Plano: Criar a partir de rotina já existente ou criar a partir de uma nova rotina                                                                                                                                                                                            |
| 1.1 Informar rotina já existente                                                         |                                                                                                                                                                                                                                                                              |
| 1.2 Criar apartir de nova rotina<br>1+2                                                  | Plano: Preencher detalhes a partir do tipo de viagem e informar os dias em que a rotina se repete<br>Problema: Usuário não pode ter duas rotinas cadastradas para uma mesma data e horário<br>Recomendação: não permitir que o usuário cadastre uma rotina que obstrua outra |
| 1.2.1 Informar tipo de viagem<br>1/2/3                                                   |                                                                                                                                                                                                                                                                              |
| 1.2.1.1. Informar local de Saida, Horário de saida                                       | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 1.2.1.2. Informar local de Retorno, Horário de Retorno.                                  | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 1.2.1.3. Informar local de saida, Horário de saida, local de Retorno, Horário de Retorno | Problema: Usuário não deve ser capaz de inserir um endereço não existente ou fora do estado de são paulo<br>Recomendação: Validar existencia e localização (estado) do endereço                                                                                              |
| 1.2.2. Informar dias em que a rotina se repete                                           |                                                                                                                                                                                                                                                                              |
| 2\. Informar nome, descrição, quantidade de vagas e modalidade do grupo.                 |                                                                                                                                                                                                                                                                              |
| 3\. Confirmar criação do grupo.                                      |                                                                                                                                                                                                                                                                              |  


### GOMS
* **GOAL 0: Criar um grupo**
    * **GOAL 1: Informar rotina**
        * OP. 1.1: Tocar no botão criar um grupo
	 * **METHOD 1.2.A:** Tocar no botão 'rotina já existente'
            * (SEL. RULE: Usuário deve ter selecionado uma rotina já existente exibida em lista)
        * **METHOD 1.2.B:** Clicar em criar a partir de nova rotina
            * (SEL. RULE: Usuário deve ter selecionado para criar a partir de uma rotina não cadastrada em sua conta)
            * OP. 1.2.B.1: Clicar em adicionar uma nova rotina.
			* OP. 1.2.B.2: Clicar no tipo de viagem.
			* GOAL 1.2.B.3: Definir detalhes da rotina
				* **METHOD 1.2.B.3.A:** Rotina só de ida
					* (SEL. RULE: No op 1.2.B.2 Usuário deve ter selecionado corrida só de ida)
					* OP 1.2.B.3.A.1: Tocar em endereço de ida
					* OP 1.2.B.3.A.2: Digitar o endereço de ida
					* OP 1.2.B.3.A.3: Tocar em horário de saída da ida
					* OP 1.2.B.3.A.4: Arrastar no relógio para definir horario de ida
				 
				* **METHOD 1.2.B.3.B:** Rotina só de volta
					* (SEL. RULE: No op 1.2.B.2 Usuário deve ter selecionado corrida só de volta)
					* OP 1.2.B.3.B.1: Tocar em endereço de volta
					* OP 1.2.B.3.B.2: Digitar o endereço de volta
					* OP 1.2.B.3.B.3: Tocar em horário de saída da volta
					* OP 1.2.B.3.B.4: Arrastar no relógio para definir horario de volta
				   
				* **METHOD 1.2.B.3.C:** Rotina de ida e volta
					* (SEL. RULE: No op 1.2.B.2 Usuário deve ter selecionado corrida de ida e volta)
					* OP 1.2.B.3.C.1: Tocar em endereço de ida
					* OP 1.2.B.3.C.2: Digitar o endereço de ida
					* OP 1.2.B.3.C.3: Tocar em endereço de volta
					* OP 1.2.B.3.C.4: Digitar o endereço de volta
					* OP 1.2.B.3.C.5: Tocar em horário de saída da ida
					* OP 1.2.B.3.C.6: Arrastar no relógio para definir horario de ida
					* OP 1.2.B.3.C.7: Tocar em horário de saída da volta
					* OP 1.2.B.3.C.8: Arrastar no relógio para definir horario de volta
				
				* OP. 1.2.B.4: Clicar nos botões dos dias da semana dessa rotina
				* OP. 1.2.B.5: Clicar na modalidade de transporte utilizada
				* OP. 1.2.B.6: Clicar em salvar rotina
	
	* **GOAL 2: Informar descrição do grupo**
		* OP. 2.1: Tocar no campo nome do grupo
        * OP. 2.2: Digitar nome do grupo
		* OP. 2.3: Tocar no campo descrição do grupo
		* OP. 2.4: Digitar descrição do grupo
		* OP. 2.5: Tocar na modalidade do grupo
		* OP. 2.6: Tocar no campo vagas do grupo
		* OP. 2.7: Arrastar para definir quantidade de vagas do grupo
		* OP. 2.8: Tocar em salvar grupo


### CTT

<img width="1996" height="1087" alt="image" src="https://github.com/user-attachments/assets/abf30691-7f57-4d28-bb82-27347479f40d" />


## 3. Iniciar Viagem


### HTA

<img width="1434" height="645" alt="image" src="https://github.com/user-attachments/assets/925651b6-7bc1-4fd6-930d-d96a30f3649a" />

| Objetivos/Operações                                   | Problemas e Recomendações                                                                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0\. Iniciar uma viagem<br>1>2                         | Input: Grupo da viagem, confirmação de presença dos passageiros.<br>Feedback: Viagem iniciada com trajeto montado incluindo os pontos de parada para buscar passageiros confirmados<br>Plano: Selecionar grupo da viagem depois Iniciar a viagem com os passageiros confirmados                                                               |
| 1\. Selecionar grupo da viagem                        | Ação: O horário da viagem deve estar proximo ao cadastrado na rotina para poder confirmar a mesma<br><br>Recomendação: Notificar por push quando o horário permitir a abertura da viagem                                                                                                                                                      |
| 2\. Iniciar a viagem<br>1/2                           | Plano: Iniciar viagem sem todos os passageiros presentes OU Iniciar viagem com todos os passageiros presentes                                                                                                                                                                                                                                 |
| 2.1 Iniciar viagem sem todos os passageiros presentes | Problema: não deve ser possivel iniciar a viagem se nenhum passageiro tiver confirmado.<br>Recomendação: bloquear o inicio da viagem caso nenhum passageiro tenha confirmado.<br>Recomendação 2: exibir mensagem caso nem todos os passageiros tenham confirmado (incentivar para aguardar mais tempo), porem permitir que inicie mesmo assim |
| 2.2 Iniciar viagem com todos os passageiros presentes |                                                                                                                                                                                                                                                                                                                                               |

### GOMS
* **GOAL 0: Iniciar uma viagem**
    * **GOAL 1: Selecionar grupo da viagem**
        * OP. 1.1: Tocar no grupo
		* OP. 1.2: Tocar em iniciar viagem do grupo
		* OP. 1.3: Aguardar estar próximo do horário da viagem
		* OP. 1.4: Selecionar em confirmar viagem do grupo
	* **GOAL 2: Iniciar a viagem**
		* OP. 2.1: Aguardar a confirmação de pelo menos um passageiro
			* **METHOD 2.2.A:** Iniciar viagem sem todos os passageiros presentes
				* (SEL. RULE: O dono do grupo deve querer iniciar a viagem sem a confirmação de todos os passageiros, 1 passageiro minimo é exigido)
				* OP. 2.2.A.1: Tocar em iniciar a viagem.
				* OP. 2.2.A.2: Tocar em confirmar que um passageiro não esta presente
			* **METHOD 2.2.B:** Iniciar viagem com todos os passageiros presentes
				* (SEL. RULE: Todos os passageiros devem ter confirmado presença na viagem)
				* OP. 2.2.B.1: Tocar em iniciar a viagem.

### CTT

<img width="1108" height="890" alt="image" src="https://github.com/user-attachments/assets/18f7a21c-2839-4f53-a58e-60c79669bf01" />


## 4. Realizar check in na viagem

### HTA
<img width="1429" height="695" alt="image" src="https://github.com/user-attachments/assets/ae4a9094-bfe0-4589-ba8b-ff91ddb7b6eb" />



| 0\. Realizar check in em viagem (Passageiro)    | Input: Confirmação de presença, Confirmação de check in<br>Feedback: Usuário deu check in na viagem e esta viajando nela.<br>Plano: Confirmar a presença na viagem DEPOIS confirmar a entrada no veículo |
| ----------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1\. Confirmar presença na viagem<br>1>2         | Plano: Selecionar a viagem depois confirmar a presença                                                                                                                                                   |
| 1.1 Selecionar a viagem                         |                                                                                                                                                                                                          |
| 1.2 Confirmar a presença na viagem              | Ação: O dono do grupo deve ter aberto a viagem para o passageiro poder fazer a confirmação<br><br>Recomendação: Notificar passageiro quando o dono do grupo abrir a viagem.                              |
| 2\. Confirmar entrada no veículo<br>1>2         | Plano: Monitorar posição do veículo DEPOIS confirmar a entrada no veículo                                                                                                                                |
| 2.1 Monitorar a posição do veículo<br>1+2       | Plano: Acompanhar veículo por mapa E receber notificação de veículo próximo                                                                                                                              |
| 2.1.1 Acompanhar veículo pelo mapa              |                                                                                                                                                                                                          |
| 2.1.2 Receber notificação de chegada do veículo |                                                                                                                                                                                                          |
| 2.2 Confirmar a entrada no veículo              | Ação: O dono do grupo deve estar próximo (em distancia real) do passageiro para permitir o check in                                                                                                      |

				
* **GOAL 0: Realizar check in em viagem**
    * **GOAL 1: Confirmar presença na viagem**
        * OP. 1.1: Tocar na viagem exibida na lista
		* OP. 1.2: Tocar em confirmar presença na viagem
	* **GOAL 2: Confirmar entrada no veículo**
		* **GOAL 2.1: Monitorar o veículo**
			* **GOAL 2.1.1: Acompanhar distancia pelo mapa**
				* OP. 2.1.1.1: Tocar no botão de mapa da viagem
				* OP. 2.1.1.2: utilizar gestos de pinça e arrastar para acompanhar o veículo em movimento
			* **GOAL 2.1.2: Receber notificações de distancia do veículo**
				* OP. 2.1.1.1: Perceber notificação de veículo próximo
				* OP. 2.1.1.1: Perceber notificação de chegada do veículo
				
				
		* **GOAL 2.2: Confirmar entrada no veículo**
			* OP. 2.2.1: Aguardar estar próximo (15 metros) do veículo do dono do grupo
			* OP. 2.2.2: Tocar no pop up de check in quando disponivel
			* OP. 2.2.3: Confirmar check in na viagem

### CTT

<img width="1361" height="850" alt="image" src="https://github.com/user-attachments/assets/12b62843-d033-4811-ac5b-490ebf1c425e" />

