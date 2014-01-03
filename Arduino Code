int data = 2;  //2
int latch = 3; //3
int clock = 4; //4

int i = 100;

void setup()
{
  pinMode(data, OUTPUT);    
  pinMode(latch, OUTPUT);
  pinMode(clock, OUTPUT);  
}

void loop() 
{ 
  //binary();

  for(int a = 0; a<=500; a++){
    i = 0;
    allOn();
  }

  hello_shane();

  i = 75;
  allSnake();

  for(int a = 0; a <= 1; a++){
    i = 100;
    oneBar();
  }

  for(int a = 0; a <= 4; a++){
    i = 100;
    spaceBars();
  }

  for(int a = 0; a <= 4; a++){
    i = 75;
    bars();
  }
}

void shift(int cathodes, int display1, int display2, int display3)
{
  digitalWrite(latch, LOW);
  shiftOut(data, clock, MSBFIRST, cathodes);
  shiftOut(data, clock, MSBFIRST, display1);
  shiftOut(data, clock, MSBFIRST, display2);
  shiftOut(data, clock, MSBFIRST, display3);
  digitalWrite(latch, HIGH);                   
  delay(i);
}

void hello_shane()
{
  for(int a  = 0; a <= 150; a++){
    shift(0,1,0,0);
    shift(27,2,0,0);
    shift(0,4,0,0);

    shift(0,16,0,0);
    shift(10,32,0,0);
    shift(10,64,0,0);

    shift(0,0,2,0);
    shift(30,0,4,0);
    shift(30,0,8,0);

    shift(0,0,32,0);
    shift(30,0,64,0);
    shift(30,0,0,1);

    shift(0,0,0,4);
    shift(14,0,0,8);
    shift(0,0,0,16);
  }
  for(int a = 0; a <= 150; a++){
    shift(2,1,0,0);
    shift(10,2,0,0);
    shift(8,4,0,0);

    shift(0,16,0,0);
    shift(27,32,0,0);
    shift(0,64,0,0);

    shift(0,0,2,0);
    shift(11,0,4,0);
    shift(0,0,8,0);

    shift(0,0,32,0);
    shift(23,0,64,0);
    shift(27,0,0,1);
    shift(0,0,0,2);

    shift(0,0,0,8);
    shift(10,0,0,16);
    shift(10,0,0,32);
  }
}

/*
void tammy()
 {
 for(int a = 0; a <= 200; a++){
 shift(15,1,0,0);
 shift(0,2,0,0);
 shift(15,4,0,0);
 
 shift(0,16,0,0);
 shift(11,32,0,0);
 shift(0,64,0,0);
 
 shift(0,0,2,0);
 shift(23,0,4,0);
 shift(0,0,8,0);
 
 shift(0,0,32,0);
 shift(23,0,64,0);
 shift(0,0,0,1);
 
 shift(3,0,0,4);
 shift(24,0,0,8);
 shift(3,0,0,16);
 }
 }
 */


void allOn()
{
  shift(0,127,0,0);
  shift(0,0,127,0);
  shift(0,0,0,127);
}

void oneBar()
{
  shift(0,1,0,0);
  shift(0,2,0,0);
  shift(0,4,0,0);
  shift(0,8,0,0);
  shift(0,16,0,0);
  shift(0,32,0,0);
  shift(0,64,0,0);

  shift(0,0,1,0);
  shift(0,0,2,0);
  shift(0,0,4,0);
  shift(0,0,8,0);
  shift(0,0,16,0);
  shift(0,0,32,0);
  shift(0,0,64,0);

  shift(0,0,0,1);
  shift(0,0,0,2);
  shift(0,0,0,4);
  shift(0,0,0,8);
  shift(0,0,0,16);
  shift(0,0,0,32);
  shift(0,0,0,64);
}

void bars()
{
  shift(0,85,42,85);
  shift(0,42,85,42);
}

void spaceBars()
{
  shift(0,17,34,68);
  shift(0,34,68,136);
  shift(0,68,136,17);
  shift(0,136,17,34);
}
void allSnake()
{
  //First Display
  shift(30,1,0,0);
  shift(29,1,0,0);
  shift(27,1,0,0);
  shift(23,1,0,0);
  shift(15,1,0,0);

  shift(15,2,0,0);
  shift(23,2,0,0);
  shift(27,2,0,0);
  shift(29,2,0,0);
  shift(30,2,0,0);

  shift(30,4,0,0);
  shift(29,4,0,0);
  shift(27,4,0,0);
  shift(23,4,0,0);
  shift(15,4,0,0);

  shift(15,8,0,0);
  shift(23,8,0,0);
  shift(27,8,0,0);
  shift(29,8,0,0);
  shift(30,8,0,0);

  shift(30,16,0,0);
  shift(29,16,0,0);
  shift(27,16,0,0);
  shift(23,16,0,0);
  shift(15,16,0,0);

  shift(15,32,0,0);
  shift(23,32,0,0);
  shift(27,32,0,0);
  shift(29,32,0,0);
  shift(30,32,0,0);

  shift(30,64,0,0);
  shift(29,64,0,0);
  shift(27,64,0,0);
  shift(23,64,0,0);
  shift(15,64,0,0);

  //Second Display
  shift(15,0,1,0);
  shift(23,0,1,0);
  shift(27,0,1,0);
  shift(29,0,1,0);
  shift(30,0,1,0);

  shift(30,0,2,0);
  shift(29,0,2,0);
  shift(27,0,2,0);
  shift(23,0,2,0);
  shift(15,0,2,0);

  shift(15,0,4,0);
  shift(23,0,4,0);
  shift(27,0,4,0);
  shift(29,0,4,0);
  shift(30,0,4,0);

  shift(30,0,8,0);
  shift(29,0,8,0);
  shift(27,0,8,0);
  shift(23,0,8,0);
  shift(15,0,8,0);

  shift(15,0,16,0);
  shift(23,0,16,0);
  shift(27,0,16,0);
  shift(29,0,16,0);
  shift(30,0,16,0);

  shift(30,0,32,0);
  shift(29,0,32,0);
  shift(27,0,32,0);
  shift(23,0,32,0);
  shift(15,0,32,0);

  shift(15,0,64,0);
  shift(23,0,64,0);
  shift(27,0,64,0);
  shift(29,0,64,0);
  shift(30,0,64,0);

  //Third Display
  shift(30,0,0,1);
  shift(29,0,0,1);
  shift(27,0,0,1);
  shift(23,0,0,1);
  shift(15,0,0,1);

  shift(15,0,0,2);
  shift(23,0,0,2);
  shift(27,0,0,2);
  shift(29,0,0,2);
  shift(30,0,0,2);

  shift(30,0,0,4);
  shift(29,0,0,4);
  shift(27,0,0,4);
  shift(23,0,0,4);
  shift(15,0,0,4);

  shift(15,0,0,8);
  shift(23,0,0,8);
  shift(27,0,0,8);
  shift(29,0,0,8);
  shift(30,0,0,8);

  shift(30,0,0,16);
  shift(29,0,0,16);
  shift(27,0,0,16);
  shift(23,0,0,16);
  shift(15,0,0,16);

  shift(15,0,0,32);
  shift(23,0,0,32);
  shift(27,0,0,32);
  shift(29,0,0,32);
  shift(30,0,0,32);

  shift(30,0,0,64);
  shift(29,0,0,64);
  shift(27,0,0,64);
  shift(23,0,0,64);
  shift(15,0,0,64);
}

/*
void binary()
 {
 i = 100;
 for(int w = 0; w <= 127; w++){
 for(int e = 0; e <= 127; e++){
 for(int r = 0; r <= 127; r++){
 shift(30,r,e,w); 
 }
 }
 }
 }
 */


