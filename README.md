# OmniAuth::Strategies::AzureActiveDirectoryB2C

This gem is an Azure Active Directory B2C Strategy for [OmniAuth][omniauth].

# Configuration
Original repos cloned and moved as no longer being maintained

In your `Gemfile` add `'gem 'openid_connect', 'https://github.com/bayko/openid_connect.git'`

In your `Gemfile` add `gem 'omniauth-azure_active_directory_b2c', https://github.com/bayko/omniauth-azure_active_directory_b2c.git`.

# Required ENVs
```yml
AZURE_CLIENT_ID: < b2c app registration client id >
AZURE_CLIENT_SECRET: < b2c app registration secret >
AZURE_TENANT_URL: < mytenant.onmicrosoft.com >
AZURE_B2C_URL: < https://mytenant.b2clogin.com >
AZURE_B2C_CALLBACK_URL: 'https://< my rails host>/auth/azure_active_directory_b2c/callback'
AZURE_B2C_POLICY_NAME: < b2c user flow name >
AZURE_JWK_ISSUER: < https://mytenant.b2clogin.com/my tenant uuid/v2.0/ >

# https://mytenant.b2clogin.com/mytenant.onmicrosoft.com/<my user flow name>/discovery/v2.0/keys
AZURE_JWK_KID: '...'
AZURE_JWK_N: '...'
AZURE_JWK_E: '...'
AZURE_JWK_KTY: '...'
```
