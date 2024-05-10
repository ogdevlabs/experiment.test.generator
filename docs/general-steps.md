# General steps

The steps for outline at general level


## Providing only the source control URI

### Obtain the OpenAPISpec document

1. Clone repository
2. Get into the application folder
3. Review if test already exist (ls -R | grep -E '^tests?|^integration-tests?|^test-cases?|^spec?' | wc -l
)
4. Execute the application
5. Open swagger 
6. Store the OpenApiSpec document


### Running .NET Kiota from a Docker container
1. Run as container
 ```
 docker run --openapi <path URI> mcr.microsoft.com/openapi/kiota generate --language <csharp> -n <namespace-prefix>
 ```

 ### Execute the Generated client

 ```
 dotnet run
 ```