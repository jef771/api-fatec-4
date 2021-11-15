# Endurance (API - Fatec sjc)

## Descrição
O sistema Endurance tem como objetivo principal o gerenciamento de eventos, possibilitando a criação e o controle aos colaboradores da empresa. O público externo poderá ser cadastrado no sistema para participar dos eventos, seguindo as restrições sanitárias devido a pandemia e a validação do comprovante de vacinação contra SARS-CoV-2, tanto para dose única quanto para demais doses. Os usuários cadastrados serão notificados sobre novos eventos e atualizações via e-mail.

## Tecnologias
[Spring Boot](https://spring.io/projects/spring-boot)
- Devido ao grande número de materiais disponíveis na internet, adequação ao padrão de projeto MVC e conhecimento prévio o framework Spring Boot foi decisão unânime do grupo.
  
[angular](https://angular.io/cli)
- Foi escolhido também pela grande quantidade de materiais de estudo na internet, fácil integração com o framework Spring Boot e conhecimento prévio. 
  
[Oracle](https://www.oracle.com/br/database/)
- Escolha natural visto que o cliente é a própria Oracle.


## Contribuições
Fiquei encarregado de todo o back end do projeto e, mais tarde, da criação do banco de dados. A arquitetura que eu escolhi foi a MVC, pois, apesar de ser uma arquitetura mais antiga, ainda é muito utilizada no mercado de trabalho - pois funciona! -, desso modo trazendo um aprendizado efetivo para o meu desenvolvimento, adequa-se muito bem às soluções propostas para o problema e requer menos *resources* da parte do estudante - em uma arquitetura de micro serviços por exemplo seria difícil encontrar uma maneira de hospedar pelos menos 5 end-points sem pagar nada - pois, sendo estruturada de maneira monolitica, requer apenas uma hospedagem.

##### Arquitetura MVC
imagem
- Uma visão geral da arquitetura do programa. Já que na parte **View** foi utilizado um framework de frontend (Angular) o backend ficou encarregado da parte Model e Controller e outros pacotes interessantes para o projeto como exception para um melhor controle do fluxo do programa e constant para deixar o código mais legível.

###### Model
imagem de uma entidade
- Um exemplo de uma das 3 entidades do programa, podemos ver a utilização da biblioteca Lombok para simplificar e manter o código mais legível eliminando código **boilerplate** (código recorrente como getters e setters), também podemos observar a utilização do framework Hibernate sendo utilizado no seu modelo JPA para deixar mais simples a comunicação entre o banco de dados e o Model. E na terceira imagem temos um exemplo do mapeamento das diferentes entidades, OneToOne (1-1) no caso referindo-se a um evento sendo criado por um usuário e ManyToMany (N-N) sendo uma lista de participantes para esse evento. As outras 2 entidades seguem esse mesmo modelo de organização.




