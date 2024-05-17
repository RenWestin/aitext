# Cisco IOS Modes and Commands

## 1. User EXEC Mode
- **Description**: This is the default mode after you log into a Cisco switch. It provides limited access to basic monitoring commands.
- **Command to Enter**: N/A (default mode)
- **Prompt Example**: `Switch>`
- **Command to Exit**: `logout` or `exit`
- **Exit to Mode**: N/A

## 2. Privileged EXEC Mode
- **Description**: Provides access to all commands and features. You can view configurations, manage files, and enter Global Configuration Mode.
- **Command to Enter**: `enable`
- **Prompt Example**: `Switch#`
- **Command to Exit**: `disable` or `exit`
- **Exit to Mode**: User EXEC Mode

## 3. Global Configuration Mode
- **Description**: Used for making configuration changes to the device. You can configure system-wide settings here.
- **Command to Enter**: `configure terminal`
- **Prompt Example**: `Switch(config)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Privileged EXEC Mode

## 4. Interface Configuration Mode
- **Description**: Used to configure specific network interfaces on the device.
- **Command to Enter**: `interface {interface-id}`
- **Prompt Example**: `Switch(config-if)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 5. VLAN Configuration Mode
- **Description**: Used for configuring VLAN settings on the switch.
- **Command to Enter**: `vlan database`
- **Prompt Example**: `Switch(vlan)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Privileged EXEC Mode

## 6. Line Configuration Mode
- **Description**: Used to configure console, AUX, and VTY (telnet/SSH) lines.
- **Command to Enter**: `line {line-type} {line-number}`
- **Prompt Example**: `Switch(config-line)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 7. Router Configuration Mode
- **Description**: Used for configuring routing protocols.
- **Command to Enter**: `router {protocol}`
- **Prompt Example**: `Switch(config-router)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 8. Sub-Interface Configuration Mode
- **Description**: Used to configure sub-interfaces for VLANs or other purposes.
- **Command to Enter**: `interface {interface-id.subinterface}`
- **Prompt Example**: `Switch(config-subif)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 9. Access List Configuration Mode
- **Description**: Used for creating and modifying access control lists (ACLs).
- **Command to Enter**: `ip access-list {standard | extended} {name}`
- **Prompt Example**: `Switch(config-acl-std)#` or `Switch(config-acl-ext)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 10. Control Plane Configuration Mode
- **Description**: Used to configure control plane policing and other related settings.
- **Command to Enter**: `control-plane`
- **Prompt Example**: `Switch(config-cp)#`
- **Command to Exit**: `exit`
- **Exit to Mode**: Global Configuration Mode

## 11. Script Configuration Mode
- **Description**: Used to enter Tcl scripting mode for advanced scripting tasks.
- **Command to Enter**: `tclsh`
- **Prompt Example**: `Switch(tcl)#`
- **Command to Exit**: `tclquit` or `exit`
- **Exit to Mode**: Privileged EXEC Mode
