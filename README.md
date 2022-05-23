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
<p>Serialização é o processo de transformar algum objeto em um formato de dados que pode ser restaurado mais tarde. As pessoas geralmente serializam objetos para salvá-los no armazenamento ou para enviar como parte das comunicações. A desserialização é o inverso desse processo – tomando dados estruturados a partir de algum formato e reconstruindo-o em um objeto. Hoje, o formato de dados mais popular para serializar dados é JSON. Antes disso, era XML.</p>
<h2>O que é e quais as regras do formato JSON?</h2>
<p>
JSON, que significa JavaScript Object Notation, é uma formatação utilizada para estruturar dados em formato de texto e transmiti-los de um sistema para outro, como em aplicações cliente-servidor ou em aplicativos móveis. Uma maneira de utilização é por meio de requisições AJAX, em que a aplicação recupera os dados armazenados no servidor de hospedagem sem a necessidade de recarregar a página.

A especificação JSON surgiu por volta do ano 2000, mas só passou a fazer parte da linguagem JavaScript após o lançamento da versão 5 do ECMAScript. Atualmente, esse formato é suportado por diversos tipos de linguagem de programação, além de ser uma alternativa mais leve que o modelo XML.</p>

<p> Os dados contidos em um arquivo no formato JSON devem ser estruturados por meio de uma coleção de pares com nome e valor ou ser uma lista ordenada de valores. Seus elementos devem conter:

<b>chave: corresponde ao identificador do conteúdo. Por isso, deve ser uma string delimitada por aspas.</b>
  <br>
<b>valor: representa o conteúdo correspondente e pode conter os seguintes tipos de dados: string, array, object, number, boolean ou null.</b>
</p>

<b>Exemplo de sintaxe:</b>
```
"ano": 2022,
"site": "www.github.com",
"casado": true
```

<b>Exemplo de sintaxe com array de objetos:</b>

``` 
[ 
  {
    "nome": "Vitória", 
    "idade": 25,
    "site:" "www.github.com",
    "casado": false
  }, 
  
  {
    "nome": "Vivi", 
    "idade": 23,
    "site:" "www.github.com",
    "casado": true
  }
]
```
    
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
<p>Lançada em 2001 e inspirada em linguagens como XML, Python, C, entre outras, YAML ou, acrônimo recursivo para “YAML Ain’t Markup Language” é um formato de serialização de dados legível por humanos, sendo bastante utilizado para arquivos de configuração, assim como o JSON e o XML.</p>

<h2>Principais características</h2>
<ul>
  <br>
  <li>
Além da sua familiaridade com XML, possui como principais características:
  </li>

<li>Utilizam um conjunto de caracteres unicode (UTF-8 ou UTF-16);</li>
<li>Possui propósito centrado em dados no lugar de documentos marcados;</li>
<li>Case sensitive;</li>
<li>Pode ser utilizada por diversas linguagens;</li>
<li>É mais legível que o XML e JSON;</li>
<li>Possui uma excelente documentação, entre outros. </li>
</ul>
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
      <li>  <a href="https://www.treinaweb.com.br/blog/o-que-e-yaml">O que é YAML</a></li>
  </li>
  </ul>
