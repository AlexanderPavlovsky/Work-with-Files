# Work-with-Files
#include "stdafx.h"
#include <iostream>
#include <fstream>

using namespace std;

int main()
{
	char s1[100];
	FILE *file;
	fopen_s(&file, "D:\\text.txt", "r");
	fgets(s1, 100, file);
	fclose(file);
	FILE *file1;
	fopen_s(&file1, "D:\\text1.txt", "w");
	fputs(s1, file1);
	fclose(file1);
    return 0;
}
