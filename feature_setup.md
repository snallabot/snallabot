# Setting up Snallabot features

We recommend to first setup teams, then setup game channels. All other features of the bot are optional

## Setting up teams

Snallabot provides an easy interface to assign teams for your league. 

1. first run `/teams configure` with the channel you would like to display the teams in and if you would like automatic role tracking
2. [OPTIONAL, NOT REQUIRED] if you are using automatic role tracking, create a role for every team in the league. Otherwise, proceed to the next step
3. assign every team to a user using `/teams assign` supplying the team, the user, and optional role to track on (if you did step 2)
4. You are now setup to use teams!
5. use `/teams open` with the team name, city, or abbreviation to free a team

if you run into permission issues, snallabot should let you know. Make sure snallabot can send messages in the channel you provide in step 1. Snallabot will also need to server member permissions to read users and roles. 

## Setting up game channels

1. /game_channels configure to setup game channels. youll need: a category to create in, admin role, and a wait ping that will schedule reminders, and a scoreboard channel. 
2. /game_channels create will create the channels for your week. make sure all the steps complete with a checkmark
3. [Optional] Want to save your game channels? Turn on snallabot logger! run `/logger configure` with the channel you want to output the game channel logs in. This might be noisy so be careful!

Snallabot wil need create channel, edit channel, create message, and server member permissions to track game channels. 

## Setting up stream counts

1. first run `/streams configure` with the stream channel you would like to post the counts in
2. you can now start counting streams with `/streams count` with the user who streamed!

## Setting up broadcasts

1. first run `/broadcasts configure` with the keyword for your league and the channel you want broadcasts in. Optional role for anyone to be mentioned. The keyword is to only show streams for your league, this must be in the title of any twitch/youtube stream for snallabot to post it!
2. then add your channels with Youtube with, `/broadcasts youtube add` or Twitch with `/broadcasts twitch add`
