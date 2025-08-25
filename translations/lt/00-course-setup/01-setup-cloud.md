<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "5cd64c01065daed468d900608612932a",
  "translation_date": "2025-08-25T12:19:46+00:00",
  "source_file": "00-course-setup/01-setup-cloud.md",
  "language_code": "lt"
}
-->
# Debesų nustatymas ☁️ – GitHub Codespaces

**Naudokite šį vadovą, jei nenorite nieko diegti savo kompiuteryje.**  
Codespaces suteikia nemokamą, naršyklėje veikiančią VS Code aplinką su visomis iš anksto įdiegtomis priklausomybėmis.

---

## 1.  Kodėl Codespaces?

| Privalumas | Ką tai reiškia jums |
|------------|---------------------|
| ✅ Jokio diegimo | Veikia Chromebook, iPad, mokyklos kompiuteriuose ir pan. |
| ✅ Paruoštas kūrimo konteineris | Python 3, Node.js, .NET, Java jau įdiegta |
| ✅ Nemokamas limitas | Asmeniniai paskyros gauna **120 branduolių valandų / 60 GB valandų per mėnesį** |

> 💡 **Patarimas**  
> Taupykite savo limitą **stabdydami** arba **ištrindami** nenaudojamus codespaces  
> (View ▸ Command Palette ▸ *Codespaces: Stop Codespace*).

---

## 2.  Sukurkite Codespace (vienu paspaudimu)

1. **Fork’inkite** šį repozitoriją (viršuje dešinėje mygtukas **Fork**).  
2. Savo fork’e spauskite **Code ▸ Codespaces ▸ Create codespace on main**.  
   ![Dialogas su mygtukais codespace kūrimui](../../../00-course-setup/images/who-will-pay.webp)

✅ Atsidarys naršyklės VS Code langas ir pradės kurtis kūrimo konteineris.
Pirmą kartą tai užtrunka **apie 2 minutes**.

## 3. Pridėkite savo API raktą (saugus būdas)

### A variantas Codespaces Secrets — Rekomenduojama

1. ⚙️ Pavarėlės ikona -> Command Pallete-> Codespaces : Manage user secret -> Add a new secret.
2. Pavadinimas: OPENAI_API_KEY
3. Reikšmė: įklijuokite savo raktą → Add secret

Viskas—mūsų kodas jį automatiškai suras.

### B variantas .env failas (jei tikrai reikia)

```bash
cp .env.copy .env
code .env         # fill in OPENAI_API_KEY=your_key_here
```

---

**Atsakomybės atsisakymas**:  
Šis dokumentas buvo išverstas naudojant dirbtinio intelekto vertimo paslaugą [Co-op Translator](https://github.com/Azure/co-op-translator). Nors siekiame tikslumo, prašome atkreipti dėmesį, kad automatiniai vertimai gali turėti klaidų ar netikslumų. Originalus dokumentas jo gimtąja kalba turėtų būti laikomas autoritetingu šaltiniu. Kritinei informacijai rekomenduojame profesionalų žmogaus vertimą. Mes neatsakome už nesusipratimus ar neteisingą interpretavimą, kilusį naudojantis šiuo vertimu.