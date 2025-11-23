1) **Avaliação de IHC através de inspeção HEURÍSTICA \[1 solução completa por pessoa da equipe \- todas as telas do projeto\]**

> **_NOTE:_**: SOMENTE VIOLAÇÕES

Dez Heurísticas de Nielsen

**Descrição da avaliação**

Avaliação heurística, definida por Nielsen e Molich (1994), é um método de avaliação de usabilidade onde um avaliador procura problemas de usabilidade numa interface com o usuário através da análise e interpretação de um conjunto de princípios ou heurísticas. Este método de avaliação é baseado no julgamento do avaliador.

1\. Primeiramente, leia e analise as dez heurísticas (ver Tabela 1).

**Tabela 1 \- Conjunto de heurísticas de Nielsen (1994)**

| 1\. | Visibilidade do status do sistema: |
| :---- | :---- |
| O sistema deve sempre manter os usuários informados sobre o que está acontecendo através de feedback apropriado, em um tempo razoável. | Avaliador: Márcio Forner <br> <br> A interface apresenta poucas mensagens de sucesso, não fica claro quando um estado mudou. Especialmente no cadastro de rotina, solicitação de entrada em grupos e confirmação de presença em viagens. Apenas foram feitas mensagens de erro. <br> <br> **Correção:** Incluir mensagem de sucesso no cadastro bem sucedido de itens.  <br> <br> **Nota de gravidade:** 1 - Cosmético: Não há necessidade imediata de solução|
| **2\.** | **Compatibilidade entre sistema e mundo real:** |
| O sistema deve utilizar a linguagem do usuário, com palavras, frases e conceitos familiares para ele, ao invés de termos específicos de sistemas. Seguir convenções do mundo real, fazendo com que a informação apareça em uma ordem lógica e natural. | N/A  |
| **3\.** | **Controle e liberdade para o usuário:** |
| Estão relacionados à situação em que os usuários frequentemente escolhem as funções do sistema por engano e então necessitam de "uma saída de emergência” claramente definida para sair do estado não desejado sem ter que percorrer um longo diálogo, ou seja, é necessário suporte a *undo* e *redo*. | Avaliador: Márcio Forner <br> <br> O modal de cadsatro de rotina fecha imediatamente, mesmo tendo preenchio as maiores partes da informação. Estas são perdidas após o fechamento <br> <br> **Correção:** exigir confirmação antes de fechar o modal de cadastro. <br> <br> **Nota de gravidade:** 2 - Simples: 	Problema de baixa prioridade (pode ser reparado) |
| **4\.** | **Consistência e padrões:** |
| Referem-se ao fato de que os usuários não deveriam ter acesso a diferentes situações, palavras ou ações representando a mesma coisa. A interface deve ter convenções não-ambíguas. | Avaliador: Márcio Forner <br> <br> Na tela de cadastro de rotina, a rotina é chamada de rota. Para todo o resto da aplicação é chamado de rotina. <br> <br> **Correção**: Nomear o signo como rotina para padronizar. <br> <br> **Nota de gravidade:** 1 - Cosmético: Não há necessidade imediata de solução |
| **5\.** | **Prevenção de erros:** |
| Os erros são as principais fontes de frustração, ineficiência e ineficácia durante a utilização do sistema. | N/A |
| **6\.** |  **Reconhecimento em lugar de lembrança:** |
| Tornar objetos, ações, opções visíveis e coerentes. O usuário não deve ter que lembrar informações de uma parte do diálogo para outra. Instruções para o uso do sistema devem estar visíveis ou facilmente acessíveis. | N/A |
| **7\.** | **Flexibilidade e eficiência de uso:** |
| A ineficiência nas tarefas pode reduzir a eficácia do usuário e causar-lhes frustração. O sistema deve ser adequado tanto para usuários inexperientes quanto para usuários experientes. |Avaliador: Livia Lumi Miyabara <br> <br> Telas que serão utilizadas por um motorista com o carro em movimento necessitam de atenção especial. A tela de acompanhamento de viagem está com ícones muito pequenos, botões menores ainda e informações que estão se repetindo ocasionando em poluição visual. <br> <br> **Correção:** Remover a seção "Integrantes da viagem", uma vez que os participantes da viagem já estão listados pela Rota. Aumentar tamanho de todos os botões para facilitar o uso durante trajetos, aumentar tamanho das informações exibidas para facilitar leitura. <br> <br> **Nota de gravidade:** 4 - Catastrófico: Muito grave, deve ser reparado de qualquer forma. */Justificativa:*/ Esse aspecto da interface viola a ISO 15005, que diz respeito a aspectos ergonômicos de interface utilizadas em condução. |
| **8\.** | **Projeto minimalista e estético:** |
| Os diálogos não devem conter informações irrelevantes ou raramente necessárias. Cada unidade extra de informação em um diálogo compete com unidades relevantes e diminui sua visibilidade relativa. |Avaliador: Livia Lumi Miyabara <br> <br> Apesar de aderência ao design minimalista na maior parte do projeto, novamente a tela de viagem citada na heurística 7 esta com informações demais que não são necessárias no momento da viagem. <br> <br> **Correção:** Remover a seção "Integrantes da viagem", uma vez que os participantes da viagem já estão listados pela Rota. <br> <br> **Nota de gravidade:** 4 - Catastrófico: Muito grave, deve ser reparado de qualquer forma. |
| **9\.** | **Auxiliar os usuários a reconhecer, diagnosticar e recuperar erros:** |
| Mensagens de erro devem ser expressas em linguagem natural (sem códigos), indicando precisamente o erro e sugerindo uma solução. | Avaliador: Livia Lumi Miyabara <br> <br>No formulário de cadastro e edição de rotina, não indicamos para o usuário quais campos devem ser corrigidos. <br> <br> **Correção**: caso algum campo obrigatório não esteja preenchido, indicar com contorno vermelho para o usuário. <br> <br> **Nota de gravidade:** 3 - Grave: Problema de alta prioridade (deve ser reparado) |
| **10\.** | **Ajuda e documentação:** |
| Mesmo que seja melhor que o sistema possa ser usado sem documentação, pode ser necessário fornecer ajuda e documentação. Tais informações devem ser fáceis de encontrar, ser centradas na tarefa do usuário, listar passos concretos a serem seguidos e não ser muito grandes. A ajuda deve estar facilmente acessível e on-line. | Avaliador: Livia Lumi Miyabara <br> <br> O sistema não possui documentação geral de uso. <br> <br> **Correção:** Elaboração de uma documentação para auxilio do usuário. <br> <br> **Nota de gravidade:** 3 - Grave: Problema de alta prioridade (deve ser reparado) |

2\. A seguir, avalie o sistema procurando possíveis problemas de usabilidade.   
3\. Quando um problema qualquer for detectado, classifique-o em uma das dez heurísticas de Nielsen, anotando o problema na tabela correspondente e atribuindo o **grau de severidade** (0 até 4\) para este problema (dado pela tabela 2\) e recomece novamente até não encontrar mais problemas de usabilidade.

**Tabela 2 \- Grau de severidade dos problemas de usabilidade**

| Grau de severidade | Tipo | Descrição |
| ----- | :---- | :---- |
| 0 | Sem importância | Não afeta a operação da interface |
| 1 | Cosmético | Não há necessidade imediata de solução |
| 2 | Simples | Problema de baixa prioridade (pode ser reparado) |
| 3 | Grave | Problema de alta prioridade (deve ser reparado) |
| 4 | Catastrófico | Muito grave, deve ser reparado de qualquer forma. |

> **_NOTE:_**: **colocar o print**

Problema 1 (Sem mensagem de sucesso):

![Problema 1 gif](https://github.com/user-attachments/assets/21c21665-d32e-4fe4-8fb4-0b4e49b50947)

Problema 3 (Sem confirmação antes de fechar):

![Problema 3 gif](https://github.com/user-attachments/assets/36d5bd96-a054-42da-a47b-9ba48974c9ea)


Problema 4 (nome rota ao inves de rotina):

<img width="555" height="876" alt="image" src="https://github.com/user-attachments/assets/977fc669-a3a8-4a92-b80c-cb23717892bd" />

Problema 7 e 8 (interface poluida e ineficiente que será usada por motoristas):

<img width="455" height="810" alt="image" src="https://github.com/user-attachments/assets/b08d944e-4d06-43a5-a923-4b369cf94fa0" />

Problema 9: N/A

Problema 10: N/A


> **_NOTE:_**: **escolher a tabela de declaração de violação padrão da equipe**

2) **INDICAÇÃO DE BOAS PRÁTICAS DE HEURÍSTICA \- HEURÍSTICAS NÃO VIOLADAS \[1 solução completa por pessoa da equipe\]**

#### Heuristica 1 - Visibilidade do estado do sistema:
Status de viagem com animações que indicam dinamismo e atividade em progresso.

<img width="343" height="605" alt="image" src="https://github.com/user-attachments/assets/d1c41d23-cc0e-485a-9b2e-d948d80db8a7" />

#### Heuristica 2 - Correspondência entre o sistema e o mundo real:
Os termos utilizados possuem clareza e é facil de entender o que esta acontecendo.

<img width="314" height="555" alt="image" src="https://github.com/user-attachments/assets/4ebcfefe-4e87-4a57-bcbe-a66bdea5ea7e" />

#### Heuristica 3 - Controle e liberdade do usuário::
Modais e telas possuem botão de retorno, botão para fechamento.

<img width="315" height="613" alt="image" src="https://github.com/user-attachments/assets/ab4139a6-eab4-4da9-8668-482bfd625278" />

#### Heuristica 4 -  Consistência e padronização::
Itens de cadastro de rotina e sugestão de viagem possuem elementos visuais em comum.

<img width="332" height="577" alt="image" src="https://github.com/user-attachments/assets/fb3a5d6e-1b75-4e81-9048-d64979c9967a" /> <img width="329" height="528" alt="image" src="https://github.com/user-attachments/assets/46b04663-3e97-42f7-a00b-87dd57710f87" />

#### Heuristica 5 -  reconhecimento em vez de memorização::
Funcionalidades sempre visiveis no rodapé, tela de grupos contem apenas informações de grupos seguindo design minimalista.

<img width="278" height="493" alt="image" src="https://github.com/user-attachments/assets/67474f3c-52f0-4ab3-90b6-a5acdb6f9cc5" />

#### Heuristica 6 -  flexibilidade e eficiência de uso:
Permitimos que nosso usuário crie um grupo diretamente a partir de uma rotina cadastrada

<img width="278" height="454" alt="image" src="https://github.com/user-attachments/assets/1c290e88-1528-49f2-9424-9cf8c480a5cf" />

#### Heuristica 7 - projeto estético e minimalista::
Telas possuem proposito unico, evitando poluição visual

<img width="284" height="497" alt="image" src="https://github.com/user-attachments/assets/a548c55f-8844-40b0-8b1d-74f905fe5e0d" /> <img width="283" height="489" alt="image" src="https://github.com/user-attachments/assets/1f3d2227-1976-47c6-8a95-15fa4a322066" /> <img width="259" height="502" alt="image" src="https://github.com/user-attachments/assets/126f0097-c493-47eb-a972-f5490c70ab09" />

#### Heuristica 8 - prevenção de erros: :
Um dia marcado com X sinaliza um dia lotado, onde não é possivel participar da viagem. Não permitimos o clique no dia, impedindo que usuários façam solicitações

<img width="422" height="123" alt="image" src="https://github.com/user-attachments/assets/1e2283eb-6034-4df0-bfff-da6abee6432e" />

#### Heuristica 9 - Recuperação de erros :
Falha avaliada, não estamos apontando onde está o erro para o usuário.

#### Heuristica 10 -  ajuda e documentação: :
Para o fluxo de cadastro de usuário, deixamos instruções na tela para auxiliar o usuário.

<img width="2103" height="897" alt="image" src="https://github.com/user-attachments/assets/a0c8ce4e-9992-47ce-9514-9608e2e7f843" />
