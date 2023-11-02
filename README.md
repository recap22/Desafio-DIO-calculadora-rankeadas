function NivelRankeadas(vitorias, derrotas){

	// Calcula o saldo de vitórias
	let saldoDeVitorias = vitorias - derrotas;
    
    // Determina o nível co base no saldo de vitórias
    let Nivel;
    
 switch (true) {
	
    case saldoDeVitorias < 10:
    	Nivel = "Ferro";
        break;
        
	case saldoDeVitorias >= 11 && saldoDeVitorias <= 20:
    	Nivel = "Bronze";
        break;
    
    case saldoDeVitorias >= 21 &&  saldoDeVitorias <= 50:
    	Nivel = "Prata";
        break;
        
    case saldoDeVitorias >= 51 && saldoDeVitorias <= 80:
    	Nivel = "Ouro";
        break;
    
    case saldoDeVitorias >= 81 && saldoDeVitorias <= 90:
    	Nivel = "Diamante";
        break;
    case saldoDeVitorias >= 91 && saldoDeVitorias <= 100:
    	Nivel = "Lendário";
        break;
    default:
    	Nivel = "Imortal";
  }
  
  // Retorna a mensagem de saída
  return `O Herói tem um saldo de ${saldoDeVitorias} Vitórias e está no nível de ${Nivel}!`;
}

let vitorias = 99;
let derrotas = 21;

const resultado = NivelRankeadas(vitorias, derrotas);
	console.log(resultado);# Desafio-DIO-calculadora-rankeadas
