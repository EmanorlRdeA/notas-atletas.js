# notas-atletas.js
Atividade para Certificação
let atletas = [
    {
      nome: "Cesar Abascal",
      notas: [10, 9.34, 8.42, 10, 7.88]
    },
    {
      nome: "Fernando Puntel",
      notas:  [8, 10, 10, 7, 9.33]
    },
    {
      nome: "Daiane Jelinsky",
      notas: [7, 10, 9.5, 9.5, 8]
    },
    {
      nome: "Bruno Castro",
      notas: [10, 10, 10, 9, 9.5]
    }
];

let nomesDosCompetidores = 0
let mediaValida = 0
let notasObtidas = 0
for (let i = 0; i < atletas.length; i++){

    nomesDosCompetidores = atletas.map(function(nomes){
        return nomes.nome
    })
    function notasObtidas() {
  atletas.map(function(notas){
        let total = notas.notas
        total.forEach(function(x, y) {
            return x - y;
        });
        return total
    })
    }

for(let i = 0; i < atletas.length; i++){
  let totalDasNotas = 0;
  atletas[i].notasComputadas = atletas[i].notas;
  atletas[i].notasComputadas = atletas[i].notasComputadas.sort(notasObtidas).slice(1, 4);
  atletas[i].notasComputadas.map(function(notas){
    totalDasNotas = totalDasNotas + notas;
});
  console.log("Atleta: " + atletas[i].nome + "\nNotas: " + atletas[i].notas + "\nMédia Válida: " + (totalDasNotas / atletas[i].notasComputadas.length));
};
}
