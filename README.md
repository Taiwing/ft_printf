# ft\_printf

Implementation of printf functions in C.

## Setup

```shell
# clone this repo
git clone https://github.com/Taiwing/ft_printf.git
# build it
cd ft_printf/ && make
```

## Usage

Compile the ft\_printf library with this C program:

```C
#include "ft_printf.h"

int	main(void)
{
	ft_printf("It works!\n");
	return (0);
}
```

```shell
# compile the program
gcc -o test my_program.c -I includes/ libftprintf.a
# and run it
./test
```

## Features

This implementation handles a lot of the original *printf* conversions:

- integer: 'douxX'
- float: 'eEfFgG'
- pointer: 'pP'
- characters and strings: 'cCsS'

It also adds the binary conversions 'bB' to print integers binary representation
and the 't' conversion which prints arrays or double arrays of any printable
type.

## Development

This project is a light-weight version of ft\_printf without the full libft. The
libft functions needed for ft\_printf are located in src/libft C files with
"libft.h" as its header. There is an other version of ft\_printf in libft, that
probably will be more up to date than this one. This one should be updated with
the libft version each time it is used.
