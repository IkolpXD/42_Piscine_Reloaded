# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: made-jes <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/10/26 18:00:35 by made-jes          #+#    #+#              #
#    Updated: 2024/10/27 11:35:06 by made-jes         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SOURCES = ft_display_file.c

OBJECTS := $(SOURCES: .c=.o)

NAME = ft_display_file

CC = gcc

CCFLAGS = -Wall -Werror -Wextra

HEADER = ft_display_file.h

all: $(NAME)

$(NAME): $(OBJECTS) $(HEADER)
	$(CC) $(CCFLAGS) -o $(NAME) $(OBJECTS)
	chmod +x $(NAME)

%.o: %.c
	$(CC) $(CCFLAGS) -o $@ -c $<

clean:
	rm -f *.o

fclean: clean
	rm -f $(NAME)

re: fclean all
