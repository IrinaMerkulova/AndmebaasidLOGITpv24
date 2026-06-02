## SQL protseduur  -

[Põhimõisted](README.md) | [Kasutajad](kasutaja.md) | [Trigerid](triger.md) | [Protseduurid](protseduurid.md) | [Võtmed/Keys].(kodutoo.md)

store procedure - salvestatud protseduurid - sama mis on funktsioonid programmeerimises, mingi tegevus, mis 
on salvestatud andmebaasi, ja mida saab automaatselt teha (INSERT, UPDATE, SELECT, UPDATE).
```sql
CREATE Procedure lisaKategooria
--parameetrid @...
@uusKategooria varchar(30)
AS
BEGIN
--kirjeldus
	INSERT INTO categories(category_name)
	VALUES (@uusKategooria);
	SELECT * FROM categories;
END;
```
<img width="318" height="271" alt="{05494122-D65F-4960-B0E4-2A7E6EC3A81C}" src="https://github.com/user-attachments/assets/e509f74e-7207-4ff4-b303-91b936e50834" />

<img width="499" height="219" alt="{A619FFA0-82B1-4864-BFEB-7EB616F0ED3E}" src="https://github.com/user-attachments/assets/b3e2b637-174b-4305-b593-cbe05ff36d41" />


