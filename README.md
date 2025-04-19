# 🔥 **Pokémon Battle Simulator - Charizard Challenge**  
[![Charizard Challenge](https://img.shields.io/badge/Challenge-Charizard🔥-orange?style=for-the-badge)](https://pokeapi.co/)

Um épico simulador de batalhas Pokémon onde você desafia o lendário **Charizard** com Pokémon aleatórios da 1ª geração!  
Prepare-se para efeitos visuais, sons de batalha e uma disputa baseada em **vantagens de tipo**!

---

<div align="center">
  <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/6.png" alt="Charizard" width="120"/>
  <img src="https://user-images.githubusercontent.com/96122701/233764797-4e0cf614-8a35-4ee6-974c-7a2d01f27d64.gif" alt="Battle GIF" width="200"/>
  <img src="https://user-images.githubusercontent.com/96122701/233765022-99c066e5-57b2-4ab7-8f90-cf1cf373e9b1.gif" alt="Particles" width="200"/>
</div>

---

## 🕹️ Como Jogar

1. ➕ **Clique em "Adicionar Desafiante"** para buscar um Pokémon aleatório
2. ⚔️ **Clique em "Batalhar"** para iniciar a luta com o Charizard
3. 💥 **Aproveite os efeitos visuais e sonoros**
4. 📈 **Veja se o desafiante venceu ou foi derrotado**
5. 🏆 **Os vencedores vão direto para o ranking!**

---

## ⚙️ Mecânicas do Jogo

| Elemento | Descrição |
|---------|-----------|
| 🔄 **Fila de Desafiantes** | Organiza os Pokémon que vão enfrentar o Charizard |
| 🔥 **Sistema de Tipos** | Vantagens e desvantagens entre tipos afetam o dano |
| ❤️ **Barra de Vida Animada** | Reflete o progresso da batalha com cores dinâmicas |
| 💥 **Efeitos Visuais** | Inclui flashes, partículas e explosões |
| 🏆 **Ranking** | Guarda os 5 últimos vencedores no navegador (via localStorage) |

---

## 🧰 Tecnologias Utilizadas

- 🧱 **HTML5**, 🎨 **CSS3** e ⚙️ **JavaScript Puro**
- 📡 [**PokéAPI**](https://pokeapi.co/) para obter dados reais dos Pokémon
- ✨ [**particles.js**](https://vincentgarreau.com/particles.js/) para o fundo animado
- 💾 **localStorage** para salvar o ranking

---

## 🗂️ Estrutura do Código

```js
// Fila de espera
let fila = [];

// Pokémon chefe fixo: Charizard
const chefe = {
  nome: "CHARIZARD",
  imagem: "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/6.png",
  tipo: "FIRE",
  vida: 100
};

// Objeto com vantagens de tipo
const typeAdvantages = {
  FIRE: { GRASS: 2, WATER: 0.5, ROCK: 0.5 },
  // ...
};
```

### Funções principais:

- `adicionarDesafiante()` ➕  
- `iniciarBatalha()` ⚔️  
- `calculateTypeAdvantage()` 📊  
- `atualizarFila()` 🔁  
- `salvarRanking()` 🏅

---

## 🎨 Personalização

Quer mudar o chefe? É só alterar o objeto `chefe`:

```javascript
const chefe = {
  nome: "MEWTWO",
  imagem: "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/150.png",
  tipo: "PSYCHIC",
  vida: 100
};
```

---

## 🚀 Acesse o Jogo no GitHub Pages

Você pode jogar a batalha contra o Charizard diretamente no seu navegador! Clique no link abaixo para acessar a versão online do jogo:

[![Acesse o Jogo Pokémon](https://img.shields.io/badge/Play%20Now-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://robson-ifes.github.io/jogo-batalhapokemon/)

🔗 **Link para o GitHub Pages**:  
[https://robson-ifes.github.io/jogo-batalhapokemon/](https://robson-ifes.github.io/jogo-batalhapokemon/)


---

## 🚀 To-Do Futuro (Sugestões)

- [ ] Adicionar múltiplos modos de dificuldade
- [ ] Som específico para vitória ou derrota
- [ ] Sistema de XP ou estatísticas
- [ ] Trocar o chefe via botão no menu

---

## 📣 Agradecimentos

- [PokéAPI](https://pokeapi.co/) por disponibilizar os dados dos Pokémon
- Comunidade de código aberto pela ajuda na construção do código
