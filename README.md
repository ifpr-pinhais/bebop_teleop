# bebop_teleop
Uma versão modificada do teleop básico do ROS, permite se comunicar com o tópico de velocidade do drone usado na simulação do projeto de drones de inspeção. Adiciona uma nova tecla que publica um sinal para que seja definida uma marca na posição atual do drone.

# Launch
Run.
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
# Usage
```
Reading from the keyboard  and Publishing to Twist!
---------------------------
Moving around:
   u    i    o
   j    k    l
   m    ,    .

For Holonomic mode (strafing), hold down the shift key:
---------------------------
   U    I    O
   J    K    L
   M    <    >

t : up (+z)
b : down (-z)
s: Define uma marca na posição atual do drone, publica um comando no tópico /marca

anything else : stop

q/z : increase/decrease max speeds by 10%
w/x : increase/decrease only linear speed by 10%
e/c : increase/decrease only angular speed by 10%

CTRL-C to quit
```
