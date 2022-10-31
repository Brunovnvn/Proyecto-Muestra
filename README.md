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
  - Sensor instalado
  - Conexion y desconexion de modulo BLE

INFORMACIÓN DE MICROCONTROLADOR:

  Pines PWM (VELOCIDAD de ambos motores):
    - 4 (GP2) (Motor 1 - Izq) y 5 (GP3)(Motor 2 - Der)
    
  Pines PWM (DIRECCIÓN de ambos motores):
    - 9 (GP6) (Motor 1 - Izq) y 10 (GP7) (Motor 2 - Der)
    
  Pines BLE (UART0):
    - 1 (UART0 TX) y 2 (UART0 RX)
    
  Pines control de luces:
    - 12 (GP9) y 14 (GP10)
  
  Pin bocina:
    - 15 (GP11)

  Pines control de sensor:
    - 16 (GP12) y 17 (GP13)
    
        
  
Alimentación de placa:
  - 5V
  - Cable naranja (Positivo +)
  - Cable azul (Negativo -)

Componentes usados: 
  - (2x) Transistor (Bipolar) BC337
  - (2x) Relé (DPDT - MR62-N3 (Bobina 5V) )
  - (2x) Resistencia 220 Ohms
  - (2x) Transistor (NPN) 
  
Precauciones: !!!!!!!
  - Autoiuducción de relé / Solución: Diodo
  - En cada cambio de direccion, 
  apagar PWM por unos milisegundos 
  para no producir un arco  
