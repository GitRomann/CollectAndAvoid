## Engine version -> 5.6

## Character movement
# Max speed 600 -> 700
# Jump Z Velocity 420 -> 430
# Gravity scale 1 -> 1.2

# I use the cast when I pick up coin because I need to check overlapped actor. If it is hero, we can pick up the coin. If not, we don't do anything.

# I update the score in function not using event Tick because I need to call Update Score function once, not in every frame. In addition calling in every frame is bad for perfomance

# Pick up source - https://pixabay.com/ru/sound-effects/search/монета/
# The sound of danger - https://pixabay.com/ru/sound-effects/search/опасность/
# The sound of tranquility - https://pixabay.com/ru/sound-effects/search/спокойствие/

### Profiling:
Frame - 10-11 ms
draw and frame take the most time
the reason: event tick
i disabled event tick at some blueprints and game time became less


