`openssl genrsa -des3 -out myCA.key 2048`

`openssl req -x509 -new -nodes -key myCA.key -sha256 -days 1825 -out myCA.pem`

Windows7:
`certutil –addstore -enterprise –f "Root" <pathtocertificatefile>`

`openssl genrsa -out dev.mergebot.com.key 2048`
`openssl req -new -key dev.mergebot.com.key -out dev.mergebot.com.csr`
