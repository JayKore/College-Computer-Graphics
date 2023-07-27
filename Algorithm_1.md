{
    dx=x2-x1;
    dy=y2-y1;

    if(abs(dx) > abs(dy)) {

        step = dx;
    } else {
        step = dy;
    }

    Xn = dx/step;
    Yn = dy/step;

    for(i=0;i<=step;i++)
    {
        putpixel(x1,y1,RED);
        x1 = x1 + Xn;
        y1 = y1 + Yn;
    }
}
