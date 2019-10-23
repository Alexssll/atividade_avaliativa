# atividade_avaliativa
/////////////////questao 01//////////////////
Alternativa "D"
//////////////////questao02-A////////////////

void main(){
  int qtd = 1;
  int preco = 5; 
  String nome_produto = "CTBJ";
  
  print("O nome do produto é: $nome_produto"); 
   
  print("A quantidade do produto é: $qtd"); 
    
  print("O preço do produto é: $preco"); 
   
}
//////////////////questao02-B////////////////

void  imprimir_numeros(){
  for (int i = 0; i < 10; i++) {
    print(' ${i + 1}');
}
}
void main(){
  imprimir_numeros();
}


//////////////////questao02-C////////////////

void imprimir_numeros(int a){

    for (int i = 0; i < a; i++) {
    print(' ${i + 1}');
}
}  
void main(){
  imprimir_numeros(50);
}

//////////////////questao02-D////////////////

void imprimir_numeros(int a){
int somat = 0;
    for (int i = 0; i < a; i++) {
      somat = somat + a;
     print ('$somat');
}
}  
void main(){
  imprimir_numeros(50);
}


//////////////////questao02-E////////////////
class Auto{          // classe
  String modelo;    //atributos
  
  void nao_esta_na_garagem (){                              //metodos com funçoes
    print('O seu caminhao $modelo nao esta na garagem.');
  }

  void esta_na_garagem (){
    print('O seu caminhao $modelo esta na garagem.');
  }
}

class Automoveis extends Auto{  //herança
 Automoveis(String modelo){    //construtor
    this.modelo = modelo;
  }  
}

void main(){
  Automoveis Caminhoes  = Automoveis ('FH460');  //objetos 
  Caminhoes.esta_na_garagem();
}
//////////////////////////////////////atividade avaliativa 4 pts/////////////////////////////////////
 class Banco {
  int numero_conta;
  String tipo_conta;
  String nome_cliente;
  double saldo_total;
  
  Banco(this.numero_conta,this.tipo_conta, this.nome_cliente, this.saldo_total);
   void criar_conta () {
     print ('Nome : $nome_cliente');
     print ('Tipo da conta: $tipo_conta');
     print ('n_conta $numero_conta');
   }
  
  void transferencia_cliente (int a, int b, double c) {
    print ('Conta $b transfere $c para a conta $b');
    saldo_total = saldo_total - c;
  }
  
  
  void saque_cliente (double valor_do_saque) {
    print ('Saque: $valor_do_saque');
    saldo_total = saldo_total - valor_do_saque;
    print('Saldo: $saldo_total');
    
  }
   
  void deposito_total (double valor) {
    print('Depósito de: $valor');
    saldo_total = saldo_total + valor;
    print('Saldo: $saldo_total');
  }
 
  double saldo_t () => this.saldo_total;
}
void main() {
 Banco s = new Banco(808080,'fisca','ALex',50000);
 s.criar_conta();
 s.deposito_total(200);
 s.saque_cliente(400);
 s.transferencia_cliente(100, 110, 500);
 double valorsaldo = s.saldo_t();
 print('Saldo atual: $valorsaldo');

}
