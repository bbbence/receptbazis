## **1. Az alkalmazás célja**

Az alkalmazás feladata, hogy egy receptek megosztására, kommentelésére, és értékelésére alkalmas közösségi felületet nyújtson, melyben a felhasználó ill. az adminisztrátor képes a feltöltött receptek kezelésére, szerkesztésére és nyilvántartására.

## **2. Az alkalmazás telepítése**

- A célgépre klónozza le a https://github.com/bbbence/receptbazis repository tartalmát
- Telepítse a függőségeket az `npm i` parancs segítségével
- Amennyiben szükséges, telepítse az Angular keretrendszert az `npm i -g @angular/cli` paranccsal

## **3. Az alkalmazás konfigurálása**

Állítsa be az API végpont elérési útvonalát a _base.service.ts_ állományban.

## **4. Az alkalmazás indítása**

Indítsa el a megadott Docker containert.

## **5. A végpontok dokumentációja**

1. GET /api/user (- felhasználó lista lekérése)

2. POST /api/user (- felhasználó létrehozása)

3. GET /api/user/<id> (- egy bizonyos felhasználó lekerese Id alapján)

4. PUT /api/user/<id> (- felhasználó updatelése)

5. DELETE /api/user/<id>  (- felhasználó törlése Id alapján)

6. GET /api/recipe/<receptId>/comments  (- egy recepthez tartozó összes komment listázása)

7. DELETE /api/recipe/<receptId>/comments/<kommentId> (- egy komment törlése Id alapján)

8. PUT /api/recipe/<receptId>/comments/<kommentId>  (- egy komment szerkesztése Id alapján) 

9. POST /api/recipe/<receptId>/comments/<kommentId> (- új komment létrehozása)

10. GET /api/tag (- összes címke listázása)

11. POST /api/tag (- új címke létrehozása)

12. PUT /api/tag/<id> (- címke szerkesztése Id alapján)

13. DELETE /api/tag/<id> (- címke törlése Id alapján)

14. GET /api/rating/ (-összes értékelés listázása)

15. GET /api/recipe/<receptId>/ratings  (- a recepthez tartozó értékelés lekérése)

16. POST /api/recipe/<receptId>/ratings/ratingId> (- egy új értékelés létrehozása)

17. PUT /api/recipe/<receptId>/ratings/ratingId> (- egy értékelés szerkesztése Id alapján)

18. DELETE /api/recipe/<receptId>/ratings/ratingId> (- egy értékelés törlése Id alapján)
