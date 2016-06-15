# Where Am I

Where Am I is a clone of [GeoGuessr](https://geoguessr.com/), a game that places the player in a random spot in the world via Google Street View and expects them to guess where they are. The player receives a score based on how close their guess was to their actual location.

## Features

 - [ ] On game start, the player is placed in a random part of the world on Google Street View.
 - [ ] The player can move and look around to the extent that Street View will let them, and can use Street View controls to do so.
 - [ ] The player can enter a guess on the world mini-map.
 - [ ] After making their guess, the player is shown an appropriately-zoomed map with markers on the location of their guess and on their actual location. A line is drawn between the two markers, and the player is told their score and the distance between the markers in miles.
 - [ ] After several rounds, the game is over. The player is shown their total score, and a world map displaying the markers and lines from each round.

## Timeline

### Phase 1

- [x] Build basic `GameView` component that properly sets up connection to Google Maps API.
- [x] Configure view to show no more information than we want:
  - [x] Street View should always be on
  - [x] Street View controls should be on
  - [x] Street labels and other meta-information should be off
- [ ] Implement randomized placement (in a valid Street View location).

### Phase 2

- [ ] Build `GuessingMap` component that:
  - [ ] displays the entire world
  - [ ] and allows the user to enter a guess by placing a marker and clicking a submit button.
- [ ] Build `ResultsMap` component that:
  - [ ] places markers on the player's actual location at the time of guess and on the guessed location;
  - [ ] that draws a line between the two markers;
  - [ ] that displays the distance between the markers and the resulting score;
  - [ ] and that sets the map zoom to an appropriate amount (not too close, not too far)

### Phase 3

- [ ] Build `GameOverView` component that:
  - [ ] Displays the entire world
  - [ ] Displays the marker-pairs, lines, distances, and scores for each round on the map
  - [ ] Displays the player's total score
  - [ ] Provides a `New Game` button
- [ ] Build a `StartGame` component / landing page.
