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

QUESTÃO 3 => 4 PONTOS

void main() {
  Conta ob= new Conta(66,100,44);
  int MostraAgencia=ob.ContaDados(ob.Agencia1);
  print("a minha agencia é $MostraAgencia");
   int MostraConta=ob.ContaDados2(ob.Conta1);
    print("a minha agencia é $MostraConta");
  ob.SaldoConta();
  ob.Deposito(1000);
  ob.Transferencia(122222000000);
  ob.Saque(200);
 

  
 
}

class Conta{
   int Agencia1;
  double Saldo1;
  int Conta1;
  Conta(int A1, double S1, int C1){
    this.Agencia1=A1;
     this.Saldo1=S1;
    this.Conta1=C1;
  }
  int ContaDados(int a)=>a;
 int ContaDados2(int e){
   return e;
 }
 void SaldoConta(){
   print("saldo atual é ${this.Saldo1}");
 }
  
  void Deposito(double d){
    this.Saldo1=this.Saldo1+d;
    SaldoConta();
    
  }
  
  void Transferencia( double b){
    if(this.Saldo1<b){
      print("saldo insuficiente para a transferencia");
    }
    else{
    this.Saldo1=this.Saldo1-b;
    SaldoConta();
    }
  }
  
  void Saque(double y){
     if(this.Saldo1<y){
      print("saldo insuficiente para o saque");
    }
    else{
    this.Saldo1=this.Saldo1-y;
    SaldoConta();
    }
     
 }
  
  
}

