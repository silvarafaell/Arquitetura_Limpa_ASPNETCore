Curso Arquitetura Limpa com ASP.NET Core no nextwave(LuisDEV)

### Fundamentos de Arquitetura Limpa
 - Arquitetura é a organização fundamental de um sistema, incluindo seus componentes, o relacionamento entre eles, o ambiente, e os principios em que se baseia sua construção
 - Geralmente representados com a descrição de um estrutura , se utilizando tambem as vezes de um diagrama ou um desenho.
 - É uma arquitetura amplamente utilizada em projetos .NET
 - Proposta por Robeert Martin(Uncle Bob), com foco em promover a testabilidade, desacoplamento, coesão, e reusabilidade de código.
 - Tem como foco o domínio do sistema, tendo em sua essência o Domain-Driven Design
 - Tem diversas variaçõe, mas a essência é a mesma
 - Sua estrutura é dividida em 4 camadas principais, sendo elas
   - Core
   - Infrastructure
   - Application
   - API/UI
 ### Camadas da Arquitetura Limpa
  - Camada Core
   - Camada central da Clean Architecture, contendo a expressão em código do domínio do negócio
   - Alguns conceitos e componentes do Domain-Driven Design são expressados aqui, como
     - Entidades
     - Value Objects
     - Repositórios(Interfaces)
     - Eventos
   - Os principais componentes que geralmente estao contidos aqui são:
     - Entidades e Agregados
     - Values Objects
     - Factories
     - Repositorios(Interface)
     - Enums relacionados a outros componentes dessa camada
     - Serviços de Domínio
     - Exceções de Domínio
 - Camada Infrastructure
   - Camada responsavel por integração com componentes de infraestrutura, como acesso a dados, caching, serviços de computação em nuvem, outros sistemas (externos ou              internos a organização), entre outros.
   - Cada um dos subitens pode ser dividido em projetos proprios, como:
     - Persistence
     - Integration
     - Cloud Services
     - Caching
     - Authentication
   - Os principais componentes que geralmente estão contidos aqui são:
     - Classes relacionadas a acesso a dados, como contexto de dados e implementação de Repositorios
     - Serviços de Infraestrutura, que permite integração com serviços anteriormente citados neste tópico.
     
