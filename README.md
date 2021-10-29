# CostumeDB Backend

This repository serves as the backend of [CostumeDatabase.com](https://costumedatabase.com/) (code is over at [costume-db](https://github.com/reaganhenke/costume-db)). If you have an idea, feel free to contribute!

The Costume Object has fields for name, origin, imageUrl, fandomLink, description, theme, size, and characters. 

Example:
```json
{
  "name": "Belcher Kids",
  "origin": "Bob's Burgers",
  "imageUrl": "https://i.imgur.com/scYENWc.png",
  "fandomLink": "https://bobs-burgers.fandom.com/wiki/Belcher_Family",
  "description": "No siblings are closer than Tina, Gene, and Louise!",
  "theme": ["siblings"],
  "size": 3,
  "characters": [
    {
      "hair": "black",
      "gender": "male"
    },
    {
      "hair": "black",
      "gender": "female",
      "glasses": true
    },
    {
      "hair": "black",
      "gender": "female"
    }
  ]
}
```

## fields
- `name`: the name of the costume
- `origin`: where the costume is from (often, the name of the show or movie). 
- `imageUrl` (optional): an image of the characters. The image needs to be hosted somewhere we can render it. See the image section below. 
- `fandomLink` (optional): a link to a fandom page where people can learn more
- `description`: a brief description of the characters
- `theme`: a list of themes the costume may fall under
- `size`: how many people is the costume for?
- `characters`: an array of the characters (more detail in the next section)

## characters
Characters have fields for hair, gender, glasses, and if they can be a pet or not. It looks like this:
```json
      {
        "hair": "brown",
        "gender": "female",
        "glasses": true,
        "pet": false
      }
```

Users can search for the following hair colors:
- `black`
- `blond`
- `brown`
- `red`
- `gray`
- `blue`
- `pink`
- `green`
- `bald`
- `any`: The "any" type should be used when the character can have any hair color. For example, a costume of Mustard and Ketchup. "any" types will be returned even if the user searches for a specific color.
If the user doesn't specify hair color, all of the above may be returned.

Users can search for the following genders:
- `male`
- `female`
- `any`: The "any" type should be used when the character can have any gender. For example, a costume of Mustard and Ketchup. 
If the user doesn't specify gender, all of the above may be returned. 

You may leave out the `glasses` and `pet` fields if they aren't relevant. 

## images
This field is for a link to an image of the characters/costume. It is optional, if you don't provide one a fallback will be used. Avoid using fan art or cosplay photos, we want to see the original characters!

Note that the image must be able to be used as a `src` attribute (it can't have CORS headers blocking us). We've found [imgur](https://imgur.com/) works great for hosting images. Unsure if your image link will work? Test it out using the following steps. 

Use this [Tryit Editor from W3Schools](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_trulli) and replace the `src` value with your URL. If it renders successfully, you're good to go!

## general notes
Please read the terms of use on [CostumeDatabase.com](https://costumedatabase.com/terms). Thanks for helping us out :)

[More information about contributing to Github](https://www.dataschool.io/how-to-contribute-on-github/)
1. Fork the project repository 
2. Clone your fork 
3. Add this repo as an upstream `git remote add upstream https://github.com/reaganhenke/costume-db-backend`
4. Pull the latest `git pull upstream main`
5. Create a new branch
6. Commit your changes and push them to your fork
7. On Github, open a Pull Request against the base-repository

Please make sure your pull request is up to date with the latest changes from master; you're responsible for resolving any merge conflicts. We may close or request changes on pull requests that don't meet the requirements. Feel free to ask any questions you may have. Thanks for helping us out!
