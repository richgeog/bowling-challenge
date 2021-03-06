
Bowling Challenge
=================
[![Build Status](https://travis-ci.org/richgeog/bowling-challenge.svg)](https://travis-ci.org/richgeog/bowling-challenge) [![Test Coverage](https://codeclimate.com/github/richgeog/bowling-challenge/badges/coverage.svg)](https://codeclimate.com/github/richgeog/bowling-challenge/coverage) [![Code Climate](https://codeclimate.com/github/richgeog/bowling-challenge/badges/gpa.svg)](https://codeclimate.com/github/richgeog/bowling-challenge)

## Task:

Count and sum the scores of a bowling game for one player.

A bowling game consists of 10 frames in which the player tries to knock down the 10 pins. In every frame the player can roll one or two times. The actual number depends on strikes and spares. The score of a frame is the number of knocked down pins plus bonuses for strikes and spares. After every frame the 10 pins are reset.

Create a nice interactive animated interface with jQuery.


## Bowling rules

### Strikes

The player has a strike if he knocks down all 10 pins with the first roll in a frame. The frame ends immediately (since there are no pins left for a second roll). The bonus for that frame is the number of pins knocked down by the next two rolls. That would be the next frame, unless the player rolls another strike.

### Spares

The player has a spare if the knocks down all 10 pins with the two rolls of a frame. The bonus for that frame is the number of pins knocked down by the next roll (first roll of next frame).

### 10th frame

If the player rolls a strike or spare in the 10th frame they can roll the additional balls for the bonus. But they can never roll more than 3 balls in the 10th frame. The additional rolls only count for the bonus not for the regular frame count.

    10, 10, 10 in the 10th frame gives 30 points (10 points for the regular first strike and 20 points for the bonus).
    1, 9, 10 in the 10th frame gives 20 points (10 points for the regular spare and 10 points for the bonus).

### Gutter Game

A Gutter Game is when the player never hits a pin (20 zero scores).

### Perfect Game

A Perfect Game is when the player rolls 12 strikes (10 regular strikes and 2 strikes for the bonus in the 10th frame). The Perfect Game scores 300 points.

In the image below you can find some score examples.

![Ten Pin Score Example](images/example_ten_pin_scoring.png)

## How to setup

In terminal:
````
open SpecRunner.html
````
* In the browser `inspect element`
* Select console, type `frame = new Frame`

## Testing

Jasmine:
````
open SpecRunner.html
````

## V1

* The game begins with 10 pins and 2 balls to be thrown per frame
* A ball can be thrown
* 2 balls can be thrown in one frame
* The score for each frame is totalled

## Still to do

* After either 10 pins are knocked down in 1 ball or after 2 balls are thrown in a frame it moves to the next frame
* It knows what a gutter game is
* Strikes and spares are added up and included into the last frame
* Knows what a perfect game is
* CSS

## Key learnings

*
*
