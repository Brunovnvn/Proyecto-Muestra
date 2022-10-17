# Proyecto-Muestra

Dron terreste de 2 ruedas motorizadas +  1 rueda con libre sentido
Controlado por modulo BLE (Blootooth Low Energy)
Conectado a aplicación movil (MIT App Inventor)
Controlado por microcontrolador (Raspberry Pi-Pico)
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

Información de microcontrolador:
  Pines PWM (Motor izquierdo (1) ):
    - 4 y 5
  Pines PWM (Motor derecho (2) ):
    - 9 y 10
  Pines UART0 (BLE):
    - 1 y 2
  Pines control de luces:
    - 
  Pines sensor:
    - 
  Pines bocina:
    - 
  
  
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
      
