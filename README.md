# ecs.pizza 
How much pizza do YOU eat?

## A competitive pizza tracking system 
ecs.pizza was developed during CampusHack, a 24 hour hackathon held in March 2018. It was run by
the [Electronics and Computer Science Society](https://society.ecs.soton.ac.uk) at the University of Southampton.
Despite being barely relevant to the theme of the hackathon, ecs.pizza was awarded third place.

## Repositories
ecs.pizza is split up over multiple repositories to separate out the components:

- [ecspizza-android][ecspizza-android]
  - Android Client 
  - Written in Java
- [ecspizza-art][ecspizza-art]
  - Art assets for the project
- [ecspizza-fingerprint][ecspizza-fingerprint]
  - Custom Computer Vision algorithms
  - Written in Python with the OpenCV library
  - Creates a finger from a picture of a pizza that can then be used to see if two pictures are of the same pizza
  - Prevents *cheating*!
- [ecspizza-flask][ecspizza-flask]
  - Web Client + API
  - Written in Python with [flask][flask]
  - User registration and login system
  - Pizza Leaderboard
  - Works with ecspizza-ispizza to verify images
  - Exposes a REST API for the Android App
- [ecspizza-ispizza][ecspizza-ispizza]
  - Machine learning algorithm to detect pizza.
  - Essentially a wrapper around [TensorFlow][tensorflow]
  - Ensures that submitted images are pizza.
- [ecspizza-presentation][ecspizza-presentation]
  - The presentation we gave at the hackathon
  - Written in [reveal.js][reveal]

[ecspizza-android]: https://github.com/dysfunctionals/ecspizza-android
[ecspizza-art]: https://github.com/dysfunctionals/ecspizza-art
[ecspizza-fingerprint]: https://github.com/dysfunctionals/ecspizza-fingerprint
[ecspizza-flask]: https://github.com/dysfunctionals/ecspizza-flask
[ecspizza-ispizza]: https://github.com/dysfunctionals/ecspizza-ispizza
[ecspizza-presentation]: https://github.com/dysfunctionals/ecspizza-presentation
[flask]: http://flask.pocoo.org/
[tensorflow]: https://www.tensorflow.org/
[reveal]: https://revealjs.com/
