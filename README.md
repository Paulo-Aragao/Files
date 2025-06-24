# Repositório de Arquivos JSON

Este projeto utiliza o GitHub Pages para hospedar arquivos JSON estáticos, servindo como uma API simples e gratuita para outros projetos web.

A página principal (`index.html`) funciona como um visualizador, listando todos os arquivos disponíveis e fornecendo links diretos para eles.

---

## Como Usar

### Página de Acesso

Para visualizar a lista de todos os arquivos JSON disponíveis, acesse a página principal:

- **`https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`**

### Acesso Direto aos Arquivos

Para usar os arquivos em seus projetos, utilize as URLs diretas. Por exemplo:

- `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/files/file1.json`
- `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/files/produtos.json`

*Substitua `SEU-USUARIO` e `NOME-DO-REPOSITORIO` pelos seus dados.*

---

## Como Adicionar Novos Arquivos

1.  **Adicione o arquivo**: Coloque seu novo arquivo `.json` dentro da pasta `/files`.
2.  **Atualize a lista**: Abra o arquivo `index.html`, encontre o array `jsonFiles` dentro da tag `<script>` e adicione o caminho para o seu novo arquivo.

```javascript
// Exemplo de atualização no index.html
const jsonFiles = [
    'files/file1.json',
    'files/produtos.json',
    'files/usuarios.json',
    'files/seu-novo-arquivo.json' // <== Adicione a nova linha aqui
];