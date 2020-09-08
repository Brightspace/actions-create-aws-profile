# Create Aws Profile

Github action that creates an aws profile using the session token in the environment variables.

## Usage

Simple usage
```yaml
steps
  - uses: Brightspace/actions-create-aws-profile@master
    with:
      profile-name: 'Profile Name to Create'
```

Custom Environment Variables
```yaml
steps
  - uses: Brightspace/actions-create-aws-profile@master
    with:
      profile-name: 'Profile Name to Create'
      access-key-id-var: ACCESS_KEY_ENV_VAR
      secret-access-key-var: SECRET_ACCESS_KEY_ENV_VAR
      session-token-var: SESSION_TOKEN_ENV_VAR
```

