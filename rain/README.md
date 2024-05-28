# Rainwater Retention Calculator

This Python program calculates the total amount of rainwater retained between walls after a rainstorm. The walls are represented as a list of non-negative integers, with each integer representing the height of a wall of unit width 1. The program views the cross-section of a relief map to determine the water retention.

## Function Prototype

```python
def rain(walls):

Parameters
walls: A list of non-negative integers representing the heights of walls.
Return Value
Returns an integer indicating the total amount of rainwater retained.
Assumptions
The ends of the list (before index 0 and after index walls[-1]) are not walls and will not retain water.
If the list is empty, the function returns 0.
Example Usage
Code
Create a file named 0_main.py with the following content:
```

#!/usr/bin/python3
"""
0_main
"""
rain = **import**('0-rain').rain

if **name** == "**main**":
walls = [0, 1, 0, 2, 0, 3, 0, 4]
print(rain(walls)) # Output: 6
walls = [2, 0, 0, 4, 0, 0, 1, 0]
print(rain(walls)) # Output: 6

Execution
Run the script using the following command:

jesse@ubuntu:~/$ ./0_main.py
6
6
jesse@ubuntu:~/$

Visual Representation
Walls: [0, 1, 0, 2, 0, 3, 0, 4]
The walls are represented in the following way:

bash

    #
    #
    #   #
    #   #
    #   #

#

#

Certainly! Below is a fully designed README file for the Rainwater Retention Calculator project, incorporating all necessary details for easy understanding and usage:

markdown
Copy code

# Rainwater Retention Calculator

This Python program calculates the total amount of rainwater retained between walls after a rainstorm. The walls are represented as a list of non-negative integers, with each integer representing the height of a wall of unit width 1. The program views the cross-section of a relief map to determine the water retention.

## Function Prototype

```python
def rain(walls):
Parameters
walls: A list of non-negative integers representing the heights of walls.
Return Value
Returns an integer indicating the total amount of rainwater retained.
Assumptions
The ends of the list (before index 0 and after index walls[-1]) are not walls and will not retain water.
If the list is empty, the function returns 0.
Example Usage
Code
Create a file named 0_main.py with the following content:

python
Copy code
#!/usr/bin/python3
"""
0_main
"""
rain = __import__('0-rain').rain

if __name__ == "__main__":
    walls = [0, 1, 0, 2, 0, 3, 0, 4]
    print(rain(walls))  # Output: 6
    walls = [2, 0, 0, 4, 0, 0, 1, 0]
    print(rain(walls))  # Output: 6
Execution
Run the script using the following command:

sh
Copy code
jesse@ubuntu:~/$ ./0_main.py
6
6
jesse@ubuntu:~/$
Visual Representation
Walls: [0, 1, 0, 2, 0, 3, 0, 4]
The walls are represented in the following way:

bash
Copy code
    #
    #
    #   #
    #   #
    #   #
#   #   #
#   #   #
Rainwater retained is shown as *:
```

Total water retained: 6 square units.

Walls: [2, 0, 0, 4, 0, 0, 1, 0]
The walls are represented in the following way:

#

#

#

#

#

#

Certainly! Below is a fully designed README file for the Rainwater Retention Calculator project, incorporating all necessary details for easy understanding and usage:

markdown
Copy code

# Rainwater Retention Calculator

This Python program calculates the total amount of rainwater retained between walls after a rainstorm. The walls are represented as a list of non-negative integers, with each integer representing the height of a wall of unit width 1. The program views the cross-section of a relief map to determine the water retention.

## Function Prototype

```python
def rain(walls):
Parameters
walls: A list of non-negative integers representing the heights of walls.
Return Value
Returns an integer indicating the total amount of rainwater retained.
Assumptions
The ends of the list (before index 0 and after index walls[-1]) are not walls and will not retain water.
If the list is empty, the function returns 0.
Example Usage
Code
Create a file named 0_main.py with the following content:

python
Copy code
#!/usr/bin/python3
"""
0_main
"""
rain = __import__('0-rain').rain

if __name__ == "__main__":
    walls = [0, 1, 0, 2, 0, 3, 0, 4]
    print(rain(walls))  # Output: 6
    walls = [2, 0, 0, 4, 0, 0, 1, 0]
    print(rain(walls))  # Output: 6
Execution
Run the script using the following command:

sh
Copy code
jesse@ubuntu:~/$ ./0_main.py
6
6
jesse@ubuntu:~/$
Visual Representation
Walls: [0, 1, 0, 2, 0, 3, 0, 4]
The walls are represented in the following way:

bash
Copy code
    #
    #
    #   #
    #   #
    #   #
#   #   #
#   #   #
Rainwater retained is shown as *:

bash
Copy code
    #
    #
    #   #
    #   #
    #   #
# * # * #
# * # * #
Total water retained: 6 square units.

Walls: [2, 0, 0, 4, 0, 0, 1, 0]
The walls are represented in the following way:

shell
Copy code
#       #
#       #
#       #
#   #   #
#   #   #
#   #   #
Rainwater retained is shown as *:

shell
Copy code
# * * * #
# * * * #
#   #   #
#   #   #
#   #   #
#   #   #
Total water retained: 6 square units.

Implementation Details
rain Function
The function works by:

Initializing two pointers, left and right, starting at the beginning and end of the list respectively.
Keeping track of the maximum height seen from the left (left_max) and from the right (right_max).
Moving the pointers towards each other, updating the maximum heights and calculating the water retained at each step.
```
