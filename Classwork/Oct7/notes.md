pnpm i

This is a checkout. Whenever you're checking out a new repo/branch, or if you clone something, you always have to run pnpm i. 

This is because the modules folder isn't in the same state as package.json.


Next we will run: pnpm run dev

This will run the compiler and we can click on the server link it provides us.

Inside navbarvue file:

In the nav tag:
    Use any of the div tags.
    Write: div.container then hit enter
    put the div on the very bottom of the file.
    In the navbar class section write is-info


Now in App.vue:
    In the header tag write .container then hit enter
    In that div put RouterView />
    In the style tag write:

        body {
            background-color: aliceblue
        }

        .container {
            background-color: white;
            box-shadow: drop-shadow(0 0 10px rgba (0, 0, 0, 0.8));
            min-height: 100vh;
        }

