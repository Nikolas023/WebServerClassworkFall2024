Implementing the MVC.

pnpm i to make sure everything is up to date after doing git pull.

pnpm run dev to start working on the application.

Open the application by clicking the localhost link.

any index.vue needs to have a lower case i.

DummyJSON could be used for a test server.

We're going to take their json and use it.

Take the Json from this file: 'https://dummyjson.com/products'

Copy all the json.

In the source folder, make a new file and call it data/products.json. We're keeping files here for now but in the future it will be in a server.

Paste all the json there.


Now get a set of users from 'https://dummyjson.com/users.

Copy all that information then put it in the data folder, and call it users.json


We're going to make a folder called model. 

In source make a new file in source and call it: models/products.ts

This file shouldn't know that we're using vue.

in that typescript file import this: 



import data from '../data/products.json';
import type { DataListEnvelope } from './dataEnvelope'

export function getAll() : DataListEnvelope{
    return {
        data: data.items,
        total: data.total
    };
}



In the models folder, make another model and call it dataEnvelope.ts

In this file:


export interfaace DataEnvelope<T> {
    data: T;
    error: string;
}

export interface DataListEnvelope<T> {
    data: T[]
    total: number
    error: string
}


Figure out what the question mark does in typescript when it 
is put next to a variable like this:

price?: number

The ? makes stuff optional. This fixes 'something is declared but not used' errors.

In pages make a new file: Products/index.vue

vbase for a vue setup


go in the component folder and make a new file called ProductCard.vue



