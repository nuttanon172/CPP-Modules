NAME    =	scavtrap

CXX      =	c++

CXXFLAGS =	-Wall -Wextra -Werror -std=c++98

HEADERS     =	ClapTrap.hpp \
			ScavTrap.hpp

SRCS    =	ClapTrap.cpp \
			ScavTrap.cpp \
			main.cpp

OBJS    =	$(SRCS:.cpp=.o)

$(NAME): $(OBJS)
	$(CXX) $(CXXFLAGS) $(OBJS) -o $(NAME)

$(OBJS): $(HEADERS)

.PHONY: all clean fclean re
all: $(NAME)

clean:
	@rm -rf $(OBJS)

fclean: clean
	@rm -f $(NAME)

re: fclean all
