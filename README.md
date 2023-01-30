# Funcionamento

O adiciona um event listener ao botão de busca, que ao ser clicado, chama a função getPokemon(). Essa função primeiramente pega o nome do Pokémon digitado pelo usuário e o converte para minúsculas com a ajuda da função lowerCaseName().

Em seguida, a URL da página do Pokémon na Bulbapedia é montada e a requisição é feita através do método fetch(). O retorno é então processado na função parse_data().

A função parse_data() faz uso de algumas técnicas de string para extrair informações da página, tais como a imagem, nome, tipos, número na Pokédex e geração do Pokémon.

Por fim, as informações são renderizadas na tela, dentro de um elemento com classe .pokemonBox.

# Observações

Esse código é baseado na estrutura de páginas da Bulbapedia e pode não funcionar caso haja mudanças na estrutura da página ou se outra fonte de informações for utilizada.
