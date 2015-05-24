# Bsz2-tételek
Tételek a BME-VIK SZIT által tanított Bevezetés a Számításelméletbe 2. (VISZIAA01) tárgyához.

# Build-elés és "fejlesztés"
A build-hez a XeLaTeX engine-t használd, a kimenet tetszőleges lehet (PDF target a leggyakoribb).
IDE-nek a TeXstudio-t ajánlom, és a LaTeX fejlesztői eszközöket pedig a TeXlive disztribúció keretében lehet a legkönnyebben beszerezni.

A teljes tételsor, valamint a tételek egyesével való legenerálásához érdemes használni a make_all.sh bash script-et, ami legenerálja és berakja ezeket a pdfs/ kimeneti könyvtárba, valamint feltakarít maga után.

# Dependency-k
A következő csomagok szükségesek ahhoz, hogy a .tex fájlok sikeresen leforduljanak, ezt bemásolva terminálba ezek fel is települnek (TeXlive esetén):

    tlmgr install etoolbox tcolorbox framed polyglossia hyperref

# Stílusok
- Definíciók: 
A definíciókhoz a [[framed]](http://www.ctan.org/pkg/framed) csomag **shaded** környezetét használjuk. 
- Tételek, állítások, lemmák: 
Ezekhez szintúgy a [framed] csomag egy környezetét, méghozzá a **framed** környezetet használjuk.
- Bizonyítások: 
A [framed] csomag **leftbar** környezetét használjuk ezekhez.
