# Atividade

## Roteador Rambo

### Redes Desconhecidas
- 192.168.220.0/24

### Redes Conhecidas
- 192.168.210.0/24
- 200.128.10.0/24

### Comandos
- Router>enable
- Router#configure terminal
- Router(config)#hostname Rambo
- Rambo(config)#interface g0/0/0
- Rambo(config-if)#ip address 192.168.210.1 255.255.255.0
- Rambo(config-if)#no shutdown
- Rambo(config-if)#interface g0/0/1
- Rambo(config-if)#ip address 200.128.10.1 255.255.255.0
- Rambo(config-if)#no shutdown
- Rambo(config-if)#exit
- Rambo(config)#ip route 192.168.220.0 255.255.255.0 200.128.10.2



## Roteador Rock

### Redes Desconhecidas
- 192.168.210.0/24

### Redes Conhecidas
- 192.168.220.0/24
- 200.128.10.0/24

### Comandos
- Router>enable
- Router#configure terminal
- Router(config)#hostname Rock
- Rock(config)#interface g0/0/0
- Rock(config-if)#ip address 192.168.220.1 255.255.255.0
- Rock(config-if)#no shutdown
- Rock(config-if)#interface g0/0/1
- Rock(config-if)#ip address 200.128.10.2 255.255.255.0
- Rock(config-if)#no shutdown
- Rock(config-if)#exit
- Rock(config)#ip route 192.168.210.0 255.255.255.0 200.128.10.1
