# Lab1

#include "stdafx.h"
#include <string>
#include <iostream>
#include <conio.h>

using namespace std;

/* ������� ��� ������ */
typedef struct _baseType {

	char fname[20]; //������� � �������� 	
	char group[20]; //������	
	int bal[5]; //������		

} baseType;

/* ��������� ���� ������ */
typedef struct _Node {

	baseType field; // ���� ������
	struct _Node *next; // ��������� �� ��������� �������
	struct _Node *prev; // ��������� �� ���������� �������

} Node;

/* ��������� ����������� ������ */
typedef struct _dblList {
	int size; //���������� ��������� ������
	Node *head; //��������� �� ������ ������
	Node *tail; //��������� �� ����� ������
} dblList;
