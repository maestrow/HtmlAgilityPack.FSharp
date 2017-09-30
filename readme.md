F# wrapper for [HtmlAgilityPack](http://html-agility-pack.net/) and [HtmlAgilityPack.CssSelectors.NetCore](https://github.com/trenoncourt/HtmlAgilityPack.CssSelectors.NetCore). Originally posted by Gustavo Guerra at http://www.fssnip.net/kr/title/HtmlAgilityPackFSharp.

## Build

- [Bootstrap Paket](https://gist.github.com/maestrow/94d99017380adbcadff29f048f423729#file-paket-bootstrap-md)
- `dotnet restore`
- `dotnet build`

## Using in *.fsx

- Add in `paket.dependencies`:
```
nuget HtmlAgilityPack.CssSelectors.NetCore
github maestrow/HtmlAgilityPack.FSharp HtmlAgilityPack.FSharp.fs
```
- `paket install`
- `paket generate-load-scripts --framework netstandard2.0`

Then in your script: 
```
#load ".paket/load/netstandard2.0/HtmlAgilityPack.CssSelectors.NetCore.fsx"
#load "paket-files/maestrow/HtmlAgilityPack.FSharp/HtmlAgilityPack.FSharp.fs"

```