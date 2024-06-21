# STARTUP ODONTO
Repositório para o projeto Odonto da Startup
Para rodar o aplicativo em sua máquina, execute os seguintes passos:
## BACKEND
1. Acesse o submódulo BackEnd-Startup
2. Clique no botão "Code"/"Código" (verde) e siga essas opções:
  2.1 Para ter o arquivo em .zip é necessário apenas fazer o download da pasta e extraí-los em um local de sua preferência.
  2.2 Já para ter o projeto e também ter as atualizações futuras, basta clonar, com o comando git clone no terminal e o link do repositório: https://github.com/carlalopesj/BackEnd-Startup.git
3. Após clonar o BackEnd ou ter os arquivos em maõs, abra o VsCode e no terminal dê um "npm install" (caso não tenha as dependências instaladas), caso já tenha, dê apenas "npm run dev". (Pode ser, ao rodar o npm run dev, apareça algo relacionando ao nodemon, para resolver é só digitar "npm install nodemon".
4. Se no terminal aparecer que a conexão foi estabelecida com sucesso, o backend já está funcionando.
5. Para testar, abra o link oferecido (localhost:3535) na web e adicione o endpoint media (localhost:3535/media) e irá aparecer alguns dados já adicionados no banco.

## FRONTEND
1. Acesse o submódulo FrontEnd-Startup
2. Clique no botão "Code"/"Código" (verde) e siga essas opções:
  2.1 Para ter o arquivo em .zip é necessário apenas fazer o download da pasta e extraí-los em um local de sua preferência
  2.2 Já para ter o projeto e também ter as atualizações futuras, basta clonar, com o comando git clone no terminal e o link do repositório: https://github.com/carlalopesj/FrontEnd-Startup.git
3. Após clonar o FrontEnd ou ter os arquivos em mãos, abra o VsCode e no terminal dê um "npm install"
4. Ao terminar a instalação, escreva o comando "npx expo start", e será gerado uma build, que você pode acessar via web localhost, usando emuladores, ou se preferir acessando o qrCode pelo seu próprio celular

### Integrando o FrontEnd com o Backend
Para integrar os dois, é necessário alterar o IP, de acordo com a sua rede nas seguintes pastas:

1x - src/app/index/index.tsx

1x - src/app/cadastro/index.tsx

2x - src/app/dentes/index.tsx

A parte que deve ser alterada está comentada ao lado, você deve alterar 4 vezes. Para verificar o seu ip, digite "ipconfig" no terminal e veja os números correspondentes ao IPv4.
Altere apenas a parte do ip, mantendo a porta 3535.

Obs: para que o FrontEnd funcione com o BackEnd é necessário que os dois estejam rodando ao mesmo tempo com os comandos de "npm run dev" no backend e "npx expo start" no frontend
