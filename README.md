# Punto-5.71
Further Analysis
Q.5.71 Load and run the program of Example 5.12.
format compact;

>> t = linspace(0,10*pi,200);

>> X = t;

>> Y=(-t+10*pi).*cos(t);

>> Z=3*exp(0.2*t)-3;

>> stem3(X,Y,Z)

>> xlabel(‘t’), ylabel(‘(-t+10*pi).*cos(t)’)

>> zlabel(‘3*exp(0.2*t)-3’),title(‘Stem3(X,Y,Z), 3D View’)

>> % the graph is shown in Figure 5.89

>> subplot(2,2,1); plot3(X,Y,Z)

>> grid on

>> xlabel(‘X’),ylabel(‘Y’),zlabel(‘Z’)

>> title(‘Plot3(X,Y,Z), 3D View’)

>> subplot(2,2,2); plot3(X,Y,Z); view(0,0)

>> xlabel(‘X’),zlabel(‘Z’)

>> title(‘XZ View’)

>> subplot(2,2,3); plot3(X,Y,Z); view(0,90)

>> xlabel(‘X’),ylabel(‘Y’)

>> title(‘XY View’)

>> subplot(2,2,4); plot3(X,Y,Z); view(90,0)

>> ylabel(‘Y’),zlabel(‘Z’)

>> title(‘YZ View’)
