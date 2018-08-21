### Token structure
>[ Base64(HEADER) ] . [ Base64(PAYLOAD) ] . [ Base64(SIGNATURE) ]
example:
>eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiYWRtaW4iOnRydWV9.TJVA95OrM7E2cBab30RMHrHDcEfxjoYZgeFONFh7HgQ

### Token 安全性最佳实践

- 说到安全性的最佳实践，有一点我想特别强调一下，那就是在生成 `Token` 时使用用户的 `IP` 地址。这能防止另一个人在盗取你的 `Token` 后在另一个设备上使用。
- 同时请确保你使用Https，它的加密信道可以有效防止中间人攻击。
