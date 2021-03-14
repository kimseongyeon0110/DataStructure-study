#include <stdio.h>
#include <stdlib.h>

int main(int argc, const char* argv[]) {
   
    int row, column;
    int i, j, k;
    printf("이차원 배열 동적 코드 할당 작성\n");
    printf("가로 : ");
    scanf("%d", &column);
    printf("세로 : ");
    scanf("%d", &row);


    int** image = (int**)malloc(sizeof(int*) * column);

    if (image == NULL) {
        exit(1);
    }

    for (i = 0; i < column; i++) {
        *(image + i) = (int*)malloc(sizeof(int) * row);
    }

    for (i = 0; i < column; i++) {
        for (j = 0; j < row; j++) {
            scanf("%d", &image[i][j]);
        }
    }

    printf("========\n");
    for (i = 0; i < column; i++) {
        for (j = 0; j < row; j++) {
            printf("image[%d][%d] = %d \n", i, j, image[i][j]);
        }
    }

    for (i = 0; i < column; i++) {
        free(image[i]);
    }

    free(image);

    return 0;
}

