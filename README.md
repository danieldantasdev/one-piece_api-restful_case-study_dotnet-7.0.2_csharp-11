# Problema de domínio?

Num mundo de piratas e marinheiros, deseja-se desenvolver um sistema para gerir tripulações de piratas e marinheiros.
<br>
<br>
Cada `Tripulação` pirata é liderada por um `Capitão`, o líder supremo e responsável pelas decisões finais.
Além do `Capitão`, uma `Tripulação` pode ser composta por vários `Membros`. 
Cada `Tripulação` pode ter vários `Barcos` ou `Navios`, assim como pode ter somente uma `Bandeira`.
Cada `Membro` pode ter várias `Habilidades especiais`, podendo ser por `Haki` ou `Akuma No Mi`.

Cada `Membro` possui as seguintes características:
- Nome
- Apelido Pirata
- Função (ex: navegante, espadachim, cozinheiro, médico)
- Habilidades especiais (pode ter várias)
- Data de entrada na tripulação

Cada `Tripulações` também possuem características importantes:
- Nome
- Símbolo da Tripulação (uma bandeira pirata)
- Saque total acumulado (quantidade de tesouros, ouro, etc.)
- Número de Membros na tripulação
- Lista de Membros pertencentes à tripulação

Cada Membro da tripulação pode possuir um ou mais Tesouros que foram saqueados em aventuras anteriores. Cada Tesouro possui as seguintes características:
- Nome do Tesouro
- Tipo do Tesouro (ouro, joias, artefatos, etc.)
- Valor estimado do Tesouro

Instância mínima:
- Pelo menos uma tripulação liderada por um Capitão.
- Pelo menos três Membros na tripulação.
- Cada Membro possui pelo menos uma habilidade especial.
- Pelo menos dois Tesouros saqueados pela tripulação.
- Uma Rota Planejada com pelo menos duas Etapas.
- Pelo menos um Decreto Pirata emitido pelo Capitão.

**Contexto:**

O mundo de "One Piece" é repleto de piratas que viajam pelos mares em busca de tesouros, aventuras e fama. 
Enquanto isso, a Marinha é responsável por manter a ordem e capturar piratas que desafiam as leis.

**Requisitos:**

1. Existem várias Tripulações de Piratas no sistema, cada uma liderada por um Capitão. Cada Tripulação possui um nome e um Jolly Roger (bandeira pirata).

2. Os Piratas, membros das Tripulações, têm nomes, habilidades especiais e cargos a bordo do navio (por exemplo, Navegador, Cozinheiro, Médico).

3. Os Tesouros são acumulados pelas Tripulações à medida que realizam saques. Cada Tesouro possui um nome, valor e descrição.

4. As Ilhas são locais que as Tripulações podem visitar. Cada Ilha tem um nome, uma descrição e pode conter Tesouros.

5. A Marinha é responsável por rastrear as atividades das Tripulações de Piratas. Cada Marinheiro tem um nome e um nível de autoridade.

6. Quando uma Tripulação de Piratas visita uma Ilha, eles podem encontrar Tesouros e enfrentar Marinheiros.

**Classes de Domínio:**

- `Tripulacao` (Tripulação de Piratas)
    - Propriedades: Nome, Jolly Roger
    - Métodos: Adicionar Pirata, Saquear Tesouro, Visitar Ilha

- `Capitao` (Capitão da Tripulação)
    - Propriedades: Nome, Habilidade Especial
    - Métodos: Nomear Pirata, Definir Cargo

- `Pirata` (Membros da Tripulação)
    - Propriedades: Nome, Habilidade Especial, Cargo

- `Tesouro` (Tesouros coletados)
    - Propriedades: Nome, Valor, Descrição

- `Ilha` (Locais visitados)
    - Propriedades: Nome, Descrição, Tesouros

- `Marinha` (Autoridade que busca capturar Piratas)
    - Propriedades: Nível de Autoridade, Nome

**Relações:**

- Uma `Tripulacao` pode ter vários `Piratas`.
- Uma `Tripulacao` pode saquear vários `Tesouros`.
- Uma `Tripulacao` pode visitar várias `Ilhas`.
- Uma `Ilha` pode conter vários `Tesouros`.
- A `Marinha` pode monitorar várias `Tripulacoes`.
- Um `Ser` pode ser de uma `Raça`.
- Um `Ser` pode ter 0 ou mais `Sonhos`.
- Um `Ser` pode ter 0 ou mais `Apelidos`.
- Um `Ser` pode ter 0 ou mais `Habilidades`.

**Cenários de Uso:**

- Os Piratas adicionam Tesouros ao saquear Ilhas.

- As Tripulações visitam diferentes Ilhas em busca de Tesouros e enfrentam Marinheiros da Marinha.

- A Marinha registra as atividades das Tripulações e tenta capturá-las.

- As Tripulações competem para acumular o maior valor em Tesouros e se tornar a Tripulação mais famosa dos mares.

Este é um exemplo simplificado de um sistema baseado no mundo de "One Piece". Claro, você pode expandir e refinar essas classes de domínio e cenários de uso de acordo com os requisitos específicos do seu projeto. Além disso, você pode criar diagramas de classe e objetos com base nessas classes para ajudar na implementação do sistema.
