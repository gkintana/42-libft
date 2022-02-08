# ⚠️ WARNING ⚠️
Please refrain from using my Makefile as a reference since it needs to be revised.

# 42 - FT_PRINTF PROJECT 

### Introduction
The versatility of the printf function in C represents a great exercise in programming for us. This project is of moderate difficulty. It will enable you to discover variadic functions in C.

## Mandatory Part
A brief description of the required conversions:
* %c print a single character
* %s print a string of characters
* %p the void * pointer argument is printed in hexadecimal
* %d print a decimal (base 10) number
* %i print an integer in base 10
* %u print an unsigned decimal (base 10) number
* %x print a number in lowercase hexadecimal (base 16)
* %X print a number in uppercase hexadecimal (base 16)
* %% print a percent sign

Complete references can be found in: **man 3 printf / man 3 stdarg**

### Technical Considerations
* The prototype of ft_printf should be **int ft_printf(const char \*, ...);**
* You have to recode the libc's printf function
* It must not do the buffer management like the real printf
* It will manage the following conversions: cspdiuxX\%
* It will be compared with the real printf
* You must use the command ar to create your library, using the command libtool is forbidden

## Bonus Part
* Manage any combination of the following flags '-0.' and minimum field width with all conversions
* Manage all the following flags: '# +' (yes, one of them is a space)


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
