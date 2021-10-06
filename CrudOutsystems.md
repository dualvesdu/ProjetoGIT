Projeto CRUD no Outsystems

Com as práticas de desenvolvimento de aplicações, disponibilizo a extensão .OML código na plataforma Outsystems
para que de forma simples um projeto com módulo reativo de um form para criar, listar, editar e deletar campos.

O projeto simples consiste em três na base de dados Clients:
Name - tipo de dados text
Birthday - tipo de dados Date
Address - tipo de dados text

Foi criado dois "screen", o primeiro screen que é o principal com o nome "Home"
onde visualizamos os inputs do form que é gerado do segundo screen "Clents"

No Screen "Home" foi inserido os elementos:
Icon "plus" com o link para o segundo Screen
E no MainContent foi atribuido uma Entidade da Database chamada "Clients" com os três atribuidos já mencionados acima
*LISTAR*
Foi adicionado um button como onde foi criado um parametro "ClientId" e consequente atribuido na ação com um "DeleteClients"
*DELETE*

No Screen "Clients" foi inserido os elementos:
Form com disposição de inputs para os três atributos;
Um button para guardar na base os inputs e assim temos a ação onde é atribuido nas propriedades um "GetClientById.List.Current"
*CREATE*

Para ter a funcionalidade de alterar, foi explorado "Widget Tree" na página Home e na opção MainContent, atribuimos o link "MainFlow\Create"
e adicionamos a expressão "GetClients.List.Current.Clients.Name"
*UPDATE*

Esse é o link para acesso a aplicação
https://personal-gzjzarnf.outsystemscloud.com/ProjectCrud/Home

Link do código para descarregar
https://drive.google.com/file/d/17HKlgu8TTAK1f1sP2RocFJOGX8l0Sbuv/view?usp=sharing