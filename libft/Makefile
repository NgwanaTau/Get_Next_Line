# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: thmotaun <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2017/08/14 11:29:18 by thmotaun          #+#    #+#              #
#    Updated: 2017/09/16 16:10:18 by thmotaun         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME		:= libft.a

CC			:=	gcc
CFLAGS		+= -Wall -Wextra -Werror
CFLAGS		+= -I includes

SRC			:=	ft_abs.c\
				ft_atoi.c\
				ft_bzero.c\
				ft_isalnum.c\
				ft_isalpha.c\
				ft_isascii.c\
				ft_isdigit.c\
				ft_isprint.c\
				ft_itoa.c\
				ft_lstadd.c\
				ft_lstdel.c\
				ft_lstdelone.c\
				ft_lstiter.c\
				ft_lstmap.c\
				ft_lstnew.c\
				ft_memalloc.c\
				ft_memccpy.c\
				ft_memchr.c\
				ft_memcmp.c\
				ft_memcpy.c\
				ft_memdel.c\
				ft_memmove.c\
				ft_memset.c\
				ft_putchar.c\
				ft_putchar_fd.c\
				ft_putendl.c\
				ft_putendl_fd.c\
				ft_putnbr.c\
				ft_putnbr_fd.c\
				ft_putstr.c\
				ft_putstr_fd.c\
				ft_strcat.c\
				ft_strchr.c\
				ft_strclr.c\
				ft_strcmp.c\
				ft_strcpy.c\
				ft_strdel.c\
				ft_strdup.c\
				ft_strequ.c\
				ft_striter.c\
				ft_striteri.c\
				ft_strjoin.c\
				ft_strlcat.c\
				ft_strlen.c\
				ft_strmap.c\
				ft_strmapi.c\
				ft_strncat.c\
				ft_strncmp.c\
				ft_strncpy.c\
				ft_strnequ.c\
				ft_strnew.c\
				ft_strnstr.c\
				ft_strrchr.c\
				ft_strsplit.c\
				ft_strstr.c\
				ft_strsub.c\
				ft_strtrim.c\
				ft_toupper.c\
				ft_tolower.c\
				ft_ulstr.c\

OBJ			:=	$(SRC:.c=.o)

.PHONY = all clean fclean re

all: $(NAME)

$(OBJ): %.o: %.c
		@$(CC) -c $(CFLAGS) $< -o $@

$(NAME): $(OBJ)
		@ar rcs $(NAME) $(OBJ)
		@echo "\033[32mCompiled Library\033[0m"

compile:
		@$(CC) $(CFLAGS) $(NAME)
		@echo "\033[32mCompiled Library\033[0m"

norm:
	@norminette $(NAME)

clean:
		@rm -f $(OBJ)
		@echo "\033[32mRemoved Object Files\033[0m"

fclean: clean
		@rm -f $(NAME)
		@echo "\033[32mRemoved Library\033[0m"

re: fclean all
