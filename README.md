# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list

### How to run

after  clone this project, you should do the following steps:

1. Open terminal and go to your local directory where you have cloned this repository.

2. Run `npm install` in order to install all dependencies of the application.

3. Run `npm instal -g pnpm` in order to install all dependencies of the pnpm.

4. Run `pnpm run dev` to launch the application in development mode. You can now see the application at `http://localhost:8080`.

5. Paste the link ('http://localhost:8080') that will be provided by pnpm into your browser. You should see the main page of our Gym Management System.

### How to  use the app?

1. In the main page, you should be able to see one portal for login. Through that single login page, you can access 1)Admin Portal, 2)Member Portal aswell as the 3)User portal.

    1) Admin Portal:

        email: admin@gmail.com
        password: 123456789

        Using the above credetials you can login as an admin. You will be redirected to the dashboard page contains 2 pages,

            a) Manage Members:-

                i) 'Add Member' button which is to add new members to the Gym. In which you can create new credentials for the members and can also add other details like fees, weight, address etc..

                    - Using the credentials provided by the admin, a member can log in to the portal.
            
                ii) Refresh button to refresh the site in order to update the changes that made(added member).

                iii) Added member details. In that you can see all the members that have added, their health condition,  also you can edit the details. You will also have option to:

                    -Bill Not Paid: to mark a member  bill as not paid.

                    -Send Bill Reminder: to remind the  member about his unpaid bills.(This notifications will be send to the member in which the member can see that in member's portal).

            b) Report:- 


                i) Total number of members

                ii) Total income

                iii) Total due

                    etc...
            
            c) Log Out:

                also there will be an option to log out and go back to the log in page.
        

    2) Member Portal:

        By using any of the Member credentials given in the admin portal, you can login into a Member account. 
        For example,

            email: officialniranjan10@gmail.com
            password: Niranjan@45

            using this email you can login to the member account of member 'Niranjan'

        The Member Dashboard contain 2 pages,

            a) View Bill:-

                i) Monthly Bill: Here you can see the monthly bill asign to the correspoding member by the admin.

                ii) Last Bill Payment: Here you can see your last payment date.

                iii) Personal Information: Here you can see the member personal imformations like name and email.

            b) Notification:- 

                Here you can see if there is any  notification for you or not. If yes then it will show that notification otherwise "No Notification Yet". Notification can be send from admin.

            c) Log out:-

                also there will be an option to log out and go back to the log in page.

    3) User Portal:

        By using any of the user credential users can access their dashboard. If there's no account, you can register one.  And use the same credential to login.