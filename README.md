# myFlix-Angular-app

## Project Description
The myFlix Angular application was created with Angular and TypeScript. It is the client-side for a previously completed React application called myFlix based on its existing server-side code (REST API and database). 

### Key Features
* Users can register and log in
* Users can view a list of all movies by visiting the app's homepage
* Users can access different app views via a navigation bar
* Users can see detailed information about a single movie by clicking buttons to launch dialogs
* Users can add or remove movies from their favorites by clicking on the heart button 
* Heart buttons change colors to indicate whether movie is a favorite or not
* Users can view their favorite movies in the profile view
* Users can update their user information in the profile view
* Users can delete their accounts in the profile view
* Users can log out of their accounts

## Get the Project Running
Download the project locally and install the dependencies by running `npm install` and `npm install -g @angular/cli`. Then run `ng serve` from the `myFlix-Angular-client` directory.

The app is hosted on GitHub pages and can be viewed [there](https://n-townsend.github.io/myFlix-Angular-app/). 

## Updating The Documentation
In-depth documentation for this project can be viewed in the `index.html` file in the `docs` folder of `myFlix-Angular-client`. To add documentation to more components, they must first be added to the `tsconfig.json` file:

```json
"typedocOptions": {
    "entryPoints": ["./src/app/movie-card/movie-card.component.ts", "./src/app/app.component.ts", "./src/app/welcome-page/welcome-page.component.ts", "./src/app/user-profile/user-profile.component.ts"],
    "out": "docs"
}
```

Update the `index.html` file by running `npx typedoc --out docs` and adding all the routes at the end. For example, `npx typedoc --out docs ./src/app/movie-card/movie-card.component.ts ./src/app/app.component.ts`.

## Technologies
* Angular
* TypeScript
* Angular Material
