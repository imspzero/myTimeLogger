# myTimeLogger
A cross-platform, GitHub-based time tracker powered by Flutter. It can be used as a logger or a journal.

## Inspiration
* I fell in love with this app named [iTodayss](https://github.com/Yaohong9257/iTodaysshttps://github.com/Yaohong9257/iTodayss) a few years ago. As far as I know, it is the best time management app. Unfortunately, it only supports Android, and this makes it inconvenient for computer-based scenarios. This app is only a simple copy of **iTodayss**, honor to [Yaohong9257](https://github.com/Yaohong9257).
* This book [time-as-a-friend](https://github.com/xiaolai/time-as-a-friend) talked me into adopting the habit of time tracking. From this book I knew *Aleksandr Lyubishchev*. 
* "Carpe diem. Seize the day." - [Dead Poets Society](https://www.youtube.com/watch?v=vi0Lbjs5ECI)

## Design Detail
* I simply aim at cross-platform, hence, it is powered by Flutter.
* Considering data privacy and accessibility, I choose not to host the backend. I did consider some options here.
  * Google Drive? Not a good idea. Not everyone can access google.
  * Firebase? Not a good idea. I don't want to obtain and maintain the user's data.
  * Some third-party storage services? Not a good idea as well, lack of freedom.
  * Local storage only? Not an option at all because it should be able to be usable and consistent on various platforms.
* Then GitHub API came to my mind. Why not? We just need to 
  1. Create a GitHub account
  2. Create a private repository
  3. Generate a private access token [link here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
  4. Use the above information to access the GitHub API. After all, the data itself is not complicated and huge.
* I am too lazy, and choose to store the data using [issues](https://docs.github.com/en/rest/reference/issues). In this way, the repo might look messy, but it should be fine because it is a private repo and no one can see it. I assume a user only has a few thousand records per year.

## Source Code
* It is not in the stable state right now. Only 40% of functionalities are implemented at the moment. 

## TODO
* Many ideas and functions are to be implemented, but to start recording is a good beginning. 
* The data can be integrated with GitHub Actions.

