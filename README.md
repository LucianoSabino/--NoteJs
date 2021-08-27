#   NoteJs
 Repositório criado para registrar aprendizado de javascript
## Propriedade string

A propriedade [.length](https://codetogo.io/how-to-get-length-of-string-in-javascript/) é usada para retornar o comprimento da string.
- Supondo que você tenha uma variável chamada **texto** , veja como você obteria seu comprimento:

```javascript
	let text = "Hello World";
	text.length; // 11
```
> *Ex: Complete a função de `getCharCount`forma que ela retorne o número de caracteres no `str`parâmetro que ela recebe*

```javascript
	function getCharCount(str)  {
		return str.length
	}
	console.log(getCharCount("Sam"));  // 3
	console.log(getCharCount("Alex 123"));  // 8
	console.log(getCharCount("Charley is here"));  // 15
````

## Métodos básicos de string

Aqui estão alguns métodos comuns que você pode chamar em strings:

### .toLowerCase ( )

- Isso retornará uma nova string que tem todos os seus caracteres em letras minúsculas:

```javascript
	"BLUE".toLowerCase(); // "blue";
```
>*Ex: Complete a função lowerName de forma que ela retorne o parâmetro de nome que recebe em letras minúsculas.*
```javascript
	function lowerName(name)  {
		return name.toLocaleLowerCase()
	}
	console.log(lowerName("Sam"));  // "sam"
	console.log(lowerName("ALEX"));  // "alex"
````
### .toUpperCase ()

- Isso retornará uma nova string que tem todos os seus caracteres em maiúsculas:

```javascript
	"red".toUpperCase(); // "RED";
```
>*Ex: Complete a função shoutMyName de forma que retorne o parâmetro de nome que recebe em letras maiúsculas.*
```javascript
	function shoutMyName(name)  {
		return name.toUpperCase()
	}
	console.log(shoutMyName("Sam"));  // "SAM"
	console.log(shoutMyName("Charley"));  // "CHARLEY"
	console.log(shoutMyName("alex"));  // "ALEX"
````

## Acesso de personagem

Última atualização em maio de 2021

Você pode acessar um caractere específico em uma string usando a sintaxe dos colchetes `[]`.

Você deve fornecer o **índice** do caractere que deseja acessar, começando em 0.

Vamos dar um exemplo em que a variável `language`tem o valor: `"JavaScript"`. Veja como você acessa o primeiro caractere, o segundo e o terceiro:

```javascript
language[0]; //first character
language[1]; //second character
language[2]; //third character

```

Se você gostaria de _depurar_ seu código e ver o resultado de `language[1]`no console, você deve registrar no console da seguinte maneira:

```javascript
console.log(language[1]);

```
>*Ex: Conclua a função de `getFirstCharacter`forma que ela retorne o primeiro caractere do parâmetro de **nome** que recebe. *
```javascript
	function getFirstCharacter(name)  {
		return name[0]
	}
	console.log(getFirstCharacter("Amsterdam"));  // "A"
	console.log(getFirstCharacter("Japan"));  // "J"
````
### Combinando com comprimento

Você também pode combinar o acesso ao caractere com a propriedade **.length** . Então, usando a mesma `language`variável, veja como obter o penúltimo caractere dela:

```javascript
language[ language.length - 2 ]; 
// "p" because it's the second to last character from "JavaScript"


```
Observe que **idioma [language.length]** será `undefined`porque o acesso aos caracteres começa em 0.  
Portanto, para uma string de 9 caracteres, 8 é a posição do último caractere.
>*Ex: Complete a função `getLastCharacter` de modo que retorne o último caractere do parâmetro de nome que recebe.*
```javascript
	function getLastCharacter(name)  {
		return name[name.length -  1]
	}
	console.log(getLastCharacter("Sam"));  // "m"
	console.log(getLastCharacter("Alex"));  // "x"
	console.log(getLastCharacter("Charley"));  // "y"
````
