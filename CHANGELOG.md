## unreleased

## 2.5.0 - 2022-09-20

- feat: Add support for disabling the middleware on specific routes [https://github.com/clerkinc/clerk-sdk-ruby/pull/19]

## 2.4.0 - 2022-09-05

- feat: Add support for the users.disable_mfa endpoint

## 2.3.0 - 2022-08-30

- feat: Add support for the users.verify_password endpoint

## 2.2.0 - 2022-08-26

- feat: Add support for the [users.create](https://reference.clerk.dev/reference/backend-api-reference/users#create-a-user) endpoint

## 2.1.2 - 2022-08-26

- fix: Gracefully handle invalid JSON in Authorization header [https://github.com/clerkinc/clerk-sdk-ruby/pull/16]

## 2.1.1 - 2022-02-24

- fix: Make Authv2 middleware thread-safe

## 2.0.0 - 2021-10-21

This release introduces the new networkless middleware which works with the new 
authentication scheme, [Auth v2](https://docs.clerk.dev/main-concepts/auth-v2).

It is backwards-incompatible with applications using Auth v1.

- [BREAKING]: In order to use this version, you must set the authVersion prop 
    accordingly in your frontend: `Clerk.load({authVersion: 2})`

For more information on Auth v2, please refer to 
https://docs.clerk.dev/main-concepts/auth-v2.

## 1.0.3 - 2021-07-21

- fix: Proper endpoint for oauth_access_token method

## 1.0.2 - 2021-06-03

- fix: Instantiation of `Clerk::SDK` without prior call to `Clerk.configure`

## 1.0.1 - 2021-06-03

### enhancements

- Middleware now uses a proxy object which lazy loads the Clerk session and user only when needed

## 1.0.0 - 2021-05-27

- initial release
