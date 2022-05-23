<h1> JSON e Serialização </h1>

<h2>Tópicos abordados no tema:</h2>
<ul>
  <li>O que é serialização e deserialização? Quando precisamos usar essa técnica?
     </li>
    <li>O que é e quais as regras do formato JSON?
       </li>
      <li>Como podemos converter um objeto JS em JSON e vice versa?
         </li>
        <li>O que acontece quando serializamos objetos que tenham uma função dentro? Por quê?
           </li>
          <li>O que é XML? Como serializamos um objeto JS em XML?
             </li>
            <li>O que é YAML? Como serializamos um objeto JS em YAML?
               </li>
  <li> Compare um objeto serializado em JSON, XML e YAML.
  </li>
    </ul>
    
<h2> O que é serialização e deserialização? Quando precisamos usar essa técnica?</h2>
<h2>O que é e quais as regras do formato JSON?</h2>
<p>
JSON, que significa JavaScript Object Notation, é uma formatação utilizada para estruturar dados em formato de texto e transmiti-los de um sistema para outro, como em aplicações cliente-servidor ou em aplicativos móveis. Uma maneira de utilização é por meio de requisições AJAX, em que a aplicação recupera os dados armazenados no servidor de hospedagem sem a necessidade de recarregar a página.

A especificação JSON surgiu por volta do ano 2000, mas só passou a fazer parte da linguagem JavaScript após o lançamento da versão 5 do ECMAScript. Atualmente, esse formato é suportado por diversos tipos de linguagem de programação, além de ser uma alternativa mais leve que o modelo XML.</p>
    
<h2>Como podemos converter um objeto JS em JSON e vice-versa?</h2>
<p>O método JSON.parse() analisa uma string JSON, construindo o valor ou um objeto JavaScript descrito pela string. Uma função reviver opcional pode ser fornecida para executar uma transformação no objeto que será retornado.</p>

```
const text = '{"name": "vitoria", "ano": 2022}';
const converteJson = JSON.parse(text);
console.log(converteJson);
```

<h3>Convertendo um JSON em JS:</h3>

<p>O método JSON.stringify() converte valores em javascript para uma String  JSON. Esses valores podem ser substituidos especificando a função replacer, ou incluindo somente as propriedades específicas, quando o array do replacer for especificado.</p>

```
const json = {"name": "vitoria", "ano": 2022};
const text = JSON.stringify(json);
console.log(text);
```

<h2>O que acontece quando serializamos objetos que tenham uma função dentro? Por quê?</h2>

<h2>O que é XML? Como serializamos um objeto JS em XML?</h2>
<p>O XML é uma linguagem de marcação, ou seja, um conjunto de regras utilizado para formatar documentos de maneira que os dados possam ser lidos e interpretados por diferentes sistemas. No Brasil, ficou popularizado por ser o tipo de arquivo mais utilizado na emissão de notas fiscais digitais.</p>

<b>Exemplo de uma NF-e em XML:</b>
<img src="https://www.espiaonfe.com.br/images/lab/xml-nfe-estrutura-exemplo.png"/>
<p>Todo XML é constituido por tags que abrem e fecham como HTML.</p>


<h2>O que é YAML? Como serializamos um objeto JS em YAML?</h2>
<h2>Compare um objeto serializado em JSON, XML e YAML</h2>
<h2> Referências bibliográficas:</h2>
<ul>
  <li><a href="https://www.devmedia.com.br/json-tutorial/25275">Json Tutorial</a>
     </li>
    <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/JSON/parse">JSON.parse()</a>
  </li>
  <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify">JSON.stringify()</a>
    </li>
    <li><a href="XML Tutorial">Criando um XML</a>
      <li><a href="https://rockcontent.com/br/blog/json/">O que é JSON</a>
  </li>
  </ul>
