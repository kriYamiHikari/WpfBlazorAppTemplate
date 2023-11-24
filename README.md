# WpfBlazorAppTemplate
WPF Blazorアプリを作成するためのテンプレート

## 使用法

### プロジェクトファイル名の変更

`___PROJECTNAME___.csproj`の``___PROJECTNAME___`'をプロジェクト名に変更する

### テンプレート名の置換

エディターなどを使用して、ファイル名内に記載している`___PROJECTNAME___`をプロジェクト名に置換する。

### ターゲットの設定

csprjファイルのTargetFrameworkの設定をビルドを行うdotnet sdkのバージョンに合わせます。

```
<Project Sdk="Microsoft.NET.Sdk.Razor">

  <PropertyGroup>
    <TargetFramework>net8.0-windows</TargetFramework>
```

`net8.0-windows`もしくは、`net7.0-windows`が設定可能です。

### パッケージのインストール

プロジェクトディレクトリ内で以下のコマンドを入力して、パッケージのインストールを行います。

```
dotnet add package Microsoft.AspNetCore.Components.WebView.Wpf
```

### ビルド

```
dotnet build
```

### リリースビルド

```
dotnet publish -c Release
```

