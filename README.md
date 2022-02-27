# Typescript-Memo

## Primitive types
- number: All numbers are initialized as floats in js
- string: All texts
- boolean: true or false

```
Remember in js all primitives are written in lowercase
```

## Typescript using types in a function
```ts
function add(n1: number, n2: number, showResult: boolean, phrase: string){
    const result = n1 + n2;
    if(showResult){
        console.log(phrase + result);
    }else{
        return result;
    }
}
```






# Nx.dev

## Installation 
```bash
sudo npm install -g nx
```


## Util commands
```bash
#Prints a graph with every change since the last commit
nx affected:dep-graph
```
## libs
```bash
nx generate @nrwl/node:lib number-utils --publishable --importPath=@stores/number-utils
```
- De esta manera podremos crear librerias que luego van a poder ser publicadas en npm si queremos. 
- Tambien nos da la facilidad de importar dentro de nuestras apps dichas libs con el path del importPath (en este caso "@stores/number-utils")

