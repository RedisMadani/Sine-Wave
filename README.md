# Sine Wave Generator

![equation](https://github.com/RedisMadani/Sine-Wave/assets/136177376/1e103556-9bd2-4de8-8c7a-76088b95da00)

![screenshot](https://github.com/RedisMadani/Sine-Wave/assets/136177376/25fb99a7-1c62-46ac-84ff-9188c6ef39e1)

This script generates a sine wave using the turtle graphics library in Python. The user can customize the amplitude, wavelength, horizontal shift, and vertical shift of the wave.

## Prerequisites

- Python 3.x
- Turtle graphics library

## Installation

1. Clone the repository or download the script file.
2. Make sure you have Python installed on your system.
3. Install the turtle graphics library by running the following command:

   ```
   pip install turtle
   ```

## Usage

1. Open the script in a Python IDE or text editor.
2. Modify the values of the variables `A`, `B`, `C`, and `D` to adjust the wave properties:
   - `A`: Amplitude of the wave (default: 50)
   - `B`: Wavelength of the wave (default: 100)
   - `C`: Horizontal shift of the wave (default: 0)
   - `D`: Vertical shift of the wave (default: 0)
3. Run the script.
4. A turtle graphics window will open, displaying the generated sine wave.

## Example

```python
from turtle import *
from math import *

A = 50      # Amplitude
B = 100     # Wavelength
C = 0       # Horizontal Shift
D = 0       # Vertical Shift

penup()
for x in range(-200, 200):
    y = A * sin((2 * pi / B) * (x + C)) + D
    goto(x, y)
    pendown()

hideturtle()
mainloop()
```

In this example, the script generates a sine wave with an amplitude of 50, wavelength of 100, no horizontal shift, and no vertical shift.

## License

This project is licensed under the [MIT License](LICENSE).
