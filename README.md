Sebastian Cojocariu 311CB UPB ACS

			              	Eigenvalues and eigenvectors

1)Calculam valorile lui lambda in polinoamele construite(polinoame Sturm),cu mentiunea ca indicele incepe de la 1 si nu de la 0(Conform relatiei de recurenta data)
2)Generam vectorul de valori pentru valoarea lambda data.De fiecare daca cand semnul a 2 termeni alaturati e diferit sau cel de dupa el e 0 incrementam numvp.
3)Calculam vectorul t care retine suma valorilor absolute(fara elementul de pe diag principala) pentru fiecare linie a matricei.Luam primele valori pentru limite.Cu o singura parcurgere verificam daca limitele sunt cele mai bine(daca sunt cele mai mici,respectiv cele mai mari),altfel le schimbam.
4)Daca m e mai mare ca dimeniunea lui d il facem pe m=length(d).Apelam functia LimiteValProprii pentru matricea data.Se scrie algoritmul conform indicatiei de rezolvare.La sfarsit stergem ultimul element(cel pe care l am folosit doar pt a-l genera pe r(m+1)).
5)Generam intervalele in care se gasesc primele m valori proprii.Daca m <length(d)=>m=length(d).pentru fiecare interval consecutiv( adica (r(i),r(i+1))) luam mijlocul intervalului,generam valoarea P_n(mij) si in functie de pozitia fata de 0 schimbam r(i) sau r(i+1) cu mij.Procedeul se repeta pana cand s-a atins toleranta.OBS:nu lucram direct pe vectorul r,ci ne trebuie un alt vector intrucat pot exista erori la trecerea de la un interval la altul.
6)Se creeaza functiile inmultire care genereaza vectorul coloana dat de inmultirea unei matrici tridiagonale simetrice cu un vector coloana,cat si Thomas care rezolva un sistem tridiagonal .
Se urmaresc pasii pseudocod din lab07 pentru calcularea puterii inverse,functie numita PutereInv
