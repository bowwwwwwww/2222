#include <iostream>
#include "Board.cpp"
using namespace std;
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	Board brd;
	brd.Startgame();
	brd.display();
	return 0;
#ifndef BOARD_H
#define BOARD_H
#include "figure.cpp"

	class Board
	{
	public:
		void Startgame();
		void MoveFi();
		void display();
		figure brd[10][10];
	protected:
		int firstturn;

	};

#endif
#include "Board.h"
#include "figure.cpp"

	void Board::Stratgame() {
		int ch = 1;
		for (int x = 0; x < Brd.lenght(); x++0) {
			for (int y = 0; y < brd.lenght(); y++) {
				if (ch == 1) {
					brd[x][y].figure("@", x, y);
					ch = 0;
				}
				else {
					brd[x][y].figure("#", x, y);
					ch = 1;
				}

			}
		}

	}

	void Board::display() {
		printf(" 1 2 3 4 5 6 7 8 9 10");
		printf("_____________________")
			for (int y = 1; y <= 10; y++) {
				printf("%d|", x);
				for (int x = 0; x <= 9; x++) {
					printf("%c", brd[y - 1][x].getName())
						if ((y - 1 == 0 && x == 0 || y - 1 == 9 && x == 0 || y - 1 == 4 && x == 4 || y - 1 == 4 && x == 5 || y - 1 == 5 && x == 4 || y - 1 == 5 && x == 5 || y - 1 == 9 && x == 0 || y - 1 == 9 && x == 9) && this->firstturn == 1) {
							printf(System("COLOR 06"));
						}
				}
			}
	}

	void
#ifndef FIGURE_H
#define FIGURE_H
#include "figure.cpp"
		using namespace std;


	class figure
	{
	protected:
		char team;
		int PX, PY;

	public:
		void Figure(char name, int x, int y);
		void Move(int posision);
		void setTeam(char name);
		char getName();

	};

#endif
#include "figure.h"
#include <iostream>
	using namespace std;
	void figure::Figure(char name, int x, int y) {
		this->team = name;
		this->PX = X;
		this->PY = Y;
		return 0;
	}

	char figure::getName() {
		return this.team;
	}
}

