class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        switch(this.tipo) {
            case 'guerreiro':
                console.log(`${this.nome}, o guerreiro de ${this.idade} anos, empunha sua espada e avança corajosamente!`);
                break;
            case 'mago':
                console.log(`${this.nome}, o mago de ${this.idade} anos, conjura um feitiço poderoso contra seus inimigos!`);
                break;
            case 'arqueiro':
                console.log(`${this.nome}, o arqueiro de ${this.idade} anos, dispara flechas rápidas e precisas nos inimigos!`);
                break;
            default:
                console.log(`${this.nome}, de ${this.idade} anos, prepara-se para o combate!`);
        }
    }
}

// Exemplo de uso:
let heroi1 = new Heroi("Gorim", 35, "guerreiro");
let heroi2 = new Heroi("Elara", 122, "mago");
let heroi3 = new Heroi("Legolas", 287, "arqueiro");
let heroi4 = new Heroi("Frodo", 50, "hobbit");

heroi1.atacar();
heroi2.atacar();
heroi3.atacar();
heroi4.atacar();
