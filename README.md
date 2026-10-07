# Kingdom Modpack

Distribuição pública do modpack oficial da Kingdom para Minecraft 1.21.4 com Fabric.

## Publicação

1. Coloque apenas mods cuja licença permita redistribuição dentro da pasta preparada localmente.
2. Gere os tamanhos e hashes com o script do repositório privado `kingdom-launcher`.
3. Preencha `manifest.template.json` com o servidor, Java 21 e arquivos reais.
4. Renomeie a cópia final para `manifest.json` e anexe todos os arquivos a uma GitHub Release.
5. Use uma tag como `modpack-v1.0.0`.

## Pacotes de recursos do servidor

As fontes de itens, mobs e sons continuam separadas durante a montagem. A
publicação final contém somente dois pacotes consolidados:

- `Kingdom-Lite.zip`: texturas 3D reduzidas e sem músicas;
- `Kingdom-Full.zip`: pacote integral gerado pelo ItemsAdder.

O servidor lê `packs-manifest.json`, enquanto o launcher continua lendo
`manifest.json`. Os dois manifestos devem ser anexados à mesma release para que
a publicação de uma textura nunca interrompa as atualizações do launcher.

O launcher consulta:

```text
https://github.com/DouglasPerrone/kingdom-modpack/releases/latest/download/manifest.json
```

Não publique senhas, tokens, chaves privadas ou mods sem autorização de redistribuição.
