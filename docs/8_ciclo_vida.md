**CICLO DE VIDA DE ENGENHARIA DE USABILIDADE**

![Ciclo de vida](imagens/ciclo_de_vida.png)

1. **Características da Plataforma**  
   

| Característica | Descrição |
| :---- | :---- |
| Descrição do Software | **Frontend:** A interface do usuário se trata de um aplicativo para Smarthphones, desenvolvido em JavaScript com React Native. <br>**Backend:** Solução desenvolvida em .NET 8, utiliza recursos da Google Cloud como provedor de Mapas e serviços de localização. <br>**Infraestrutura:** Serviço sera hospedado na Azure (Recursos: Azure App service, Azure CDN), banco de dados postgres hospedado na neondb. |
| Descrição do Hardware |  **Ambiente do usuário:** Smartphones android compativeis. <br> **Ambiente do servidor:** Hospedagem na azure cloud utilizando recurso do App Service |
| LISTA DE Capacidades da Plataforma (com explicação) | **Escalabilidade:** O Azure App Service será configurado para escalar horizontalmente em caso de utilização acima de 70% da capacidade. <br> **Compatibilidade:** O desenvolvimento em React Native permite a criação de uma interface acessivel por uma grande variedade de smartphones, trazendo a possibilidade de lançar o aplicativo para IOS futuramente. |
| LISTA DE Restrições da Plataforma (com explicação) | **Dependencia de conectividade:** O sistema distribuido requer conexão com a Internet para seu funcionanemto, também é necessário uma baixa latencia para bom funcionamento dos serviços de localização em tempo real da aplicação. <br>  **Custo de operação variavel:** por utilizar funções de escalamento automático, o custo de operação é baseado no número de acessos.|

2. **Princípios Gerais do Projeto (INCREMENTAR TABELA)**     

| Nome | Descrição | Link |
| :---- | :---- | :---- |
| Descrição do Contexto | O aplicativo será utilizado por alunos e professores do Centro Universitário FEI para organizar viagens para o campus e realizar o acompanhamento em tempo real das mesmas. Todos os usuários possuem o mesmo nivel de acesso a aplicação e o equipamento é apenas seu smartphone.|  |
| Lei Geral de Proteção de Dados (LGPD) \- Lei n.º 13.709/2018 | A LGPD é a legislação brasileira que regulamenta o tratamento de dados pessoais. O aplicativo possui funcionalidades que expõe nome, endereço e localização em tempo real do usuário. É necessário que essas informações sejam armazenadas com tecnicas de mascaramento e anonimização para garantir a segurança dos nossos usuários e conformidade com a legislação citada | [https://www.planalto.gov.br/ccivil\_03/\_ato2015-2018/2018/lei/l13709.htm](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm) |
| Lei n.º 10.098/2000 \- Lei da Acessibilidade |  Esta lei brasileira estabelece normas gerais e critérios básicos para a promoção da acessibilidade das pessoas com deficiência ou com mobilidade reduzida. É importante para o projeto porque define diretrizes para tornar produtos e serviços, incluindo interfaces de usuário, acessíveis a todos os usuários, independentemente de suas habilidades físicas ou cognitivas. Os critérios estabelecidos pela funcionalidade devem ser respeitados no desenvolvimento da interface. | [https://www.planalto.gov.br/ccivil\_03/leis/l10098.htm](https://www.planalto.gov.br/ccivil_03/leis/l10098.htm) |
| ABNT NBR ISO 9241 Ergonomia da interação humano-sistema |  Esta série de normas brasileiras, baseadas nas normas ISO 9241, fornece diretrizes e orientações para o design centrado no usuário de sistemas interativos, incluindo a concepção de interfaces de usuário. A parte 210 aborda o processo de design centrado no humano, enquanto a parte 11 fornece orientações específicas sobre usabilidade. Essas normas são importantes para o projeto porque estabelecem princípios e métodos para garantir que a interface do usuário atenda às necessidades e expectativas dos usuários. Para garantir uma boa experiencia com a interface do aplicativo devemos respeitar os principios estabelecidos pela norma. | [https://www.inf.ufsc.br/\~edla.ramos/ine5624/\_Walter/Normas/Parte%2011/iso9241-11F2.pdf](https://www.inf.ufsc.br/~edla.ramos/ine5624/_Walter/Normas/Parte%2011/iso9241-11F2.pdf) |
|  | . |  |

   

3. **Metas de Usabilidade**

   1. **Qualitativo**

    


   2. **Quantitativo**  
    
| Metas | Porcentagem | Justificativa |
| ----- | :---- | :---- |
| Facilidade de … |  |  |
|  |  |  |
|  |  |  |
|  | 1% |  |
|  | 20% |  |
| **Total** | **100%** |  |
