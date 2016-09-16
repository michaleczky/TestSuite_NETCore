# TestSuite_NETCore
Test Suite in .NET Core. Features:
- Google OAuth 2 integration

# Prerequisites and installation (OS X)

1. [.NET Core runtime](https://www.microsoft.com/net/core#macos)

2. Run `dotnet restore` to install project dependencies.

3. Create database and run migrations with `dotnet ef database update`

4. Setup Google OAuth2 client's id and secret by the following commands:
    ```
    dotnet user-secrets set AppSettings:GoogleClientId <clientId>
    dotnet user-secrets set AppSettings:GoogleClientSecret <clientSecret>
    ```
5. (Visual Studio Code) Add the following lines to `.vscode/launch.json` in *configurations* section in order to start the app in 
Development mode instead of Production. 
    ```
            "env": {
                "ASPNETCORE_ENVIRONMENT": "development"
            }
    ```

# Run the app

1. Start the app with `dotnet run environment=development`.
2. Open the `http://localhost:5000` in browser.

# Troublshooting

## Google OAuth2 authentication

### Arriving to a blank page after succesfull login

Try to empty the browser cache or open the app in a private browser window (to avoid previous sessions remain cached in the browser). 

