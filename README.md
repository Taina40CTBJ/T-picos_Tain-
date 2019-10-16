# T-picos_Tain-
QUESTÃO 1- D

QUESTÃO 2:

a)
void main() {
  
  int a=2;
  int b=3;
  String nome='taina';
  print(a);
  print(b);
  print(nome);
 }

b)

void main() {
  ImprimeValores();
  
     }

void ImprimeValores(){
  for(int i=1; i<11;i++){
    print(i);
  }
}

c)

void main() {
  int valor=50;
  ImprimeValores(valor);
  
     }

void ImprimeValores(int a){
  for(int i=1; i<=a;i++){
    print(i);
  }
}

d)

void main() {
 int a=5;
  Soma(a);
}

void Soma(int d){
  int soma=0;
  for(int i=1; i<=5; i++){
    soma=soma+i;
  }
  print(soma);
  
}

e)

void main() {
  Pessoa p= new Pessoa('Pedro',30);
  int b=p.idade;
  print(p.nome);
  print(p.idade);
  p.Trabalhar();
  p.TempoIdade(b);
      }


class Pessoa{
  var nome;
  var idade;
  Pessoa(var n, var i){
    this.nome=n;
    this.idade=i;
  }
  
 void Trabalhar(){
   print("já cheguei do tabalho,família linda que Deus me deu");
 }
  
  void TempoIdade(int a){
    int d= a+10;
    print("a minha idade daqui a 10 anos é: $d");
    
  }
}
