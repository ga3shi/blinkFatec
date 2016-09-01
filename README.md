# blinkFatec
//Define as variáveis
int led[] = {1,2,3,4,5,6};
int pinoAtual = 0;
int pinos = 6;
int a=0, b=0,c=0,d=0,e=0;

void setup() {
  //Define os leds como saída
  for(pinoAtual;pinoAtual<pinos;pinoAtual++){
    pinMode(led[pinoAtual], OUTPUT);  
  }
}

void loop() {
// Chama todas as letras e respectivas transições
 for(a;a<=100;a++){
  invocaF();

 }  
 f1();
 for(b;b<=100;b++){
  invocaA();
 }
 f2();
 for(c;c<=100;c++){
  invocaT();
 }
 f3();
 for(d;d<=100;d++){
  invocaE();  
 }
 f4();
 for(e;e<=100;e++){
  invocaC();
 }
 f2();

// Reinicia as variáveis
 a=0;
 b=0;
 c=0;
 d=0;
 e=0;
}

// Funções de 1 a 9 tem a tarefa de acender o respectivo pino
void pino1(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}


void pino2(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}


void pino3(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}


void pino4(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}

void pino5(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}

void pino6(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
  }
}

void pino7(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
  }
}

void pino8(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
  }
}

void pino9(){
  for(pinoAtual = 0;pinoAtual<1;pinoAtual++){
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], LOW);pinoAtual++;
    digitalWrite(led[pinoAtual], HIGH);pinoAtual++;
  }
}

void invoca12345(){
  pino1();delay(5);
  pino2();delay(5);
  pino3();delay(5);
  pino4();delay(5);
  pino5();delay(5);
}

void invoca789(){
  pino7();delay(5);
  pino8();delay(5);
  pino9();delay(5);
}

void invocaF(){
  invoca12345();delay(5);
  pino7();delay(5);
}

void invocaA(){
  invoca12345();delay(5);
  pino6();delay(5);
  pino7();delay(5);
  pino9();delay(5);
}

void invocaT(){
  pino1();delay(5);
  pino2();delay(5);
  pino3();delay(5);
  pino5();delay(5);
  pino8();delay(5);
}

void invocaE(){
  invoca12345();delay(5);
  invoca789();delay(5);
}

void invocaC(){
  pino1();delay(5);
  pino2();delay(5);
  pino3();delay(5);
  pino4();delay(5);
  invoca789();delay(5);
}

void f1(){
  pino1();delay(500);
  pino2();delay(500);
  pino3();delay(500);
  pino6();delay(500);
  pino9();delay(500);
  pino8();delay(500);
  pino7();delay(500);
  pino4();delay(500);
  pino5();delay(500);
}

void f2(){
  pino1();delay(500);
  pino4();delay(500);
  pino7();delay(500);
  pino2();delay(500);
  pino5();delay(500);
  pino8();delay(500);
  pino3();delay(500);
  pino6();delay(500);
  pino9();delay(500);
}

void f3(){
  pino7();delay(500);
  pino5();delay(500);
  pino3();delay(500);
  pino1();delay(500);
  pino5();delay(500);
  pino9();delay(500);
}

void f4(){
  invoca789();delay(500);
  pino6();delay(500);
  pino5();delay(500);
  pino4();delay(500);
  pino1();delay(500);
  pino2();delay(500);
  pino3();delay(500);
}
