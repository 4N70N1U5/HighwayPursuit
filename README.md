# Highway Pursuit <br/> <sup>Proiect pentru materia *Dezvoltarea Jocurilor cu Unreal Engine 5*</sup> <br/> <sup>Nitoi Antonio, grupa 334</sup>

Acest joc este unul de tip **infinite runner**, in care jucatorul se afla la volanul unei masini vazuta din spate si va trebui sa se mute de pe o banda pe alta, alegand-o pe cea fara obstacole (alte masini, drum in lucru etc.). De asemenea, jucatorul este urmarit de raufacatori, care din cand in cand se vor apropia, jucatorul fiind nevoit sa se apere de ei inainte ca acestia sa-l poata lovi, astfel oprind jocul. Pentru a se apara, jucatorul se va putea folosi de anumite obstacole, dar masina lui va fi de asemenea dotata cu diverse gadget-uri pe care le va putea folosi pe baza de cooldown si/sau colectare de pe traseu pe parcursul jocului. Jocul va respecta principiile de baza ale categoriei infinite runner: jocul nu poate fi castigat, dar se poate urmari un high score cat mai mare, pe masura ce se inainteaza jocul se va mai misca mai rapid, obstacolele din fata vor fi randomizate (optional: la anumite praguri de scor, se vor putea debloca masini noi, peisaje etc.).

<details>
  <summary><strong>Etapa 0</strong> (total punctaj: 0.5)</summary>
  Descrierea completa a jocului pentru Etapa 0 a proiectului se poate gasi in fisierul Game Description.pdf sau la https://docs.google.com/document/d/1QC1xHeXg0w3rSEy4PTKirOwJG91gTw2B5ftVRt3DVQc/edit?usp=sharing
</details>

<details>
  <summary><strong>Etapa 1</strong> (total punctaj: 0.7)</summary>
  Cerinte rezolvate:
  <ul>
    <li>(0.05) În scenă trebuie să existe un teren. Nu este obligatorie deplasarea pe teren, poate servi drept peisaj în jurul platformei de joc</li>
    <li>TODO (0.15) Terenul trebuie să aibă un relief variat(să existe multiple zone joase și înalte). Terenul va avea alocat un material ce cuprinde multiple (minim 3) texturi (de exemplu, textură de iarbă, de nisip, de rocă etc). Texturile asociate trebuie pictate pe teren astfel încât să fie în concordanță cu forma terenului (de exemplu o groapă adâncă va avea textură de rocă și nu cu iarbă/floricele)</li>
    <li>TODO (0.05) Pe teren trebuie să existe minim o rampă (meniul Sculpt-> ramp)</li>
    <li>TODO (0.05) Pe teren trebuie să existe două zone simetrice (de exemplu doi munți) (vezi meniul Sculpt-> mirror)</li>
    <li>(0.05) Obiect cu material transparent - <code>M_TintedGlass</code> </li>
    <li>(0.05) Obiect cu luciu metalic care reflectă mediul înconjurător - <code>M_Chrome</code> </li>
    <li>(0.05) Existența unui obiect cu culoare emissivă - <code>M_Headlights</code> + <code>M_Taillights</code></li>
    <li>(0.2) Simularea unei culori cu sclipici (puncte sclipitoare dispuse în mod aleator) folosind un nod de zgomot și fără folosirea unei texturi externe (adică a unei imagini) - <code>M_EnemyCarPaint</code></li>
    <li>(0.05) Folosirea unui normal map pentru a crea un obiect care dă senzația că are asperități chiar dacă nu și-a modificat vertecșii - <code>Texturile pentru Landscape</code></li>
  </ul>
</details>

<details>
  <summary><strong>Etapa 2</strong> (total punctaj: 0.9-0.95)</summary>
  Cerinte rezolvate:
  <ul>
    <li>(0.1) Realizare pion prin extinderea clasei Pawn sau DefaultPawn - <code>PlayerCar</code></li>
    <li>(0.05) Pionul/caracterul va avea o cameră (de înregistrare) adăugată în components pentru a urmări pionul în stil first person sau third person. - <code>PlayerCar</code></li>
    <li>(0.15) Posibilitatea de a schimba din urmărirea first person în third person prin apăsarea unei taste. - <code>Project Settings > Input</code> + <code>PlayerCar</code></li>
    <li>(0.1) Pionul/caracterul trebuie să aibă mișcările pe axe (Axis Mappings) definite în inputs din Project Settings.</li>
    <ul><li>(0.1) Se adună la punctaj dacă se poate translata pe minim 2 axe definite astfel - <code>PlayerCar</code></li></ul>
    <li>(0.1) Pionul/caracterul își poate schimba (mări/micșora) viteza de deplasare - <code>PlayerCar</code></li>
    <li>(0.05-0.1) Un sistem de calculare a scorului. În funcție de realizările în joc se va calcula un număr care să arate cât de bine s-a descurcat jucătorul. - <code>PlayerCar</code></li>
    <li>(0.25) Se va implementa sistemul implicit de damage din Unreal fie asupra pionului/caracterului fie asupra actorilor cu care interacționează jucătorul. Se va folosi metoda ApplyDamage în urma unui eveniment din joc. Cu ajutorul unui eveniment AnyDamage actorul asupra căruia se aplică distrugerea va avea niste parametri afectați. Se va implementa un caz pentru o distrugere cu valoare mică (obiectul își poate schimba culoarea, se poate micșora etc) și un altul pentru o distrugere cu valoare mare (de exemplu obiectul poate să dispară sau să își schimbe culoarea în mod diferit față de damage-ul mic, sau să oferim un mesaj scris pe ecran). - <code>PlayerCar</code></li>
  </ul>
</details>

<details>
  <summary><strong>Etapa 3</strong> (total punctaj: )</summary>
  Cerinte rezolvate:
  <ul>

  </ul>
</details>

<details>
  <summary><strong>Etapa 4</strong> (total punctaj: 0.35)</summary>
  Cerinte rezolvate:
  <ul>
    <li>(0.05) Coordonate,rotații și/sau dimensiuni aleatoare pentru unul sau mai multe obiecte sau pion/caracter - <code>TrafficCones > RotateCones</code></li>
    <li>(0.3) Comportamente determinate probabilist (0.3 pentru 3 probabilitati). Exemplu: cu o probabilitate de  20% să se genereze elemente de culoare c1, cu o probabilitate de 30% culoare c2 și restul de culoare c3. Se poate alege orice element care să depindă de probabilitate (culoare, locație, formă, tipul de obiect, acțiune desfășurată etc.) - <code>RoadTile > SpawnObstacle</code></li>
  </ul>
</details>

<details>
  <summary><strong>Etapa 5</strong> (total punctaj: )</summary>
  Cerinte rezolvate:
  <ul>

  </ul>
</details>

<details>
  <summary><strong>Etapa 6</strong> (total punctaj: )</summary>
  Cerinte rezolvate:
  <ul>

  </ul>
</details>

<details>
  <summary><strong>Etapa 7</strong> (total punctaj: )</summary>
  Cerinte rezolvate:
  <ul>

  </ul>
</details>

<details>
  <summary><strong>Etapa 10</strong> (total punctaj: )</summary>
  Cerinte rezolvate:
  <ul>

  </ul>
</details>
