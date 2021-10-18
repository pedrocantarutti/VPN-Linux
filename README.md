# VPN-Linux

- Servidor Linux (Ubuntu >= 20.04  / Debian >= 9)
  - OpenVPN

- IP fixo nos clients
  - alterar o arquivo server.conf e incluir a linha: client-config-dir /etc/openvpn/clients;
  - criar o arquivo com o mesmo nome do client gerado e incluir a linha: ifconfig-push IP_ESCOLHIDO e MASK;
  - resetar o serviço correto: systemctl restart openvpn-server@server.service
