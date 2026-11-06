# Controle Samsung Android

Projeto Android nativo em Java, sem necessidade de Android Studio. Para compilar: envie **o conteúdo desta pasta** para um repositório GitHub. Na aba Actions, execute "Gerar APK Samsung". Baixe o artifact SamsungControle-APK ao concluir e extraia o APK.

## Recursos
- Descoberta SSDP de dispositivos Samsung/MediaRenderer na mesma rede Wi-Fi (pode mostrar outros dispositivos ou não encontrar a TV).
- Conexão Samsung Tizen WebSocket segura porta 8002 com autorização na TV.
- Controle remoto: volume, canal, navegação, Home, Return, Source, Menu e Power (ligar com TV desligada pode exigir Wake-on-LAN, não implementado).
- IP manual como alternativa e lembrança do último IP.

## Observações
A conexão usa exceção de validação de certificado TLS **somente para o IP informado da TV**, porque alguns aparelhos Samsung apresentam certificado autoassinado. Utilize apenas em redes Wi-Fi confiáveis. A busca pode falhar se o roteador isolar clientes, o multicast estiver bloqueado ou a TV não anunciar SSDP. O APK não foi testado em aparelho real. O Android pode alertar sobre instalação de APK externo. Não é um aplicativo oficial Samsung.
