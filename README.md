# 42 - LIBFT PROJECT

### Introduction
C programming can be very tedious when one doesn't have access to those highly useful standard functions. This project allows you to re-write those functions, understand them, and learn to use them. This library will help you with all your future C projects. Take the time to expand your libft throughout the year. But always, make sure to check which functions are allowed!

## Mandatory Part
### Part 1 - Libc Functions
You must re-code a set of the libc functions, as defined in their manual. Your functions will need to present the same prototype and behaviors as the originals. Your functions' names must be prefixed by "ft_".

### Part 2 - Additional Functions
You must code a set of functions that are either not included in the libc, or included in a different form.

### Technical Considerations
* It is forbidden to declare global variables
* If you need sub-functions to write a complex function, you should define these sub-functions as static to avoid publishing them with your library
* Every .c file must compile with the flags -Wall -Wextra -Werror
* You must use the command ar to create your library, using the command libtool is forbidden

## Bonus Part
Having functions to manipulate memory and strings is very useful, but you'll soon discover that having functions to manipulate lists is even more useful. You'll use the following structure to represent the elements of your list. This structure must be added to your libft.h file.

```
typedef struct  s_list
{
    void            *content;
    struct s_list   *next;
}               t_list;
```
Here is a description of the fields in the t_list struct:
* content = the data contained in the element. The void * allows to store any kind of data
* next = the next element's address or NULL if it's the last element
