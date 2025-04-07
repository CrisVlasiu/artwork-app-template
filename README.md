### Frontend - Artwork App

## Introduction

This assessment task involves creating an app that presents a collection of artwork along with information about each piece. The assessment typically takes about an hour, but you can spend as much time as needed to meet the requirements.

## What We're Looking For

- Do you know how Next.js works, including the app directory and data fetching?
- Can you build a responsive design using Tailwind CSS that works across all screen resolutions?
- Can you work effectively with a JSON response from an API?
- Can you add interactivity to the client using React?


We don't need your best work! If you can meet the above criteria and explain what you would have done with more time, that's totally fine with us.

## Goal

The goal is to create an app that presents a collection of artwork along with some information about each piece.

## Requirements

### Homepage

- The homepage should display all available artwork
- Each piece of artwork on the homepage should display a title and an image
- Each piece of artwork on the homepage should link to an individual artwork page


### Artwork Page

- Each piece of artwork should be available on a unique URL, e.g. `/artwork/[id]`
- The artwork page should display the title and image of the artwork
- The artwork page should contain a description that is hidden by default, but can be made visible by clicking something


Feel free to get creative with the UI. We have intentionally left the requirements vague so that you can showcase your skills and ideas comfortably.

## Development

### Git

You should see a directory called "artwork-app". This is your project directory - please navigate to it and initialize it as a new git repo.

Try to make regular atomic commits to the repo so that we can look through the history and understand your approach.

### Dependencies

We've used pnpm for dependencies but feel free to use npm, yarn or whatever you like.

## API

Below is a reference to the values you'll likely need in the app. If needed, full documentation for the API can be found [here](https://api.artic.edu/docs/).

### All Artwork

https://api.artic.edu/api/v1/artworks

```json
{
  "data": [
    {
      "id": 129884,
      "title": "Starry Night and the Astronauts",
      "image_id": "e966799b-97ee-1cc6-bd2f-a94b4b8bb8f9",
    },
  ]
  "config": {
    "iiif_url": "https://www.artic.edu/iiif/2",
  }
}
```

The type `ArtAPIResponseArtworks` is included in the project for your convenience.

### Individual Artwork

https://api.artic.edu/api/v1/artworks/129884

```json
{
  "data": {
    "id": 129884,
    "title": "Starry Night and the Astronauts",
    "image_id": "e966799b-97ee-1cc6-bd2f-a94b4b8bb8f9",
  },
  "config": {
    "iiif_url": "https://www.artic.edu/iiif/2",
  }
}
```

The type `ArtAPIResponseArtworks` is included in the project for your convenience.

### Images

Here is an example of an image URL: -
https://www.artic.edu/iiif/2/e966799b-97ee-1cc6-bd2f-a94b4b8bb8f9/full/843,/0/default.jpg

The URL consists of the following:

```plaintext
{iiif_url}/{image_id}/full/843,/0/default.jpg
```

The values for `iiif_url` and `image_id` can be seen in the API responses above.

Sometimes images can return 404s - if you struggle to get images to display, try a different page from the artwork endpoint, e.g. `https://api.artic.edu/api/v1/artworks?page=3`

## Completing the Test

1. Create a GitHub account or use an existing one
2. Create a private repo
3. Push your code
4. Go to settings → collaborators → add people
5. Add the following emails:

1. [daniel.yefet@betwaygroup.com](mailto:daniel.yefet@betwaygroup.com)
2. [cristian.vlasiu@betwaygroup.com](mailto:cristian.vlasiu@betwaygroup.com)





## Tips for Time Management

- Spend a little bit of time upfront exploring the project and the API. Think about a rough plan for your approach and implementation.
- Prioritize any points outlined in the "Requirements" section and cross-reference them with the criteria specified in "What we're looking for" to ensure your work aligns with those expectations.
- You are welcome to utilize any additional time for further enhancements, such as leveraging more features from the API, incorporating extra UI/UX features or making use of framework functionality. This is completely optional and entirely up to you!
