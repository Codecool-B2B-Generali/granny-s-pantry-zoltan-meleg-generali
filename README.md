# Granny's Pantry

## Story

Little Red Riding Hood's granny learned the lesson and digitalized her pantry, to make ordering online easier. Problem is, she did not receive a full documentation, nor a frontend, so she needs help administrating the items in her pantry.

## What are you going to learn?

- create requests using Postman
- create collections of requests using Postman
- use variables in Postman


## Tasks

1. Create an account at [Postman](https://www.postman.com/). You can download the client or use the app from the browser
    - Have a Postman account.

2. Create a Pantry for your email at [Pantry](https://getpantry.cloud/). Keep your `Pantry id`, as it is important later.
    - Have an id for their Pantry.

3. Create a new `Workspace` in Postman, where you can later organize your collection of requests.
    - Have at least one Workspace in Postman.

4. Create a collection named `Grannys Pantry` in Postman, for storing requests in this project.
    - Have a Collection in Postman named `Grannys Pantry`

5. Check the details of your Pantry by creating a `GET` request to `https://getpantry.cloud/apiv1/pantry/<YOUR_PANTRY_ID>` using Postman. Save this request to your Collection, and name it `Get details`.
    - Have a GET request called `Get details` saved into your Collection.
    - Response status is 200 OK.

6. Create a new Basket in your Pantry by creating a `POST` request to `https://getpantry.cloud/apiv1/pantry/<YOUR_PANTRY_ID>/basket/<YOUR_BASKET_NAME>` using Postman. Save this request to your Collection, and name it `Create new basket`.
    - Have a POST request called `Create new basket` saved into your Collection.
    - Response status is 200 OK.

7. Create a collection variable for the `base URL` (`https://getpantry.cloud/apiv1/pantry/`) as `pantry_api_path`. Create a collection variable for your Pantry id as `pantry_id`. Create a collection variable for the basket you've created as `basket_name`. Use these variables in *all* of your requests. When you rewrite your previous ones, make sure they're still functional.
    - Have a variable called `pantry_api_path` for the API path, used in all requests in the Collection.
    - Have a variable called `pantry_id` for your Pantry id, used in all requests in the Collection.
    - Have a variable called `bakset_name` for your basket, used in all affected requests in the Collection.
    - Variables used in all requests.

8. Fill the basket by sending a `PUT` request to `https://getpantry.cloud/apiv1/pantry/<YOUR_PANTRY_ID>/basket/<YOUR_BASKET_NAME>` using Postman. The request body should contain the following: `{"fruits": ["apple", "banana", "peach"]}`. Name the request as `Update Contents`.
    - Have a `PUT` request called `Fill basket` saved into your Collection.
    - Response status is 200 OK.

9. Check the content of the basket by sending a `GET` request to `https://getpantry.cloud/apiv1/pantry/<YOUR_PANTRY_ID>/basket/<YOUR_BASKET_NAME>` using Postman. Name the request as `Get content of basket`.
    - Have a `GET` request called `Get content of basket` saved into your Collection.
    - Response status is 200 OK.

10. Delete the whole basket by sending a `DELETE` request to `https://getpantry.cloud/apiv1/pantry/<YOUR_PANTRY_ID>/basket/<YOUR_BASKET_NAME>` using Postman. Name the request as `Delete basket`.
    - Have a `DELETE` request called `Delete basket` saved into your Collection.
    - Response status is 200 OK.

11. Create a new Folder inside your Collection using Postman, and call it "Restore Basket". Put here the following requests: `Create new basket`, Get content of basket`, `Fill basket`.
    - Have a Folder called "Restore basket".
    - The folder contains all of these requests [`Create new basket`, Get content of basket`, `Fill basket`].

12. How lucky we've created variables! Restore the previously deleted basket, by running all requests in your "Check Basket" folder, without editing anything.
    - API path, Pantry ID, Basket name stored in variables, used in all requests.
    - By only running the folder, a student should be able to restore the basket described in the tasks.

13. Copy the content of `postman_tests.js`, (which be found in the starter repository) to the __Collections'__ `Tests`. All tests should pass.
    - All tests copied to the Collection Tests.
    - All tests pass.

14. By exporting your work anyone can import it and use your Collection which can be extremely useful. Export your Collection and put it in your Git repo!
    - Collection exported into `JSON`.
    - Collection can be found in the student's remote repository.

## General requirements

None

## Hints



## Background materials

- [About Workspaces in Postman](https://learning.postman.com/docs/collaborating-in-postman/using-workspaces/creating-workspaces/)
- [Sending the first request using Postman](https://learning.postman.com/docs/getting-started/sending-the-first-request/)
- [Using Collections in Postman](https://learning.postman.com/docs/sending-requests/intro-to-collections/#creating-collections)
- [Setting requests details in Postman](https://learning.postman.com/docs/sending-requests/requests/)
- [Using variables in Postman](https://learning.postman.com/docs/sending-requests/variables/)
- [Creating Folders in Postman](https://learning.postman.com/docs/sending-requests/intro-to-collections/#managing-collections)
- [Exporting Collections in Postman](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#exporting-collections)
