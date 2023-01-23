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
## foreach Loop
#### for loop
```
for(int i = 0; i < parent.childCount; i++)
{
    // do stuff
}
```
#### foreach loop
```
foreach(type child in parent)
{
    // do stuff
}
```