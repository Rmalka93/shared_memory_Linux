# shared_memory_Linux
The Buffering Problem - Shared Memory

==Description==

This program is a basic calculator for polynoms implemented in C that can run commands entered by the user
Program DATABASE:
struct database that contain the shared mem and the threads


This program performs various operations on polynomials, including addition, multiplication, and printing the result. It also includes functionality to store polynomials in shared memory and perform operations using threads


The program defines several functions

copyUntilColon(const char* source, char* destination): Copies characters from source string to destination string until a colon (':') is encountered. The copied string is null-terminated.

convertToIntArray(const char* ch, int* num): Converts a string of characters ch representing a polynomial to an array of integers num.

add(const int* pol1, const int* pol2, int* resPolt, int pol1Lent, int pol2Lent): Performs addition of two polynomials pol1 and pol2 and stores the result in the array resPolt. pol1Lent and pol2Lent indicate the lengths of the respective polynomials.

mul(const int* pol1, const int* pol2): Performs multiplication of two polynomials pol1 and pol2 and prints the result.

printPol(int* res): Prints the coefficients of a polynomial stored in the array res.

generattor(char* cmd): Generates a command for storing polynomials in shared memory based on the provided cmd.

subThread(void* arg): Thread function that subtracts two polynomials and print the result.

addThread(void* arg): Thread function that adds two polynomials and print the result 
