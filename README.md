# ~ Unity ~
## Viewport
* Viewport space represents a normalized position relative to the camera.
* `ViewportToWorldPoint()` converts a normalized position on the screen to a in 3D position in world space.
```
    (0,1) __________ (1,1)
         |          |
         |          |
         |          |
         |          |
         |          |
    (0,0)|__________|(1,0)
```
## Parallax Scrolling
* Multiple image layers scrolling at different speeds.
* Gives an artificial sense of depth.
* More layers give more depth.

## Audio in Three Parts
1. __Audio Listener__ - to "hear" the audio.
2. __Audio Source__ - to "play" the audio.
3. __Audio File__ - the "sounds" that get played.
***
# ~ C# ~
## Mathf.Clamp(float value, float min, float max)
* Clamps the given value between the given minimum float and maximum float values.
* Returns the given value if it is within the minimum and maximum range.
    * Returns the minimum value if the given float value is less than the minimum.
    * Returns the maximum value if the given value is greater than the maximum value.
* Use Clamp to restrict a value to a range that is defined by the minimum and maximum values.
* __NOTE:__ if the minimum value is is greater than the maximum value, the method returns the minimum value.
* Parameters:
    * __value__ - the floating point value to restrict inside the range defined by the minimum and maximum values;
    * __min__ - the minimum floating point value to compare against;
    * __max__ - the maximum floating point value to compare against.
* Returns float (the float result between the minimum and maximum values).
## Types of Loop
#### for loop
Runs a set number of times.
```
for(int i = 0; i < parent.childCount; i++)
{
    // do stuff
}
```
#### foreach loop
Works the same as a for loop but doesn't track the iterator.
```
foreach(type child in parent)
{
    // do stuff
}
```
#### while loop
Runs continuously while some condition is true.
```
while(condition == true)
{
    // do stuff
}
```
#### do-while loop
Runs once and then continuously repeats while some condition is true.
```
do
{
    // stuff
}
while(condition == true);
```