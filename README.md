# Nokia Alcatel + PPPoE Discovery Script

### Contents:
- Nokia Alcatel General
- Nokia PPPoE discovery + Script
- Nokia BGP

### Using: 

1. Put the `./src/externalscripts/nokia-pppoe.py` script in the `/opt/zabbix/externalscripts` directory
2. Import both templates: `Alcatel Timetra TiMOS SNMP` and `Nokia Alcatel SNMPv2 - BGP`

### Hint:
You can also edit the name of the interfaces when zabbix create the itens:

1. Go to: Alcatel Timetra TiMOS SNMP
2. Itens > `Retorno Json - PPPoE`
3. Create a processing:
4. Replace: `{#IF_NAME}` with: `{#IF_NAME}(XPTO)`

Example: `lag-1:120` to `lag-1:120(CIRCUITO-BNG-SAO_PAULO)`

### Tested on:

- zabbix 5.4
- grafana 9.4
