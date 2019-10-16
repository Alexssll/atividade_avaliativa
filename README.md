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
