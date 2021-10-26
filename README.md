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
Please read the terms of use on [CostumeDatabase.com](https://costumedatabase.com/terms). We can't promise all costumes will make it into the database or gaurantee any timelines. Thanks for checking it out :)

[More information about contributing to Github](https://www.dataschool.io/how-to-contribute-on-github/)