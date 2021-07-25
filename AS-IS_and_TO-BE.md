## AS-IS e TO-BE do PSCS

### AS-IS
* Dois Transdutores de pressão PX119-1KGI;
* Dois  Termopares tipo K + max6675;
* Servo motor MG996R;
* Válvula esfera SS-45TF8; 
* Válvula Solenóide U121V5595-492210C2; 
* Bateria fornece 3.7V, que são transformados para 6V pelo Boost Regulator (U3V70F6) para alimentar a válula esfera. 
* Os 6V provenientes do Boost Regulator (U3V70F6) são diminuídos para 5V pelo Voltage Regulator (LM7805) e alimentam os termopares. 
* Voltage Regulator (U3V70X) transforma tensão de +6V para +24V, que alimenta a válvula solenoide;

### TO-BE 
* Identificar todos os códigos dos componentes presentes em cada placa;
* Definir como vai ser feito o acoplamento elétrico entre as linhas de comunicação, união dos grounds, etc;
* Detalhar melhor as especificações das placas PSCS;
* Fazer o projeto mecânico (MCAD) indicando como serão montadas as placas PSCS no sistema propulsivo;
* Discriminar linhas de dados e de potência dos fluxogramas;
* Detalhar os barramentos;
* Escolher outra bateria que gere uma tensão mais próxima de 24 V;
* Definir se usaremos outro microcontrolador exclusivo para a PSCS da propulsão;

