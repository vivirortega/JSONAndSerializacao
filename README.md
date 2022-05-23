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
  </ul>
