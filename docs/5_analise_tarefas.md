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
          * **METHOD 2.A.4.A:** Rotina só de ida
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida só de ida)
             * OP 2.A.4.A.1: Tocar em endereço de ida
             * OP 2.A.4.A.2: Digitar o endereço de ida
             * OP 2.A.4.A.3: Tocar em horário de saída da ida
             * OP 2.A.4.A.4: Arrastar no relógio para definir horario de ida
             
          * **METHOD 2.A.4.B:** Rotina só de volta
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida só de volta)
             * OP 2.A.4.B.1: Tocar em endereço de volta
             * OP 2.A.4.B.2: Digitar o endereço de volta
             * OP 2.A.4.B.3: Tocar em horário de saída da volta
             * OP 2.A.4.B.4: Arrastar no relógio para definir horario de volta
               
          * **METHOD 2.A.4.C:** Rotina de ida e volta
             * (SEL. RULE: No op 2.2 Usuário deve ter selecionado corrida de ida e volta)
             * OP 2.A.4.C.1: Tocar em endereço de ida
             * OP 2.A.4.C.2: Digitar o endereço de ida
             * OP 2.A.4.C.3: Tocar em endereço de volta
             * OP 2.A.4.C.4: Digitar o endereço de volta
             * OP 2.A.4.C.5: Tocar em horário de saída da ida
             * OP 2.A.4.C.6: Arrastar no relógio para definir horario de ida
             * OP 2.A.4.C.7: Tocar em horário de saída da volta
             * OP 2.A.4.C.8: Arrastar no relógio para definir horario de volta
  
        * OP. 2.5: Clicar nos botões dos dias da semana dessa rotina
        * OP. 2.6: Clicar na modalidade de transporte utilizada
        * OP. 2.7: Confirmar o cadastro de rotina
    
