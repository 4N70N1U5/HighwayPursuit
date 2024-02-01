# Highway Pursuit <br/> <sup>Proiect pentru materia *Dezvoltarea Jocurilor cu Unreal Engine 5*</sup> <br/> <sup>Nitoi Antonio, grupa 334</sup>

Acest joc este unul de tip **infinite runner**, in care jucatorul se afla la volanul unei masini vazuta din spate si va trebui sa se mute de pe o banda pe alta, alegand-o pe cea fara obstacole (alte masini, drum in lucru etc.). De asemenea, jucatorul este urmarit de raufacatori, care din cand in cand se vor apropia, jucatorul fiind nevoit sa se apere de ei inainte ca acestia sa-l poata lovi, astfel oprind jocul. Pentru a se apara, jucatorul se va putea folosi de anumite obstacole, dar masina lui va fi de asemenea dotata cu diverse gadget-uri pe care le va putea folosi pe baza de cooldown si/sau colectare de pe traseu pe parcursul jocului. Jocul va respecta principiile de baza ale categoriei infinite runner: jocul nu poate fi castigat, dar se poate urmari un high score cat mai mare, pe masura ce se inainteaza jocul se va mai misca mai rapid, obstacolele din fata vor fi randomizate (optional: la anumite praguri de scor, se vor putea debloca masini noi, peisaje etc.).

<details>
  <summary><strong>Etapa 0</strong> (total punctaj: 0.5)</summary>
  Descrierea completa a jocului pentru Etapa 0 a proiectului se poate gasi in fisierul Game Description.pdf sau la https://docs.google.com/document/d/1QC1xHeXg0w3rSEy4PTKirOwJG91gTw2B5ftVRt3DVQc/edit?usp=sharing
</details>

<details>
  <summary><strong>Etapa 1</strong> (total punctaj: 0.5)</summary>
  Cerinte rezolvate:
  <ul>
    <li>(0.05) În scenă trebuie să existe un teren. Nu este obligatorie deplasarea pe teren, poate servi drept peisaj în jurul platformei de joc</li>
    <li>(0.15) Terenul trebuie să aibă un relief variat(să existe multiple zone joase și înalte). Terenul va avea alocat un material ce cuprinde multiple (minim 3) texturi (de exemplu, textură de iarbă, de nisip, de rocă etc). Texturile asociate trebuie pictate pe teren astfel încât să fie în concordanță cu forma terenului (de exemplu o groapă adâncă va avea textură de rocă și nu cu iarbă/floricele)</li>
    <li>(0.05) Pe teren trebuie să existe minim o rampă (meniul Sculpt-> ramp)</li>
    <li>(0.05) Pe teren trebuie să existe două zone simetrice (de exemplu doi munți) (vezi meniul Sculpt-> mirror)</li>
    <li>(0.05) Obiect cu material transparent</li>
    <li>(0.05) Obiect cu luciu metalic care reflectă mediul înconjurător</li>
    <li>(0.05) Existența unui obiect cu culoare emissivă</li>
    <li>(0.05) Folosirea unui normal map pentru a crea un obiect care dă senzația că are asperități chiar dacă nu și-a modificat vertecșii</li>
  </ul>
</details>

<details>
  <summary><strong>Etapa 2</strong> (total punctaj: 0.45)</summary>
  Cerinte rezolvate:
  <ul>
    <li>(0.1) Realizare pion prin extinderea clasei Pawn sau DefaultPawn</li>
    <li>(0.05) Pionul/caracterul va avea o cameră (de înregistrare) adăugată în components pentru a urmări pionul în stil first person sau third person.</li>
    <li>(0.1) Pionul/caracterul trebuie să aibă mișcările pe axe (Axis Mappings) definite în inputs din Project Settings.</li>
    <ul><li>(0.1) Se adună la punctaj dacă se poate translata pe minim 2 axe definite astfel</li></ul>
    <li>(0.1) Pionul/caracterul își poate schimba(mări/micșora) viteza de deplasare</li>
  </ul>
</details>
