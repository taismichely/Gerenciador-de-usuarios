### Explicação do projeto Usuários 

O index.js cria um objeto da classe UserController(), e por fim chamando a
função desse objeto onSubmit().

### User.js

Está dentro da pasta models, pois ele é o modelo de um usuário, um modelo padarão com 
nome, gênero, aniverário, país, etc.

### UserController.js

É onde controlamos os dados 

### Explicação sobre as datas
Há três maneiras até então conhecidas por mim:

*new Date(2018, 4, 5)* No console, ele vai mostrar um mês antes
*new Date([2018, 4, 5])* No console, ele vai mostar corretamente
*new Date("2018, 4, 5")* No console, ele vai mostar um dia antes, ou sem o fuso horario

### Ao adicionar a data de registro do cadastro de cada usuário
 Precisei colocar *this._register = new Date();* dentro co construtor de classe User().

 Após isso, inseri os getters de cada propriedade. E coloquei o setter de photo, pois ele precisava. É uma prática que deveria ser feita com todas as propriedades.

### Criei uma pasta Classes, para colocar métodos estáticos que meu programa vai precisar, sem ter a necessidade de criar um objeto e seu método.

Nesse caso, foi para fazer uma função que formatasse uma data de registro pronta ao meu sistema.

### Método estático 
Não precisamos instanciar o objeto da classe. Podemos usá-la sem instanciar diretamente da classe

## Validar formulários



## Editando dados EDITAR
Copia-se um formulário verde, nele terá que aparecer os dados que foram salvos.
para isso 

## Editando valores de dados de radio button e checkbox
Ele não mostra os radio button e checkbox ativos caso o usuário tenha ativado durante o cadastro.
Isso digo na edição de dados.

Solução de reconhecer esses dados:
Fazer um switch, qaundo ocorrer uma leitura de fild.type diferente como um checkbox ou radio. Foi utlizado case para essa situação.

## Editando valores de dados. Alterando dados do objeto.
Aqui será inserido os dados que foram editados e irão ser adicionados no formulário. Foi preciso criar uma função somente para um unico metodo, pois ao criar ou editar, a ação de inserir dados novos ao tr é igual, assim foi criado a função addEventsTr(tr);

## Editando imagem com FileReader. Alterando dados no objeto.