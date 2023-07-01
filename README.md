# flatiron-phase-2-project-backend

This repo contains the database for [flatiron-phase-2-project-frontend](https://github.com/StephenCsengo/flatiron-phase-2-project-frontend)

## Setup

Fork and clone this repo. Then install the dependencies by running:

```sh
npm install
```

## Seeding Data

To set up your database, update the `db/seeds.json` file to contain an object
with a key pointing to an array of data, like this:
```json
{
  "hikes": [
    {
      "id": 1,
      "park": "Air Line State Park Trail",
      "suggestedmi": 6,
      "description": "Flat multisurface trail",
      "difficulty": "Easy",
      "image": "https://cloudfront.traillink.com/photos/air-line-state-park-trail_181851_sc.jpg"
    },
    {
      "id": 2,
      "park": "Larkin State Park Trail",
      "suggestedmi": 6,
      "description": "Flat gravel trail",
      "difficulty": "Easy",
      "image": "https://2.bp.blogspot.com/-wdQs3_c4FNU/WDbkGyNtLuI/AAAAAAAAB4U/aKA5QV7ueyUA44UyjeI_60pjs7S9hpl0gCEw/w1200-h630-p-k-no-nu/Hop%2BRiver%2BTr.%252C%2Brock%2Bcut%252C%2B7-11.jpg"
    }
  ]
}
```

Then, run `npm run seed` to copy data from the `db/seeds.json` file to the
`db/db.json` file. `json-server` uses the `db.json` file to create your RESTful
API, so make sure your `db.json` file is always up to date!

Any time you want to reset your database back to your original data, run
`npm run seed` again. Doing this will overwrite all the data in your `db.json`
file, so make sure you don't have any data in that file that you don't mind
losing!

## Running the Server Locally

To run your server in development mode, run:

```sh
npm run dev
```

While running in development mode, the server will re-load any time you make
changes to the `db.json` file, so you can test our your seed data.

While your server is running, you can make requests to
[http://localhost:3000](http://localhost:3000). Check it out in the browser to
make sure your server works!

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
