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
