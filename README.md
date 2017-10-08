## WebService Sisalfa

* Sisalfa é um Projeto e Desenvolvimento de um Sistema Colaborativo para apoiar o Processo de Alfabetização de Jovens e Adultos, o principal problema a ser abordado por este projeto de pesquisa é a investigação a respeito do projeto, desenvolvimento e aplicação de um serviço que seja colaborativo e apoie o	processo de alfabetização inspirado nas ideias de Paulo Freire.

## Operations 

| Title|Sisalfa<br/> Projeto e Desenvolvimento de um Sistema Colaborativo para apoiar o Processo de Alfabetização de Jovens e Adultos. |
| ------------- | ------------- |
| **URL**  | /Sisalfa/{Params}  |
| **Method** | **POST**  **GET**  **PUT**  **DELETE** |
|**URL** **Params** |  **Users:**<br /><br />/Sisalfa/getAllUsers<br />/Sisalfa/addUser<br />/Sisalfa/removeUser<br />/Sisalfa/alterUser<br /><br />**Context:**<br /><br />/Sisalfa/getAllContexts<br />/Sisalfa/addContext<br />/Sisalfa/removeContext<br /> /Sisalfa/alterContext<br /><br />**Challenge:**<br /><br />/Sisalfa/getAllChallenges<br />/Sisalfa/addChallenge<br />/Sisalfa/removeChallenge</br>/Sisalfa/alterChallenge</br> |
|**Data** **Params** | { <br />  User: { <br />    nome: [string], <br />  } <br />}<br /><br />{ <br /><br />   Context: {<br />    nome: [string],<br />   idUsuario: [long], <br />    imagem: [string], <br />    som: [string], <br />    video: [string], <br />  } <br />}<br /><br />{ <br /> <br />  Challenge: {<br />    palavra: [string],<br />    idUsuario: [string], <br />    idContexto: [string], <br />    som: [string], <br />    video: [string], <br />    imagem: [string], <br />  } <br />}<br /><br />   |
|**Sample Call in Html file** | $.ajax({<br />  url: "/Sisalfa/addUser",<br />  dataType: "json",<br />  data : { <br />    u: { <br />      nome : "Joao"<br />    }<br />  },<br />  type : "POST",<br />  success : function(r) {<br />    console.log(r);<br />  }<br />});<br />  |
)
