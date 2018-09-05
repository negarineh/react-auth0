This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).


Setting Up an Auth0 Application
To represent your React application in your Auth0 account, you will need to create an [Auth0 Application](https://auth0.com/docs/applications). So, head to [the Applications section on your Auth0 dashboard](https://manage.auth0.com/#/applications) and proceed as follows:

    1. click on the [Create Application button](https://manage.auth0.com/#/applications/create);
    2. then define a 'Name' to your new application (e.g., "React Demo");
    3. then select 'Single Page Web Applications' as its type.
    4. and hit the 'Create' button to end the process.

After creating your application, Auth0 will redirect you to its' Quick Start' tab. From there, you will have to click on the 'Settings' tab to whitelist some URLs that Auth0 can call after the authentication process. This is a security measure implemented by Auth0 to avoid the leaking of sensitive data (like [ID Tokens](https://auth0.com/docs/tokens/id-token)).

So, when you arrive at the 'Settings' tab, search for the 'Allowed Callback ' URLs field and add http://localhost:3000/callback into it. For this tutorial, this single URL will suffice.

That's it! From the Auth0 perspective, you are good to go and can start securing your React application.

Note: As you want the best security available, you are going to rely on the [Auth0 login page](https://auth0.com/docs/hosted-pages/login). This method consists of redirecting users to a login page hosted by Auth0 that is easily customizable right from [your Auth0 dashboard](https://auth0.auth0.com/login?state=jOgJlYBoPnUUXdPS6jl-ojATBoTSOtIf&client=zEYfpoFzUMEzilhkHilcWoNkrFfJ3hAI&protocol=oauth2&response_type=code&redirect_uri=https%3A%2F%2Fmanage.auth0.com%2Fcallback&scope=openid%20profile%20name%20email%20nickname%20created_at). If you want to learn why this is the best approach, check [the Universal vs. Embedded Login article](https://auth0.com/docs/guides/login/universal-vs-embedded) .


Source: [Securing React Apps with Auth0](https://auth0.com/blog/how-to-configure-create-react-app)
