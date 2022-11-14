# Viewing and Creating Games

Your first Django ViewSet and React components you should create are for viewing a list of all games in the system, and then a form for creating a game.

## Django Files

1. `raterproject\views\__init__.py`
1. `raterproject\views\game.py`

## React Files

1. `utils/data/gameData.js`
1. `pages/games/index.js`
1. `pages/games/[gameId].js`
1. `pages/games/edit/[gameId].js`
1. `pages/games/new.js`
1. `components/game/GameList.js`
1. `components/game/GameDetails.js`
1. `components/game/GameForm.js`

## Feature Requirements

In the React client, make sure there is a navigation bar link labeled "Games". When the user clicks that hyperlink, the URL in the browser should change to http://localhost:3000/games.

What should appear is a list of all games in the database. Start with just displaying the name of the game, which should be a hyperlink.

When the user clicks on a game name, the URL should change to http://localhost:3000/games/{id} and the game detail component should render and show the following information.

* Title
* Designer
* Year released
* Number of players
* Estimated time to play
* Age recommendation
* Categories

## Creating a Game

Once you have the basic information being shown in the list, add a link or a button at the top of the list labeled "Register New Game". When the user clicks it, the game creation form should appear.

The first version of the form should allow a user to only add one category to a game by choosing a category option in a `<select>` element.

When the the user fills out the form and clicks "Save", automatically redirect the user back to the game list view.
