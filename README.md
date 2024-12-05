#include <iostream>
using namespace std;

int main()
{
	char nota;

	do {
		cout << "--- Menu de Notas ---" << endl;
		cout << "1. Ingresar una nota (A-E)" << endl;
		cout << "2. Salir" << endl;
		cout << "Seleccionar una opcion: ";
		int opcion;
		cin >> opcion;

		if (opcion == 1) {
			cout << "Ingrese la nota (A-E): ";
			cin >> nota;
			if (nota >= 'A' && nota <= 'E') {
				switch (nota) {
				case 'A':
					cout << "Muy bien " << endl;
					break;
				case 'B':
					cout << "Bueno" << endl;
					break;
				case 'C':
					cout << "Regular" << endl;
					break;
				case 'D':
					cout << "Malo" << endl;
					break;
				case 'E':
					cout << "Muy Malo" << endl;
					break;
				}
			} else {
				cout << "Opcion equivocada. Ingresa una nota valida (A-E)." << endl;
			}
		} else if (opcion == 2) {
			cout << "Saliendo del programa..." << endl;
			break;
		} else {
			cout << "Opcion no valida, intenta de nuevo." << endl;
		}

	} while (true);

	return 0;
}
