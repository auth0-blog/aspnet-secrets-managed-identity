This repository contains a basic ASP.NET Web API application to demonstrate how to use Azure Key Vault and Azure Managed Identities.

The following article describes the implementation details: [Secrets Access with Managed Identities in .NET Applications](https://auth0.com/blog/secrets-access-managed-identities-dotnet/)

## To run this application locally

1. Clone the repo with the following command:

   ```bash
   git clone https://github.com/auth0-blog/aspnet-secrets-managed-identity
   ```

2. Move to the `aspnet-secrets-managed-identity` folder.

3. Open the `appsettings.json` file.

4. Update `VaultUri` to match the name of your Key Vault instance in the [Azure portal](https://portal.azure.com/).

5. Initialize the Secret Manager by running the following command:

   ```bash
   dotnet user-secrets init
   ```

6. Add a sample secret value by running the following command:

   ```bash
   dotnet user-secrets set "APP-SECRET" "Local value of the secret"
   ```

7. Run the application using Visual Studio or by running the command `dotnet run`.

