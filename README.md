# Sanity + Next.js frontend example

DEMO 👉 https://movie-sample-mm208c8mw.vercel.app/

This is an example [Sanity](https://www.sanity.io/) powered frontend for the movie dataset using [Next.js](https://github.com/zeit/next.js/).

## Prerequisites

You will need [Node.js](https://nodejs.org) version 8.0 or greater installed on your system.

## Setup

Get the code by either cloning this repository using git

```
git clone https://github.com/hanyangvl/sample-movies
```

Once downloaded, open the terminal in the project directory, and install dependencies with:

```
npm install
```

If you're running your own Sanity project with the example movie dataset, go to `lib/sanity.js` and change the following lines:

```
  projectId: 'YOUR_PROJECT_ID',
  dataset: 'NAME_OF_YOUR_DATASET',
```

You can locate the ID of your project in the header of the [management page for your project](https://manage.sanity.io/).

You also need to enable `localhost:3000` in your CORS Origins settings! Either through the [management page](https://manage.sanity.io/) under `settings` or by running the below in the project folder you set up with `sanity init`:

```
sanity cors add http://localhost:3000
```

Then start the example app with:

```
npm run dev
```

The app should now be up and running at http://localhost:3000 🚀
