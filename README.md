# Overview

A simple farming program that remove unnecessary grinding in Pokemon Planet :)

# Install

`pip install pytesseract selenium numpy Pillow Wheel Playsound`

Also download Tesseract OCR from its github site.

# Setup

* Update 4 attributes called: `{path to browser exe}`, `{username}`, `{password}`, and `{path to tesseract}`
* Update arrays of pokemon actions
* Update `battle_log` pixel location to adjust for different screen size. Reference demo image `battle-log.png`.

## Optional Setup
* Update `use_potion` and `use_recover_move` as a auto recovery option when you pokemon gets injured
* Update `encounter` variable condition according to your pokemon strength (if you decide to enable the first bullet point)
* Uncomment codes in `play()` to enable these options

# How it works

This program walks your character left and right (you would want left and right barriers). After encountering a wild pokemon, the program detects which pokemon was encountered and performs one of three action: fight, run, and catch. 

## Fight

Uses the first move of the active pokemon against the encountered pokemon

## Run

Run away from the encountered pokemon

## Catch

Doesn't actually catch the pokemon. It plays a notification sound to let user know a 'catch' pokemon is encountered


# Future Implementation
* Enable auto fishing using OpenCV
* Enable auto mining
* Enhance potion use with image matching via OpenCV
* Handle Evolution and Learn New Move events
* 