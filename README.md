/* COMPUTER-GRAPHICS */
#include <graphics.h>
#include <conio.h>

int main() {
    int gd = DETECT, gm;
    initgraph(&gd, &gm, "");
    int centerX = 250;
    int centerY = 250;
    int radius = 150;

    circle(centerX, centerY, radius);

    int rectWidth = 200;
    int rectHeight = 100;
    int left = centerX - rectWidth / 2;
    int top = centerY - rectHeight / 2;
    int right = centerX + rectWidth / 2;
    int bottom = centerY + rectHeight / 2;

    rectangle(left, top, right, bottom);

    getch();
    closegraph();
    return 0;
}
