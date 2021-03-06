# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED (10pts)
- [x] (5pts) User can tap a cell to see more details about a particular movie.
- [x] (5pts) User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.

#### BONUS
- [ ] (2pts) User can tap a poster in the collection view to see a detail screen of that movie.
- [ ] (2pts) In the detail view, when the user taps the poster, a new screen is presented modally where they can view the trailer.

### App Walkthrough GIF

<img src="https://github.com/mialsy/iOS_codepath_assignment1/blob/main/FlixPart2Demo.gif" width=250 alt="Part 2 demo gif here. Let me know if this link breaks"><br>

### Notes
- Grid view appear to be very small
  - Solution: checked slack channel and see people have the same problem, fix by setting the estimate size to none.

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [ ] (1pt) Run your app on a real device.

### App Walkthrough GIF

<img src="https://github.com/mialsy/iOS_codepath_assignment1/blob/main/FlixDemo.gif" alt="Demo gif here. Let me know if this link breaks" width=250><br>

### Notes
- XCode version different from the video guide, lauch screen not initialized.
  - Solution: add lauch screen file manually, and change the name to corresponding name to be able to include in the app.
  - Note: The file name has to be the same, possible other solution need to be further explored.
- Issue with text view to controler mapping:
  - Solution: figured out that there was a wrong duplicated controller link to the text view, delete duplicate can solve the problem.
  - Note: Make sure to check the controller mapping after it is established.
- Network issue with calling tmdb APIs
  - Solution: tried to call tmdb APIs directlly and still not working, then realized that I used http protocol rather than https protocol, changed to https as documented in the tmdb website fixed issue.
  - Note: be sure to distinguish https and http.
