 # Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

1. HTA
2. GOMS
3. CTT

## 1. Cadastro de usuário

### HTA

<img width="1403" height="355" alt="image" src="https://github.com/user-attachments/assets/4ed7a711-9ef1-45a9-85c7-b3e1b4da337c" />


| Objetivos/Operações                                         | Problemas e recomendações                                                                                                                                                                                                                                                                            |
| ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0\. Cadastro de usuário<br>1>2>3                            | Input: Formulário de criação de conta, Formulario de criação de rotina<br>Feedback: Usuário criado com sucesso<br>Plano: Seguir o fluxo de criação de conta e depois seguir o fluxo de criação de rotina                                                                                             |
| 1\. Criação de conta<br>1 > 2                               | Plano: Preencher formuçario de cadastro de conta e depois confirar cadastro via email institucional                                                                                                                                                                                                  |
| 1.1 Informar email institucional                            | Recomendação: bloquear o campo de email para já incluir @fei.edu.br                                                                                                                                                                                                                                  |
| 1.2 Confirmar cadastro por email                            |                                                                                                                                                                                                                                                                                                      |
| 2\. Cadastro de rotinas<br>1 + 2 + 3                        | Plano: Usuaário deve informar locais de ida e volta E horários de ida e volta E dias da semana em que o padrão se repete.<br>Problema: Usuário não pode ter duas rotinas cadastradas para uma mesma data e horário<br>Recomendação: não permitir que o usuário cadastre uma rotina que obstrua outra |
| 2.1 Informar local de ida e volta                           |                                                                                                                                                                                                                                                                                                      |
| 2.2 Informar horário de ida e volta                         |                                                                                                                                                                                                                                                                                                      |
| 2.3 Informar dias em que a rotina se repete                 |                                                                                                                                                                                                                                                                                                      |
| 3 Validar se usuário desejesa cadastrar outra rotina<br>1/2 | Plano: Cadastrar nova rotina OU encerrar o fluxo                                                                                                                                                                                                                                                     |
| 3.1 Informar sucesso no cadastro                            |   


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
<img width="1253" height="586" alt="image" src="https://github.com/user-attachments/assets/e43fc296-358b-44d0-93f5-fdf3de99eb99" />

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
| 3\. Exibir mensagem de sucesso na criação do grupo.                                      |                                                                                                                                                                                                                                                                              |  


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
<img width="1253" height="586" alt="image" src="https://github.com/user-attachments/assets/e43fc296-358b-44d0-93f5-fdf3de99eb99" />

