# Blazor inconsistency in custom elements support

```
dotnet restore
dotnet run
```

Visit [http://localhost:5059](http://localhost:5059) in a supported browser.

Customized built-in custom element is not always supported. This appears to be dependent on the rendermode. SSR renders work 100% while client-side renders (using BrowserRenderer) do not provide `createElement` with the required `is` parameter.

[aspnetcore#64213](https://github.com/dotnet/aspnetcore/issues/64213)
