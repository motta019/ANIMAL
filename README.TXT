README – Atividade Cat e FurColor

Nome: Matheus Nallin

1. O que entendi

O enum FurColor foi criado para representar as cores do pelo do gato.
Cada constante possui um código numérico e um nome de exibição.
Também foi criado o método fromCode para buscar uma cor pelo código.

A classe Cat foi criada herdando de Animal.
Ela representa um gato com informações específicas:
vidas, cor do pelo, se vive dentro de casa, comida favorita,
frequência de ronronar e se é castrado.

2. Decisões tomadas

- Inicializei lives com 7 conforme pedido.
- Usei FurColor como enum para evitar usar String.
- No construtor, o habitat e isWild dependem de isIndoor:
    indoor = DOMESTIC / false
    outdoor = FOREST / true
- displayInfo chama super.displayInfo() e depois mostra os dados do gato.

3. Como testei

Criei objetos Cat com diferentes valores.

Exemplo:

Cat c1 = new Cat(
    "Mimi",
    2,
    4.0,
    FurColor.BLACK,
    true,
    "Fish",
    25,
    true
);

Testei:
- makeSound()
- sleep()
- move()
- purr()
- loseLife()
- displayInfo()

Também testei FurColor.fromCode() com valores válidos e inválidos.