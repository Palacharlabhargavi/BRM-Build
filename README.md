# BRM-Build

# server>> storing certain book data

        >> user register
        >>subscriber

# This is a book rrecord management API server/ Backend for library system or management of recorde or manuals or books

Fine system:
User:06/07/2024-07/08/2024
10/08/2024-50\*3=150

## subscription types

3 months(basic)
6 months(standard)
12 months(premium)

> > if the subscription type is standard && if the subscription date is 06/7/2024
> > then subscription valid till 06/10/2024
> > within subscription date >> if we miss the renewal >>50/- day
> > subscription date is also been missded >> and also missed the renewal >> 100 + 50/- day

> > book1
> > basic 06/03/2024 -> subscription date 07/03/2023 => borrowed a book from library book1 renewal date is on 21/03/2024 23/03/2024 => we need to pay a fine of 50

> > book2
> > basic 06/03/2024-> subscription date 07/03/2023 => borrowed a book from library book2 renewal date is on 21/03/2024 23/06/2024 => we need to pay a fine of 100+50

missed by renewal date >> 50/-
missed by subscription date >> 100/-
missed by renewal && subscription date >> 150/-

# routes and endpoints

## /users

> > post: it is usede to create new user
> > Get:get all the info here

## /user/{id}

GET: get the user id
Put: Update a user by their id
DELETE: Delete a user id(check if that person still have an issued book)&&(is there any fine to paid)

## /users/subscription-details/{id}

GET:get user subscription details >>Date of subscription >>valid till >>is there any fine

## /books

GET: Get all thge books
POST:create/Add a new book

## /books/{id}

GET: get a book id
Put:UPdate a book by id

## /book/issued

GET: GET all issued books

## /books/issued/with fine

    GET: get all issued books with their fine

npm init
npm i nodemone --save-div
