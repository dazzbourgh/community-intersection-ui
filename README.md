# Community Intersection UI

A UI for application that finds people that are parts of all specified VK communities and whose profiles correspond to entered filters. Only publicly accessible information is used.

## Tech

Project uses Angular 7 and Docker for deployment.

## Usage

Enter IDs of communities separated by comma, fill in filter form, press "Find" and enjoy your new friends.

Example:

![Example](https://pp.userapi.com/c850724/v850724421/12941b/Ue6wqIVoM3A.jpg)

## Running

To run the app locally you will need the latest version of **npm** and **angular-cli**. Please refer to documentation for installation details.

Before running the app, you will need to install dependencies locally. Run `npm i` from the root of application (where **package.json** is located) to install the dependencies.

To run local dev server run `ng serve` from app root. This will set up development server and deploy the app to port `4200`, so you can access it in browser using the link `http://localhost:4200`.

## Using the app

Current authentication mechanism works the following way for local deployments:

1) Navigate to `localhost:8080/index`. This will trigger authentication on back end side of application. **NOTE:** back end should be up & running on port 8080 at this point.
2) Grant necessary permissions after you get redirected to VK
3) You will be redirected to `localhost:4200` fully authenticated with `SESSION` cookie set.
