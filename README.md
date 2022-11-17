# Proyecto-Muestra

DIA DE FERIA DE CIENCIAS (MUESTRA ESCOLAR):
  Viernes 18 de Noviembre del 2022 / 18.11.2022

Dron terreste de 2 ruedas motorizadas +  1 rueda con libre sentido
Controlado por modulo BLE (Blootooth Low Energy) que a su vez esta conectado a microcontrolador (Raspberry Pi-Pico)
Conectado a aplicación movil (MIT App Inventor)
  En la cual se encuentra la interfaz con los controles para el dron
Control del dron por pines PWM de Raspberry Pi-Pico
Codigo de programa creado en Visual Studio
Desarrollo del circuito en software KiCad

Permite el control de:
  - Direccion de dron
  - Velocidad de dron
  - Luces
  - Bocina
  - Conexion y desconexion de modulo BLE


Componentes usados: 
  - Zocalo para adaptación de Raspberry Pi-Pico
  - (3x) Transistor (Bipolar) BC337
  - (2x) Transistor (Mosphet) (IRF530N)
  - (2x) Relé (DPDT - MR62-N3 (Bobina 5V) )
  - (2x) Optoacoplador (PC817) 
  - (3x) Diodo (1N4007) 
  - Resistencias (Varias)
  - Cables (Varios)
  - Madera (Chasis de dron)

INFORMACIÓN DE MICROCONTROLADOR:
  
  Alimentación por USB (5V)
  Microcontrolador trabaja en 3,3V. Esta regulado por la misma.
  
  Pines BLE (UART0):
    - 1 (UART0 TX) y 2 (UART0 RX)
  
  Pines PWM (VELOCIDAD de ambos motores):
    - 21 (GP16) (Motor 1 / Izq) y 16 (GP12) (Motor 2 / Der)
    
  Pines PWM (DIRECCIÓN de ambos motores):
    - 9 (GP6) (Motor 1 / Izq) y 10 (GP7) (Motor 2 / Der)
      
  Pines control de luces:
    - 11 (GP8)
    - 12 (GP9) 
    - 14 (GP10)
    - 15 (GP11)
    
  Pin bocina:
    - 20 (GP15)
    
    
Alimentación de placa (Raspberry Pi-Pico):

  - 5V (VSYS) (pin 39) (Positivo +)
  - GND (pin 38) (Negativo -)
  

Posicionamiento dentro de la placa: 

  - Raspberry Pi-Pico entre: (17;C) y (26;V)
  - Modulo BLE entre: ( ; ) y (  ; )
  - Buzzer entre: (23;B2) y (23;E2)
  - Transistor (1) BC337 entre: (06;O / 08;O) - Transistor (2) BC337 entre: (28;O / 30;O) Transistor (3) BC337 entre: (19;C2 / 19;E2) 
  - Transistor IRF530N (1) entre: (04;A2 / 06;A2) - Transistor IRF530N (2) entre: (31;A2 / 33;A2) 
  - Relé MR62-N3 (1) entre: (03;Q / 06;X) - Relé MR62-N3 (2) entre: (30;Q / 33;X) 
  - Resistencia 22 Ohms (1) entre: (06;B2 / 06;D2) - Resistencia 22 Ohms (2) entre: (32;B2 / 32;D2) 
  - Resistencia 2K Ohms (1) entre: (07;L / 07;N) - Resistencia 2K Ohms (2) entre: (29;K / 29;N) 
Resistencia 2K Ohms (3) entre: (18;W / 18;Z) 
  - Resistencia 10K Ohms (1) entre: (07;D2 / 010;X) - Resistencia 10K Ohms (2) entre: (29;D2 / 32;D2) 
  - Resistencia 100K Ohms (1) entre: (04;N / 06;N) - Resistencia 100K Ohms (2) entre: (30;N / 32;N) - Resistencia 100K Ohms (3) entre: (15;Z / 17;Z) 
  - Optoacoplador PC817 (1) entre: (05;E2 / 06;H2) - Optoacoplador PC817 (2) entre: (32;E2 / 33;H2) 
  - Diodo 1N4007 (1) entre: (03;P / 06;P) - Diodo 1N4007 (2) entre: (30;P / 33;P) 
 Diodo 1N4007 (3) entre: (19;A2 / 23;A2) 
