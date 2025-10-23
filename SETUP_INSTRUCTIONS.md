# GitHub Pages Setup Instructions

**Tavoite:** Julkaista Privacy Policy GitHub Pagesissa App Store Connectia varten

**Arvioitu aika:** 15-20 minuuttia

---

## VAIHE 1: Luo uusi GitHub repository (5 min)

### 1.1 Mene GitHubiin
Avaa selaimessa: https://github.com/new

### 1.2 Täytä repo-tiedot

**Repository name:**
```
wavegod-spatial-docs
```

**Description:**
```
Documentation and privacy policy for Wavegod Spatial
```

**Visibility:**
- ⚠️ **Valitse:** **Public** (pakollinen GitHub Pagesille!)

**Initialize this repository:**
- ✅ **Valitse:** Add a README file

**Muut asetukset:**
- .gitignore: None
- License: None (tai MIT jos haluat)

### 1.3 Luo repo
Klikkaa **"Create repository"** nappia

---

## VAIHE 2: Lisää tiedostot repoon (5 min)

### Tapa A: Web UI (HELPOIN - suositeltu)

1. **Avaa juuri luomasi repo GitHubissa**
   - URL: `https://github.com/TipiusMaximus/wavegod-spatial-docs`

2. **Klikkaa "Add file" → "Upload files"**

3. **Raahaa KAIKKI tiedostot** `docs-repo-files/` kansiosta:
   ```
   ☑️ README.md
   ☑️ index.md
   ☑️ privacy.md
   ☑️ _config.yml
   ```

   **HUOM:** ÄLÄ raahaa tätä SETUP_INSTRUCTIONS.md tiedostoa!

4. **Commit message:**
   ```
   Add privacy policy and documentation
   ```

5. **Klikkaa "Commit changes"**

### Tapa B: Git Command Line (jos osaat)

```bash
# Kloonaa repo
cd ~/Documents  # tai mihin haluat
git clone https://github.com/TipiusMaximus/wavegod-spatial-docs.git
cd wavegod-spatial-docs

# Kopioi tiedostot (paitsi SETUP_INSTRUCTIONS.md)
cp "/Volumes/Timon ssd 2/07_SEKALAISET/wavegod_spatial/WavegodSpatial_Clean/docs-repo-files/README.md" .
cp "/Volumes/Timon ssd 2/07_SEKALAISET/wavegod_spatial/WavegodSpatial_Clean/docs-repo-files/index.md" .
cp "/Volumes/Timon ssd 2/07_SEKALAISET/wavegod_spatial/WavegodSpatial_Clean/docs-repo-files/privacy.md" .
cp "/Volumes/Timon ssd 2/07_SEKALAISET/wavegod_spatial/WavegodSpatial_Clean/docs-repo-files/_config.yml" .

# Commit ja push
git add .
git commit -m "Add privacy policy and documentation"
git push
```

---

## VAIHE 3: Aktivoi GitHub Pages (3 min)

1. **Mene repo Settings**
   - Klikkaa "Settings" välilehteä (repon yläreunassa)

2. **Valitse Pages vasemmalta**
   - Vasen sidebar → "Pages"

3. **Konfiguroi Pages:**

   **Source:**
   - Valitse: **Deploy from a branch**

   **Branch:**
   - Branch: **main** (tai **master** jos näkyy)
   - Folder: **/ (root)**

4. **Tallenna:**
   - Klikkaa **"Save"**

5. **Odota 2-10 minuuttia**
   - GitHub rakentaa sivustoa
   - Saat ilmoituksen kun valmis

---

## VAIHE 4: Testaa sivusto (5 min)

### 4.1 Tarkista deployment status

1. Palaa **Settings → Pages**
2. Ylhäällä näkyy:
   ```
   Your site is live at https://tipiusmaximux.github.io/wavegod-spatial-docs/
   ```

3. **Voi kestää 2-10 min** ensimmäisellä kerralla

### 4.2 Testaa URL:t

**Etusivu:**
```
https://tipiusmaximux.github.io/wavegod-spatial-docs/
```

**Privacy Policy (TÄRKEÄ - tämä menee App Storeen):**
```
https://tipiusmaximux.github.io/wavegod-spatial-docs/privacy
```

### 4.3 Tarkista sisältö

Avaa Privacy Policy URL ja varmista:
- ✅ Sivu näkyy oikein
- ✅ Email on: Timo.Aula@boethius.fi
- ✅ GitHub linkki on: https://github.com/TipiusMaximus/wavegod-spatial-docs
- ✅ Kaikki tekstit ovat selkeät
- ✅ Ei näy erikoismerkkejä tai virheitä

---

## VAIHE 5: Kopioi URL App Store Connectiin

### Privacy Policy URL (App Store Connect):

```
https://tipiusmaximux.github.io/wavegod-spatial-docs/privacy
```

**Missä käytetään:**
1. App Store Connect → App Information → Privacy Policy URL
2. Liitä tämä URL siihen kenttään

---

## Troubleshooting

### Jos sivu ei näy (404 error):

1. **Tarkista GitHub Pages status:**
   - Settings → Pages
   - Katso että "Your site is published at..." näkyy

2. **Odota pidempään:**
   - Ensimmäinen deployment voi kestää 10 min
   - Päivitykset yleensä 1-2 min

3. **Tarkista Branch:**
   - Settings → Pages
   - Varmista että branch on "main" (ei "master")

4. **Tarkista URL:**
   - GitHub username: TipiusMaximus (iso T!)
   - Repo name: wavegod-spatial-docs (tarkka kirjoitusasu)

### Jos muotoilu näyttää oudolta:

1. **Tarkista _config.yml:**
   - Tiedoston pitää olla mukana
   - Tarkista että theme: jekyll-theme-minimal

2. **Odota hetki:**
   - GitHub Pages päivittää teemat viiveellä

3. **Hard refresh:**
   - Cmd+Shift+R (Mac)
   - Ctrl+Shift+R (Windows)

### Jos tiedostot puuttuvat:

1. **Tarkista että kaikki ladattiin:**
   - Mene repoon GitHubissa
   - Tarkista että näet: README.md, index.md, privacy.md, _config.yml

2. **Jos puuttuu:**
   - Lataa uudelleen: Add file → Upload files

---

## Päivitykset tulevaisuudessa

Kun haluat päivittää Privacy Policya:

1. **Muokkaa alkuperäistä:**
   ```
   /Volumes/Timon ssd 2/07_SEKALAISET/wavegod_spatial/WavegodSpatial_Clean/PRIVACY_POLICY.md
   ```

2. **Kopioi muutokset docs-repo-files/privacy.md:ään**

3. **Päivitä GitHubissa:**
   - Tapa A: Web UI → privacy.md → Edit file → Commit
   - Tapa B: Git push

4. **Odota 1-2 min** → Päivitys näkyy sivustolla

---

## Seuraavat askeleet projektin julkaisussa

✅ Privacy Policy julkaistu → VALMIS!

Seuraavaksi:

1. ⏳ **Team ID päivitys** (Configuration.storekit)
2. ⏳ **App Icon tarkistus** (1024x1024)
3. ⏳ **Build & Archive** (iOS + macOS)
4. ⏳ **App Store Connect** setup

---

## Tuki

Jos ongelmia:
1. Tarkista että repo on **Public**
2. Tarkista että Pages on **enabled**
3. Odota 10 min ja refresh
4. Jos ei vieläkään toimi, lue GitHub Pages docs: https://pages.github.com

---

**Onnea julkaisuun!** 🚀

Privacy Policy URL App Storeen:
```
https://tipiusmaximux.github.io/wavegod-spatial-docs/privacy
```
