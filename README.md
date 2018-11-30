# trainning-submodules

Repositório feito para praticar como fazer sub módulos e registrando o fluxo utilizado.

## Fluxo

1. Criado uma pasta chamada `lib`, pois irei usar uma lib minha e usar como sub módulo
2. Pelo terminal entrei na pasta lib e usei o comando

```
git submodule add https://github.com/viniceosm/logpty.git logpty
```

3. Na raiz do projeto irá ser criado um arquivo chamado `.gitmodules` com o código abaixo:

```
[submodule "lib/logpty"]
  path = lib/logpty
  url = https://github.com/viniceosm/logpty.git
```

4. Agora poderá commitar seu sub módulo

```

git commit -m '🆕 primeiro commit com submodulo logpty'
```

## Atualizar sub modulos

```
git submodule update --remote --recursive

# Depois é só commitar
git add lib/logpty
git commit -m '🆙 logpty atualizado'
```