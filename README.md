# Cadastro de Funcionários com JavaScript

Aplicação de estudo que implementa um CRUD de funcionários diretamente no navegador. Permite cadastrar, listar, editar e excluir registros, salvando os dados no `localStorage`.

## Tecnologias

- HTML5 para a estrutura da página e do formulário.
- CSS3 para layout, modal, animação e adaptação a telas menores.
- JavaScript para eventos, manipulação do DOM e operações de cadastro.
- `localStorage` para persistência no navegador.
- Boxicons para os ícones de edição e exclusão.
- Google Fonts para a tipografia.

## Funcionalidades

- Cadastro de nome, função e salário.
- Listagem dos funcionários em uma tabela.
- Edição em um formulário modal.
- Exclusão de registros.
- Verificação de campos vazios antes de salvar.
- Restauração dos registros ao recarregar a página.
- Ajustes de layout para telas com largura de até 700 px.

## Como executar

O projeto não exige instalação de pacotes nem etapa de build.

```bash
git clone https://github.com/aurimarsalvador/crud-javascript.git
cd crud-javascript
```

Abra o arquivo `index.html` no navegador. Para trabalhar com uma origem local consistente, também é possível usar a extensão Live Server do VS Code ou um servidor HTTP local.

Com Python 3 instalado:

```bash
python -m http.server 8000 --bind 127.0.0.1
```

Acesse `http://localhost:8000`. Em sistemas que usam `python3`, substitua o nome do comando. No Windows, também é possível usar `py -m http.server 8000 --bind 127.0.0.1`.

As fontes e os ícones são carregados de serviços externos e precisam de conexão à internet para aparecer conforme o layout original.

## Como usar

1. Clique em **Incluir**.
2. Preencha nome, função e salário.
3. Clique em **Salvar**.
4. Use os ícones da tabela para editar ou excluir um registro.
5. Recarregue a página para conferir a persistência.

Os dados ficam na chave `dbfunc` do `localStorage`, apenas no navegador e na origem utilizados. Eles não são sincronizados entre dispositivos; limpar os dados do site também remove os cadastros.

## Organização

| Arquivo | Responsabilidade |
| --- | --- |
| [index.html](index.html) | Tabela, formulário e estrutura do modal |
| [style.css](style.css) | Estilos, responsividade e animação |
| [script.js](script.js) | CRUD, eventos e persistência local |

## Conceitos praticados

Manipulação do DOM, eventos de clique, arrays e objetos, serialização com JSON, armazenamento local e atualização da interface a partir dos dados.

## Verificação manual

Crie um registro de exemplo, edite a função, recarregue a página e confira os valores. Depois exclua o registro e verifique se a remoção permanece após outra atualização.

O repositório ainda não possui testes automatizados.

## Possíveis evoluções

- Validar melhor os valores de salário.
- Adicionar pesquisa e ordenação.
- Melhorar a acessibilidade do modal.
- Integrar o cadastro a uma API e a um banco de dados.

## Autor

[Aurimar Salvador](https://github.com/aurimarsalvador)
