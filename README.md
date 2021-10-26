# CostumeDB Backend

This repository serves as the backend of [CostumeDatabse.com](https://costumedatabase.com/). If you have an idea, feel free to contribute!

The Costume Object has fields for name, origin, imageUrl, fandomLink, description, theme, size, and characters. 

Example:
```json
{
    "name": "Ross and Rachel",
    "origin": "Friends",
    "imageUrl": "https://static.wikia.nocookie.net/friends/images/c/c9/Ross_and_Rachel_-_Final_Kiss_-_10x18.png",
    "fandomLink": "https://friends.fandom.com/wiki/Ross_and_Rachel",
    "description": "On again off again Rachel and Ross are one of the central couples on Friends. Were they on a break? It's up to you!",
    "theme": ["sitcom", "romantic"],
    "size": 2,
    "characters": [
      {
        "hair": "brown",
        "gender": "male"
      },
      {
        "hair": "brown",
        "gender": "female"
      }
    ]
  }
```

### fields
- `name`: the name of the costume
- `origin`: where the costume is from (often, the name of the show or movie)
- `imageUrl` (optional): an image of the characters
- `fandomLink` (optional): a link to a fandom page where people can learn more
- `description`: a brief description of the characters
- `theme`: a list of themes the costume may fall under
- `size`: how many people is the costume for?
- `characters`: a list of the characters, represented by hair color/gender

### general notes
Please read the terms of use on [CostumeDatabase.com](https://costumedatabase.com/terms). Thanks for helping us out :)

[More information about contributing to Github](https://www.dataschool.io/how-to-contribute-on-github/)
1. Fork the project repository 
2. Clone your fork 
3. Add this repo as an upstream `git remote add upstream https://github.com/reaganhenke/costume-db-backend`
4. Pull the latest `git pull upstream main`
5. Create a new branch
6. Commit your changes and push them to your fork
7. On Github, open a Pull Request against the base-repository

We may close or request changes on pull requests that don't meet the requirements. Thanks for helping us out!
