# BV2BDIS

BV2BIDS is a command line tool that creates the EEG-BIDS folder hierarchy from BVCD files.

## Usage

Supported projects targetting:
- .NET Core App 3.0+
- .NET Standard 2.1+

Supported language versions:
- C# 8.0+  
  Note that all projects use [Nullable Reference Types](https://docs.microsoft.com/dotnet/csharp/nullable-references).
  
## Build & Run

You should be able to build BV2BIDS for any platform supported by [.NET Core](https://dotnet.github.io/):

1. Build:
   ```
   dotnet build sln/FileFormats.sln
   ```  
   or
   ```
   dotnet build src/FileFormats/src/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI.csproj
   ```
1. Run:
   ```
   dotnet run --project src/FileFormats/src/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI.csproj
   ```
1. Publish for Windows x64:
   ```
   dotnet publish src/FileFormats/src/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI/FileFormats.BrainProducts.GenericDataFormat.BrainVisionValidatorCLI.csproj -r win-x64 -c "Release" --self-contained=true -p:PublishSingleFile=true -p:ProductId=BrainVisionToBidsConverterCLI
   ```

## Download

You may want to use a precompiled and signed version of a tool directly from Brain Products site:
