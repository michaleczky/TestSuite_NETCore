# TestSuite_NETCore
Test Suite in .NET Core. Features:
- Google OAuth 2 integration

# Prerequisites and installation (OS X)

1. [.NET Core runtime](https://www.microsoft.com/net/core#macos)
2. Run `dotnet restore` to install project dependencies.
3. Create database and run migrations with `dotnet ef database update` 

# Run the app

1. Start the app with `dotnet run`.
2. Open the `http://localhost:5000` in browser.

# Troublshooting

## Google OAuth2 authentication

### Arriving to a blank page after succesfull login

Try to empty the browser cache or open the app in a private browser window (to avoid previous sessions remain cached in the browser). 

