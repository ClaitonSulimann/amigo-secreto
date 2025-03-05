Sorteador de Amigos

Este é um simples programa em JavaScript para adicionar nomes de amigos a uma lista e sortear aleatoriamente um deles.

Funcionalidades

Adicionar amigos a uma lista.

Sortear aleatoriamente um amigo da lista.

Garantir que o mesmo amigo não seja sorteado duas vezes antes de reiniciar a lista.

Remover o último amigo adicionado.

Tecnologias Utilizadas

HTML

CSS

JavaScript

Como Usar

Clone o repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git

Abra o arquivo index.html em seu navegador.

Digite o nome de um amigo e clique no botão para adicioná-lo.

Clique no botão de sorteio para selecionar um amigo aleatório.

Use o botão de remover para apagar o último nome da lista.

Exemplo de Código

let amigos = [];
let listaDeNumerosSorteados = [];

function adicionarAmigo() {
    const nomeInput = document.getElementById("amigo");
    const listaAmigos = document.getElementById("listaAmigos");
  
    if (nomeInput.value) {
        const novoItem = document.createElement("li");
        novoItem.textContent = nomeInput.value;
        listaAmigos.appendChild(novoItem);
        amigos.push(nomeInput.value);
        nomeInput.value = "";
    } else {
        alert("Por favor, digite um nome!");
    }
}

Contribuição

Sinta-se à vontade para contribuir com melhorias! Fique à vontade para abrir um pull request com sugestões ou correções.
