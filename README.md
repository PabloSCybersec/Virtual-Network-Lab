# 🌐 Virtual Network Lab

Un laboratorio de red virtual interactivo construido con HTML, CSS y JavaScript puro — sin dependencias externas.

![Preview](https://img.shields.io/badge/status-activo-brightgreen) ![HTML](https://img.shields.io/badge/HTML-5-orange) ![CSS](https://img.shields.io/badge/CSS-3-blue) ![JS](https://img.shields.io/badge/JavaScript-ES6-yellow)

## 🚀 Demo en vivo

> [Ver demo →](https://TU-USUARIO.github.io/virtual-network-lab/)

## ¿Qué es esto?

Un proyecto de portafolio para practicar y demostrar conocimientos de redes. Visualiza una topología de red con dispositivos reales, subnets separadas y enlace entre ellas.

## Funcionalidades

- **Topología visual interactiva** — 3 subnets, 1 router, 3 switches, 2 servidores, 3 hosts
- **Inspector de dispositivos** — haz click en cualquier nodo para ver IP, MAC, gateway, puertos y servicios
- **Calculadora de subnets** — ingresa cualquier CIDR y obtén máscara, broadcast, wildcard y rango de hosts
- **Simulador de Ping** — simula ICMP entre dos hosts con animación del paquete recorriendo la red
- **Log de actividad** — registro en tiempo real de cada acción
- **Modo oscuro** — detecta automáticamente la preferencia del sistema

## Topología de red

```
                  [Router 10.0.0.1]
                 /        |        \
          [SW-A]       [SW-B]    [SW-C]
          /    \          |       /   \
    [Web]     [DB]    [Host-1] [Host-2] [Host-3]
  10.0.1.10 10.0.1.20 10.0.2.10 10.0.3.10 10.0.3.20
```

| Subnet         | Dispositivos            | Propósito        |
|----------------|-------------------------|------------------|
| 10.0.1.0/24    | Web Server, DB Server   | Servidores       |
| 10.0.2.0/24    | Host-1                  | Red de usuarios  |
| 10.0.3.0/24    | Host-2, Host-3          | Red de usuarios  |

## Cómo usar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/TU-USUARIO/virtual-network-lab.git
   cd virtual-network-lab
   ```
2. Abre `index.html` en tu navegador — no necesita servidor.

## Conceptos que practica este proyecto

- Subnetting y CIDR notation
- Subnet masks, wildcard masks y broadcast address
- Routing entre subnets (L3)
- Switching dentro de una subnet (L2)
- Default gateway y salto entre redes
- Direcciones MAC e IP
- Simulación de ICMP (ping) y TTL

## Próximas mejoras

- [ ] Firewall / ACL entre subnets
- [ ] Servidor DHCP simulado
- [ ] VLANs
- [ ] NAT (Network Address Translation)
- [ ] Agregar/eliminar dispositivos desde la UI
- [ ] Exportar topología como JSON

## Tecnologías

- HTML5 Canvas para el render de la red
- CSS custom properties para modo oscuro automático
- JavaScript vanilla (sin frameworks ni librerías)

---

*Proyecto personal para practicar redes mientras aprendo desarrollo web.*
