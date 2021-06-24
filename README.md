# CleanCloud API documentation 

Here you can find the Postman collection to access CleanCloud's APIs.

All the documentation related to the API can be found in [CleanCloud API docs](https://docs.cleancloud.io)

## User token

First it is required to have an account over CleanCloud's platform to be able to access the public API which also must be requested via https://cleancloud.io

With previous account setup done, it is required to create a user token by accessing one of the following links:

- [Score settings](https://score.cleancloud.io/#/settings)
- [Inspect settings](https://inspect.cleancloud.io/#/settings)

Also it is recommended to create a new user with ONLY API access as the API user can be leveraged to access all CleanCloud's APIs.

On CleanCloud's settings page click on the "Create token" button as shown below:

![user_token_step_1](https://user-images.githubusercontent.com/70276848/123280922-9b1b8680-d4df-11eb-970d-99e3ce87e65d.png)

Insert a name for the token and click on "Create" button, afterwards a dialog will present a user token **code** and **secret** which will be available just once.

![user_token_step_2](https://user-images.githubusercontent.com/70276848/123281297-f51c4c00-d4df-11eb-93bc-2e1cdd50e6cf.png)

Store the generated user token which will be used to dynamically generate an temporarly API tokens.

## Postman setup

Open the Postman application in your computer and import [CleanCloud API collection](https://github.com/cleancloud/api-doc/blob/main/cleancloud_api.postman_collection.json)

> File > Import > "Choose the downloaded collection"

Include manually the user token **code** and **secret** over environment variables as presented below:

![postman_user_token](https://user-images.githubusercontent.com/70276848/123282023-8986ae80-d4e0-11eb-92fa-fbbeb1bea432.png)

Afterwards expand the collection "CleanCloud API" and open the "API token" > "GET fetch api token" and generate a temporary API token:

![postman_api_token](https://user-images.githubusercontent.com/70276848/123282100-973c3400-d4e0-11eb-9332-b549dfc6ce1b.png)

Now with the API token in place, it is now time to perform requests against CleanCloud's APIs.

![postman_api_call](https://user-images.githubusercontent.com/70276848/123282232-b1761200-d4e0-11eb-9e98-4eab280cd15e.png)


All the documentation related to the API can be found in [CleanCloud API docs](https://docs.cleancloud.io) and [Development flows](https://docs.cleancloud.io/docs/cleancloud-api/docs/dev-flows.md)
