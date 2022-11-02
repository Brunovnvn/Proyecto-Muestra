# Proyecto-Muestra

Dron terreste de 2 ruedas motorizadas +  1 rueda con libre sentido
Controlado por modulo BLE (Blootooth Low Energy) que a su vez esta conectado a microcontrolador (Raspberry Pi-Pico)
Conectado a aplicación movil (MIT App Inventor)
Control de ambos motores por medio de un rele (DPDT - MR62-N3 (Bobina 5V) )
Codigo de programa creado en Visual Studio
Desarrollo del circuito en software KiCad

Permite el control de:
  - Luces
  - Bocina
  - Direccion de dron
  - Velocidad de dron
  - Sensor instalado (HC-SR04) 
  - Conexion y desconexion de modulo BLE

INFORMACIÓN DE MICROCONTROLADOR:
  
  Alimentación por USB (5V)
  Microcontrolador trabaja en 3,3V. Esta regulado por la misma.
  
  Pines BLE (UART0):
    - 1 (UART0 TX) y 2 (UART0 RX)
  
  Pines PWM (VELOCIDAD de ambos motores):
    - 4 (GP2) (Motor 1 / Izq) y 5 (GP3) (Motor 2 / Der)
    
  Pines PWM (DIRECCIÓN de ambos motores):
    - 9 (GP6) (Motor 1 / Izq) y 10 (GP7) (Motor 2 / Der)
      
  Pines control de luces:
    - 12 (GP9) y 14 (GP10)
  
  Pin bocina:
    - 15 (GP11)

  Pines control de sensor:
    - 16 (GP12) y 17 (GP13)
    
    
Alimentación de placa:

  - 5V 
  - Cables naranja / albinaranja (Positivo +)
  - Cables azul / marrón (Negativo -)

Posicionamiento dentro de la placa: 

  - Pi-Pico Pin entre: (18;C) y (25;V)
  - Transistor (1) BC337 entre: (06;O / 08;O) - Transistor (2) BC337 entre: (28;O / 30;O)
  - Transistor IRF530N (1) entre: (04;A2 / 06;A2) - Transistor IRF530N (2) entre: (31;A2 / 33;A2) 
  - Relé MR62-N3 (1) entre: (03;Q / 06;X) - Relé MR62-N3 (2) entre: (30;Q / 33;X) 
  - Resistencia 22 Ohms (1) entre: (06;B2 / 06;D2) - Resistencia 22 Ohms (2) entre: (32;B2 / 32;D2) 
  - Resistencia 2K Ohms (1) entre: (07;L / 07;N) - Resistencia 2K Ohms (2) entre: (29;K / 29;N) 
  - Resistencia 10K Ohms (1) entre: (07;D2 / 010;X) - Resistencia 10K Ohms (2) entre: (29;D2 / 32;D2) 
  - Resistencia 100K Ohms (1) entre: (04;N / 06;N) - Resistencia 100K Ohms (2) entre: (30;N / 32;N) 
  - Optoacoplador PC817 (1) entre: (05;E2 / 06;H2) - Optoacoplador PC817 (2) entre: (32;E2 / 33;H2) 
  - Diodo 1N4007 (1) entre: (03;P / 06;P) - Diodo 1N4007 (2) entre: (30;P / 33;P) 


Componentes usados: 
  - (2x) Transistor (Bipolar) BC337
  - (2x) Transistor (Mosphet) (IRF530N)
  - (2x) Relé (DPDT - MR62-N3 (Bobina 5V) )
  - (2x) Resistencia 22 Ohms
  - (2x) Resistencia 2K Ohms
  - (2x) Resistencia 10K Ohms
  - (2x) Resistencia 100K Ohms
  - (2x) Optoacoplador (PC817) 
  - (2x) Diodo (1N4007) 
  - Cables (Varios)
  

Precauciones: !!!!!!!
  - Autoiuducción de relé / Solución: Diodo
  - En cada cambio de direccion, 
  apagar PWM por unos milisegundos 
  para no producir un arco  
