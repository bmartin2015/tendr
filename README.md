# Tendr - the Tindr of Food

This is one of our projects for Dev Bootcamp. It is a Tinder clone for food.

# Team
* [Juan](https://github.com/zjuanz)
* [Sarah](https://github.com/sbetack)
* [Wes](https://github.com/yellowjell0)
* [Ben](https://github.com/bmartin2015)

# Installation - Local
You will need to get a [Google Places Web Services API key](https://developers.google.com/places/web-service/get-api-key). Create a .env file in the root and add GOOGLE_PLACES_API_KEY=[YOUR GOOGLE API KEY] to it.

Execute
  $ bundle
  $ rails db:create db:migrate
  $ rails s

Then visit http://localhost:3000/api to load the basic Downtown and South Central Austin seed - note this takes 20 - 25 minutes


# Installation - Heroku
Add Heroku to your Git Remotes

Add your API key to the Heroku environment.

Push Master to Heroku Staging
```
git push staging master
heroku run rake db:migrate --remote staging
```


Push Master to Heroku Production
```
git push production master
heroku run rake db:migrate --remote production
```

To Drop Database - Something like:
```
heroku pg:reset --remote staging
```
# How to Use
