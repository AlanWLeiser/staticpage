# Cascading Style Sheets ou Folhas de Estilo em Cascata (CSS)

- CSS é um método na qual especificamos propriedades que iram inserir estilização das tags HTML.

#### Tipos de CSS

- Inline
    - As propriedades são inseridas diretamente na tag HTML.
    - Exemplo abaixo:
    ```html
        <h1 style="color:red"> Título da página </h1>
    ```   
    - As propriedades são adicionadas dentro do atributo `style=" "` e divididas com `;`.
    - Exemplo abaixo:
    ```html
        <p style="color:red;font-size:20px;"> Título da página </p>
    ```   

- Interno
    - As propriedades são inseridas em uma tag `<style>` dentro da tag `<head>`
    - Exemplo abaixo:
    ```html
        <head>
        /*Demais tags de configuração*/
        <style>
            .circle{
                width:200px;
                height:200px;
                border-radius:50%;
            }
        </style>
    </head>
    ```   
- Externo
    - As propriedades são inseridas em um arquivo separado com extensão `.css`
    - Exemplo abaixo:
    ```css
    .circle{
        width:200px;
        height:200px;
        border-radius:50%;
    }
        
    ```   

### Seletores

- Ao retirar as propriedades CSS da tag, precisamos de um modo de identificar quais tags devem ser afetadas pelos estilos especificados.
- O método utilizado são os seletores, temos alguns tipos:
    - Universal
    - Por nome de tag
    - Por id
    - Por classe (class)

#### Seletor universal
- Afeta todas as tags o documento HTML
- Seu símbolo é `*`
- Exemplo de uso:
```css
    * {
        margin: 0;
        padding:0;
    }
```
#### Seletor por nome da tag
- Afeta todas as tags o documento HTML do tipo especificado.
- Exemplo de uso:
```css
    img {
        width: 120px;
        border:2px solid red;
    }
```
#### Seletor por id
- Afeta a tag do documento HTML que possui o id especificado.
- Seu símbolo antes do nome é `#`
- Exemplo de uso:
```css
    #tituloDaSecao {
        width: 120px;
        color: pink;
    }
```
- Para que a tag seja afetada é preciso inserir o id, de acordo com o exemplo abaixo. 
    ```html
        <h2 id="tituloDaSecao"> Título da página </h2>
    ```   
- OBSERVAÇÕES:
    - A escrita tem que ser identica!
    - Só deve existir um único id, usado em uma única tag.

#### Seletor por Classe (class)
- Afeta todas as tags do documento HTML que possuem a classe especificado.
- Seu símbolo antes do nome é `.`
- Exemplo de uso:
```css
    .tituloDaSecao {
        width: 120px;
        color: pink;
    }
```
- Para que as tags sejam afetadas é preciso inserir a classe, de acordo com o exemplo abaixo. 
    ```html
        <h2 class="tituloDaSecao"> Título da página </h2>
    ```   
- OBSERVAÇÕES:
    - A escrita tem que ser identica!
    - Pode ser usada diversas vezes ao longo do documento HTML.
