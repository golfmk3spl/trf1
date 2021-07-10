- Conectado VPN 10/07/2021 15h50
- Iniciado todas as instâncias de Wildfly Pje 1G ambiente Produção
- Detectado problema com ponto de montagem /var/lib/pgsql/11/data1/pg_wal no host srvbd34-trf1 que não estava montado
- Parada de todas as instâncias de Wildfly Pje 1G ambiente Produção
- Montagem do filesystem /var/lib/pgsql/11/data1/pg_wal no host srvbd34-trf1
- Movimentação dos arquivos gerados em /var/lib/pgsql/11/data1/pg_wal em diretório que não estava montado para o filesytem /dev/mapper/VG02-lv_pg_wal_1G no host srvbd34-trf1
- Iniciado todas as instâncias de Wildfly Pje 1G ambiente Produção
- Acompanhamento de logs das instâncias Wildfly 1G
- Finalização atendimento 17h28

⏎10/07/2021 15:50:23 Frame=512/2048/512 mssfix-ctrl=1250
⏎10/07/2021 15:50:23 UNUSED OPTIONS
1 [persist-tun] 
2 [persist-key] 
6 [resolv-retry] [infinite] 
9 [lport] [0] 
⏎10/07/2021 15:50:23 EVENT: RESOLVE ⏎10/07/2021 15:50:23 Contacting 201.49.158.253:1194 via UDP
⏎10/07/2021 15:50:23 WinCommandAgent: transmitting bypass route to 201.49.158.253
{
	"host" : "201.49.158.253",
	"ipv6" : false
}

⏎10/07/2021 15:50:23 EVENT: WAIT ⏎10/07/2021 15:50:23 Connecting to [rpv-trf1.trf1.jus.br]:1194 (201.49.158.253) via UDPv4
⏎10/07/2021 15:50:23 EVENT: CONNECTING ⏎10/07/2021 15:50:23 Tunnel Options:V4,dev-type tun,link-mtu 1522,tun-mtu 1500,proto UDPv4,comp-lzo,keydir 1,cipher AES-256-GCM,auth [null-digest],keysize 256,tls-auth,key-method 2,tls-client
⏎10/07/2021 15:50:23 Creds: Username/Password
⏎10/07/2021 15:50:23 Peer Info:
IV_VER=3.git::58b92569
IV_PLAT=win
IV_NCP=2
IV_TCPNL=1
IV_PROTO=2
IV_LZO_STUB=1
IV_COMP_STUB=1
IV_COMP_STUBv2=1
IV_IPv6=0
IV_GUI_VER=OCWindows_3.2.3-1851
IV_SSO=openurl

⏎10/07/2021 15:50:24 SSL Handshake: CN=server-trf1-vpn, TLSv1.3, cipher TLSv1.3 TLS_AES_256_GCM_SHA384, 2048 bit RSA
⏎10/07/2021 15:50:24 Session is ACTIVE
⏎10/07/2021 15:50:24 Sending PUSH_REQUEST to server...
⏎10/07/2021 15:50:24 EVENT: GET_CONFIG ⏎10/07/2021 15:50:24 AUTH_FAILED
⏎10/07/2021 15:50:24 EVENT: AUTH_FAILED ⏎10/07/2021 15:50:24 EVENT: DISCONNECTED ⏎10/07/2021 15:50:39 OpenVPN core 3.git::58b92569 win x86_64 64-bit built on Feb 10 2021 15:20:23
⏎10/07/2021 15:50:39 Frame=512/2048/512 mssfix-ctrl=1250
⏎10/07/2021 15:50:39 UNUSED OPTIONS
1 [persist-tun] 
2 [persist-key] 
6 [resolv-retry] [infinite] 
9 [lport] [0] 
⏎10/07/2021 15:50:39 Contacting 201.49.158.253:1194 via UDP
⏎10/07/2021 15:50:39 WinCommandAgent: transmitting bypass route to 201.49.158.253
{
	"host" : "201.49.158.253",
	"ipv6" : false
}

⏎10/07/2021 15:50:39 EVENT: RESOLVE ⏎10/07/2021 15:50:39 EVENT: WAIT ⏎10/07/2021 15:50:39 Connecting to [rpv-trf1.trf1.jus.br]:1194 (201.49.158.253) via UDPv4
⏎10/07/2021 15:50:39 EVENT: CONNECTING ⏎10/07/2021 15:50:39 Tunnel Options:V4,dev-type tun,link-mtu 1522,tun-mtu 1500,proto UDPv4,comp-lzo,keydir 1,cipher AES-256-GCM,auth [null-digest],keysize 256,tls-auth,key-method 2,tls-client
⏎10/07/2021 15:50:39 Creds: Username/Password
⏎10/07/2021 15:50:39 Peer Info:
IV_VER=3.git::58b92569
IV_PLAT=win
IV_NCP=2
IV_TCPNL=1
IV_PROTO=2
IV_LZO_STUB=1
IV_COMP_STUB=1
IV_COMP_STUBv2=1
IV_IPv6=0
IV_GUI_VER=OCWindows_3.2.3-1851
IV_SSO=openurl

⏎10/07/2021 15:50:40 SSL Handshake: CN=server-trf1-vpn, TLSv1.3, cipher TLSv1.3 TLS_AES_256_GCM_SHA384, 2048 bit RSA
⏎10/07/2021 15:50:40 Session is ACTIVE
⏎10/07/2021 15:50:40 Sending PUSH_REQUEST to server...
⏎10/07/2021 15:50:40 EVENT: GET_CONFIG ⏎10/07/2021 15:50:40 OPTIONS:
0 [route] [172.16.0.0] [255.240.0.0] 
1 [dhcp-option] [DNS] [172.16.3.1] 
2 [dhcp-option] [DNS] [172.16.3.4] 
3 [register-dns] 
4 [explicit-exit-notify] [3] 
5 [tun-mtu] [1500] 
6 [reneg-sec] [0] 
7 [route-gateway] [172.16.112.1] 
8 [topology] [subnet] 
9 [ping] [10] 
10 [ping-restart] [60] 
11 [ifconfig] [172.16.112.9] [255.255.252.0] 
12 [peer-id] [1] 
13 [cipher] [AES-256-GCM] 
14 [block-ipv6] 

⏎10/07/2021 15:50:40 PROTOCOL OPTIONS:
  cipher: AES-256-GCM
  digest: NONE
  compress: LZO_STUB
  peer ID: 1
⏎10/07/2021 15:50:40 CAPTURED OPTIONS:
Session Name: rpv-trf1.trf1.jus.br
Layer: OSI_LAYER_3
Remote Address: 201.49.158.253
Tunnel Addresses:
  172.16.112.9/22 -> 172.16.112.1
Reroute Gateway: IPv4=0 IPv6=0 flags=[ IPv4 ]
Block IPv6: yes
Add Routes:
  172.16.0.0/12
Exclude Routes:
DNS Servers:
  172.16.3.1
  172.16.3.4
Search Domains:

⏎10/07/2021 15:50:40 EVENT: ASSIGN_IP ⏎10/07/2021 15:50:41 SetupClient: transmitting tun setup list to \\.\pipe\agent_ovpnconnect
{
	"confirm_event" : "540a000000000000",
	"destroy_event" : "cc0a000000000000",
	"tun" : 
	{
		"adapter_domain_suffix" : "",
		"add_routes" : 
		[
			{
				"address" : "172.16.0.0",
				"gateway" : "",
				"ipv6" : false,
				"metric" : -1,
				"net30" : false,
				"prefix_length" : 12
			}
		],
		"block_ipv6" : true,
		"dns_servers" : 
		[
			{
				"address" : "172.16.3.1",
				"ipv6" : false
			},
			{
				"address" : "172.16.3.4",
				"ipv6" : false
			}
		],
		"layer" : 3,
		"mtu" : 0,
		"remote_address" : 
		{
			"address" : "201.49.158.253",
			"ipv6" : false
		},
		"reroute_gw" : 
		{
			"flags" : 256,
			"ipv4" : false,
			"ipv6" : false
		},
		"route_metric_default" : -1,
		"session_name" : "rpv-trf1.trf1.jus.br",
		"tunnel_address_index_ipv4" : 0,
		"tunnel_address_index_ipv6" : -1,
		"tunnel_addresses" : 
		[
			{
				"address" : "172.16.112.9",
				"gateway" : "172.16.112.1",
				"ipv6" : false,
				"metric" : -1,
				"net30" : false,
				"prefix_length" : 22
			}
		]
	},
	"wintun" : false
}
POST np://[\\.\pipe\agent_ovpnconnect]/tun-setup : 200 OK
TAP ADAPTERS:
guid='{A5037B1E-4A87-4749-9CA9-D849B8A10AB3}' index=14 name='Conexão Local'
Open TAP device "Conexão Local" PATH="\\.\Global\{A5037B1E-4A87-4749-9CA9-D849B8A10AB3}.tap" SUCCEEDED
TAP-Windows Driver Version 9.24
ActionDeleteAllRoutesOnInterface iface_index=14
netsh interface ip set interface 14 metric=1
Ok.
netsh interface ip set address 14 static 172.16.112.9 255.255.252.0 gateway=172.16.112.1 store=active
netsh interface ipv6 add route 2000::/4 interface=1 store=active
Ok.
netsh interface ipv6 add route 3000::/4 interface=1 store=active
Ok.
netsh interface ipv6 add route fc00::/7 interface=1 store=active
Ok.
IPHelper: add route 172.16.0.0/12 14 172.16.112.1 metric=-1
netsh interface ip set dnsservers 14 static 172.16.3.1 register=primary validate=no
netsh interface ip add dnsservers 14 172.16.3.4 2 validate=no
NRPT::ActionCreate names=[.] dns_servers=[172.16.3.1,172.16.3.4]
ActionWFP openvpn_app_path=C:\Program Files\OpenVPN Connect\OpenVPNConnect.exe tap_index=14 enable=1
permit IPv4 DNS requests from OpenVPN app
permit IPv6 DNS requests from OpenVPN app
block IPv4 DNS requests from other apps
block IPv6 DNS requests from other apps
allow IPv4 traffic from TAP
allow IPv6 traffic from TAP
ipconfig /flushdns
Configuração de IP do Windows
Liberação do Cache do DNS Resolver bem-sucedida.
TAP handle: 640b000000000000
⏎10/07/2021 15:50:41 Connected via TUN_WIN
⏎10/07/2021 15:50:41 LZO-ASYM init swap=0 asym=1
⏎10/07/2021 15:50:41 Comp-stub init swap=0
⏎10/07/2021 15:50:41 EVENT: CONNECTED tr301005@rpv-trf1.trf1.jus.br:1194 (201.49.158.253) via /UDPv4 on TUN_WIN/172.16.112.9/ gw=[172.16.112.1/]⏎10/07/2021 17:28:29 SetupClient: signaling tun destroy event
⏎10/07/2021 17:28:29 EVENT: DISCONNECTED ⏎