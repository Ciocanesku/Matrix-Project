# Matrix Project - Bomberman :bomb:

This is a Bomberman game implemented on Arduino as a final project for the robotics introduction course.

## Table of Contents

- [Game Rules](#game-rules)
- [The Menu](#the-menu)
- [Electronic Setup](#electronic-setup)
- [Demo Video](#demo-video)

## Game Rules

The objective of the Bomberman game is to destroy all the walls by placing bombs. In the game that I developed, you need to destroy the walls using a small number of bombs, the game is finished when you succesfully destroy all the walls. The game features different difficulty levels, including Easy, Medium, and Hard modes, each with its own set of challenges, every difficulty mode representing a different percentage of map walls generated. On any difficulty level you start with 2 lives, if you stay in the range of a bomb when it explodes 1 life will be deducted, if you remain with no lives the game will end and your score will not be saved. Each bomb explodes the walls from around it (including the diagonal neighbor). 


#### Known Bugs

- If I place a bomb on a room and I switch the room, the same led is still blinking on the matrix, but is not affecting the game, I find it more helpful for the times you play the game without sound to see when it is safe to return to the previous room.

## The Menu

Navigate through the game menu using the joystick. The menu includes options such as:

- Start game
- Settings
- About
- Highscores (top 3 highscores, a button to double-press for reseting all)
- About (details about the creator)
- How to play

Settings submenus allow you to customize:

- LCD brightness control
- Matrix brightness control
- Sounds ON or OFF
- Modify the name for the current session
- Back button

## Electronic Setup
![circuit bomber](https://github.com/Ciocanesku/Matrix-Project/assets/103603726/be30bd55-2405-4e05-a3c7-a0aa8e902ecf)



### Hardware Components

- Arduino UNO
- 16x2 LCD
- 8x8 LED matrix
- Joystick
- Buzzer

### Pin details
#### LCD Pins
- rs - 9
- en - 8
- d4 - 7
- d5 - 6
- d6 - 5
- d7 - 4
- brightness pin - 10
#### 8x8 Matrix Pins
- din pin - 12
- clock pin - 13
- load pin - 2
#### Joystick Pins
- X-axis pin - A0
- Y-axis pin - A1
- joystick button pin - A4


## Demo Video

Watch the demo video of the Bomberman game:  [Watch the video](https://youtu.be/Mgx98ooZ_o8).


Enjoy playing the Bomberman game on Arduino! 🕹️
