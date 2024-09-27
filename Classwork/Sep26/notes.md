serverpackage.json lives in the root. Other server files live in the server folder. 

The client folder will contain all client attributes.



The pnpm steps to generate the boilerplate:

run the command pnpm create vue@latest

Next give the project a name.

Package name needs to be all lowercase.

Typescript: yes

jsx support: yes

vue router: yes

pinia for state management: no

unite testing: no

end to end testing: no

eslint: yes

prettier for formatting: yes

vue devtools: yes



Copy his settings.json file in the .vscode folder.

The public folder is any files that you want to end up on  your server, even if they're not part of your program.

We will be working in the src folder.

Looking at the .eslintrc.cjs file:
Lint warns you about bad code.

You can add rules to the linter.

Delete the extra .gitignore

the index.html should be in the Client folder. 

copy his package.json file. 

Take a look at the package.json folder created in the client.

In that file:

Change version to 0.0.1

After all that run npn run dev. You'll get an error because you don't have your packages installed.

To install them type: pnpm i. Once you use pnpm, you have to stick with it.

Running npm i will give you an error.

Then you can run pnpm run dev

This runs a local server. 

Vue doesn't need a server at all. 

We hve a server her because it's easier to run our compiler.

nuxt is a framework build on top of vue. Next is on top of react.