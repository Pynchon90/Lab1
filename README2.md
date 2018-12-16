# Lab1

#include "stdafx.h"
#include <string>
#include <iostream>
#include <conio.h>

using namespace std;

/* базовый тип списка */
typedef struct _baseType {

	char fname[20]; //фамилия и инициалы 	
	char group[20]; //группа	
	int bal[5]; //оценки		

} baseType;

/* структура узла списка */
typedef struct _Node {

	baseType field; // поле данных
	struct _Node *next; // указатель на следующий элемент
	struct _Node *prev; // указатель на предыдущий элемент

} Node;

/* структура двусвязного списка */
typedef struct _dblList {
	int size; //количество элементов списка
	Node *head; //указатель на начало списка
	Node *tail; //указатель на конец списка
} dblList;
