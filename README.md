proxies:
- name: IKD WS
  type: trojan
  server: 104.18.2.2
  port: 443
  password: db7fdbf6-ab76-420c-95c4-0b62ebd6c55a
  udp: true
  sni: id7.natanvpn.xyz
  skip-cert-verify: true
  network: ws
  ws-opts:
    path: /trojan
    headers: 
      host: id7.natanvpn.xyz
- name: IKD GRPC 
  type: trojan
  server: 104.18.2.2
  port: 443
  password: db7fdbf6-ab76-420c-95c4-0b62ebd6c55a
  udp: true
  sni: id7.natanvpn.xyz
  skip-cert-verify: true
  network: grpc
  grpc-opts:
      grpc-service-name: trojan
