# GOG Blu-ray Templates

Give your favorite GOG games a case worthy of the shelf. This repository collects Krita templates and finished examples for designing custom Blu-ray case inserts for games sold on [GOG](https://www.gog.com) (Good Old Games). Whether you are building a single-game case or a bundle, these templates give you a proven layout to start from, so your insert looks like it belongs next to the official releases.

Found a template you love? Want to add your own game? Contributions are welcome. Read the requirements below before you open a pull request.

## What's in this repo

| Path | Contents |
| --- | --- |
| `Blu_Ray_Template_600dpi.kra` | Blank base template (600 dpi, 6354 x 3498) with spine guides. Start here for a new game. |
| `BluRay Inserts/` | Finished example inserts exported as PNG. |
| `Dread Templar/` | Example submission: source images, logos, and the 600 dpi Krita project. |
| `Tomb Raider Remastered 1-6/` | Example bundle submission: source images, logos, and the 600 dpi Krita project. |
| `Ratings/` | ESRB rating icons used on covers (`M.webp`, `T.webp`). |

## Getting started

1. Install [Krita](https://krita.org/) (version 6.0 or newer is recommended, since the templates were made with 6.0.x).
2. Copy `Blu_Ray_Template_600dpi.kra` or one of the existing `.kra` projects.
3. Turn on the grid. All placement measurements below are in **grid spaces**, so keep the grid visible while you work.
4. Export your finished insert and add your source files to a new folder for your game.

## Submission requirements

Every pull request must meet all of the following requirements.

### 1. The game must be on GOG

The game must be sold on [GOG](https://www.gog.com). Games that are only available on other storefronts do not qualify.

### 2. The front cover

The front cover is the most visible part of the insert, so it must follow these rules.

- **Cover image**
  - Use the main cover art of the game (or bundle).
  - If the game has no official cover art, use the title card most associated with the game.
  - **Bundles:** if no widely recognized image exists for the bundle, you may create your own. It **must** include the official title card for every game in the bundle. The title must include the game name and indicate that it is a bundle, using either `<Game Title> Bundle` or `<Game Title> X-Y` (for example, the Tomb Raider I-VI Remaster bundle).
  - The file must be named `front` with any extension, such as `front.jpg` or `front.png`.
  - The image does not need to keep its original aspect ratio, but it must be a reasonable size and shape, similar to how it would appear on an official case.
- **ESRB rating**
  - An official ESRB rating must appear on the **left side of the front cover**, in the **exact position** used on other case inserts.
  - Position: **3 grid spaces to the right of the spine** and **3 grid spaces up from the bottom** of the case.
  - The rating must keep its aspect ratio.
  - Use the rating from the `Ratings/` directory.
  - If the rating does not exist there yet, add it to `Ratings/`, named `<letter rating>.<extension>`, such as `M.webp` or `T.webp`.
  - Tip: the Tomb Raider I-VI Remaster template was built from the Dread Templar template by replacing elements in place. Place the new rating at the same position and size as the old one, then delete the old rating.
- **Publisher credits**
  - Credit publishers by placing their logos in the **bottom-right** of the case.
  - Logos must be **spaced 3 grid spaces apart**, matching Tomb Raider I-VI Remaster and Dread Templar.
  - Logos must sit **3 grid spaces from the bottom** of the case, at the same position as in the Dread Templar and Tomb Raider I-VI Remaster templates.
  - The **left-most** logo must be positioned **3 grid spaces to the left of the right edge** of the case.
  - If a logo is irregularly sized, as the Tomb Raider I-VI Remaster logos are, it should sit in a close approximate position that matches the spacing and placement rules above.
  - Name each logo `<company>_logo.png`, such as `aspyr_logo.png` or `crystal_dynamics_logo.png`.
  - Logos must be **transparent** whenever possible. Use a PNG for transparent logos. If a logo cannot be transparent, it does not need to be a PNG.
  - If a logo is meant to be transparent, make an effort to remove its background and any surrounding whitespace. Tools such as [remove.bg](https://www.remove.bg/), Krita's selection and color tools, or other image editors can help.
  - Logos must have **no watermarks**.
  - Logos must keep their aspect ratios.
  - Logos should look like the official publisher logos found on official game cases.

### 3. The spine

The spine must include the following.

- **GOG preservation logo**
  - Use the GOG game preservation logo, `gpp-logo.png`, from the root of this repository.
  - It must be a transparent PNG.
  - Place it **2 grid spaces down from the top** of the case.
  - It must span the width of the spine.
  - It must keep its aspect ratio.
- **Front image wrap**
  - The main front image must wrap around the spine until it reaches the beginning of the back of the cover.
- **Spine title**
  - The full title of the game must appear on the spine.
  - The spine title should match the front cover logo when possible.
  - It does not need to match official spine fonts or formatting, but it must remain readable.
  - Generative AI image generation is allowed for the spine title only. It is not allowed for other sections, which must use official imagery.
    - Why it is allowed: a spine title is text, not artwork, and official spine text is often a generic font that is hard to match to the front logo. Generative AI can straighten and sharpen an official title logo so it reads well on a narrow spine. The Tomb Raider I-VI Remaster template shows this workflow: the official Tomb Raider I-VI Remaster title was run through Gemini to straighten and improve it, then the background was removed to make it transparent. All other artwork stays official.
  - Use a transparent PNG for the spine title whenever possible, as the Tomb Raider I-VI Remaster template does. Remove the background as described in the publisher credits section.
  - A spine title that is not transparent is allowed if official cases or examples use the logo as the spine title, as the Dread Templar example does.
  - Name the file `<game_name>_banner.png` if it is transparent. Otherwise, feel free to use a different extension, such as `.jpg`.
  - The title is not grid strict, since spine titles vary in size. It does not need to sit a set number of grid spaces up, down, left, or right. Make an effort to center it horizontally and vertically on the spine.

### 4. The back cover

The back cover must include the following.

- **Gameplay image**
  - Use eye-catching official artwork of the game, preferably from GOG. Official gameplay screenshots are allowed.
  - This is the image shown front and center on the back. It should best describe the game and immediately hook the viewer. A main character in a strong pose (as in the Tomb Raider I-VI Remaster example) or a strong action scene (as in the Dread Templar example) both work well.
  - Name the file `gameplay.<extension>`.
  - It must not be transparent.
  - It must take up the upper half of the back cover.
- **Flavor images**
  - Include 3 flavor images, placed **1 grid space below** the gameplay image.
  - The left-most image must sit **2 grid spaces from the left edge** of the case.
  - The right-most image must sit **2 grid spaces from the start of the spine**.
  - The images must be **equidistant** from each other horizontally, roughly **12 grid spaces** apart.
  - Name the files `flavor_image<X>.<extension>`.
  - They must not be transparent.
  - They must match the size of the flavor images in the Dread Templar and Tomb Raider I-VI Remaster examples.
  - Content must be gameplay. Images from GOG are preferred.
  - Other gameplay images are allowed only if they show normal gameplay. Do not use pause screens or menus.
  - Do not include spoilers. Use generic gameplay scenes.
- **Flavor text**
  - Place the flavor text directly below the flavor images, with no grid spaces between them.
  - The text must come from GOG or from another official game description.
  - The text may be any color, but it should match the game's color scheme. For example, Dread Templar uses red to match its demon-killing themes, and Tomb Raider I-VI Remaster uses brown and tan to match its ancient, rocky temple themes.
- **System requirements**
  - Place the system requirements in their own segmented section so they have space on the back cover.
  - Source the requirements from GOG. For a bundle without GOG requirements, check each game in the bundle. If none are available, use official sources such as Steam.
  - Leave out any requirement that does not appear in the source. For example, if DirectX is not listed, do not include it.
  - **Bundles:**
    - Minimum requirements must be the lowest requirements needed to run the most demanding and most recent game in the bundle. In Tomb Raider I-VI Remaster, the most recent entry is Tomb Raider IV-VI Remaster, since the I-VI Remaster bundle includes I-III and IV-VI.
    - Recommended requirements must be the highest requirements needed to support the most recent entry.
  - Include at least one AMD graphics card and one NVIDIA graphics card in both the minimum and recommended sections. If the source lists only one brand, that is fine.
  - Other manufacturers, such as Intel, may be included if listed in the source. They are optional. Leave them out if adding them along with the NVIDIA and AMD cards makes the system requirements section too long to fit.
  - If the source lists multiple cards from the same brand, use the lowest supported card for the minimum section and the highest supported card for the recommended section.
  - Storage: if a bundle does not list storage, add up the offline installer sizes and round up to the nearest GB. You may round up further to add a buffer, such as rounding 11.6 GB to 16 GB.
- **Metadata**
  - Include the following, taken from the GOG page: Genre, Tags, Works on, Release date, and Company.
  - Tags do not all need to fit. Use the most relevant tags.
  - **Bundles:** use the bundle's release date. If GOG does not provide one, list the release dates of all games in the bundle. If all dates do not fit, list the release date of the latest game in the bundle instead.
- **What's included**
  - Always list the **GOG GALAXY Installer** first.
  - **Single games:** list the game and its most recent GOG patch, as Dread Templar does.
  - **Bundles:** list every game in the bundle. If the bundle includes sub-bundles, such as Tomb Raider I-III Remaster and Tomb Raider IV-VI Remaster, list only the sub-bundles instead of every individual game.
  - For every game listed, include its most recent GOG patch.
- **Bible verse**
  - Include a short, relevant Bible verse from the ESV translation.

## Pull request checklist

Before submitting, confirm each item:

- [ ] The game is sold on GOG.
- [ ] A front cover named `front.<extension>` is included, following the bundle rules if applicable.
- [ ] The ESRB rating is placed at the required position and kept at its original aspect ratio.
- [ ] The ESRB rating comes from `Ratings/`. If it was missing, it was added there as `<letter rating>.<extension>`.
- [ ] Publisher logos are named `<company>_logo.<extension>`, have no watermarks, and keep their aspect ratios.
- [ ] Publisher logos are transparent PNGs whenever possible.
- [ ] Publisher logos are spaced and positioned according to the rules above.
- [ ] The GOG preservation logo (`gpp-logo.png`) is 2 grid spaces down from the top of the spine, spans the spine width, and keeps its aspect ratio.
- [ ] The front image wraps across the spine to the beginning of the back cover.
- [ ] The full game title is on the spine, readable, and centered horizontally and vertically.
- [ ] The spine title is named `<game_name>_banner.<extension>`.
- [ ] The gameplay image is named `gameplay.<extension>`, is not transparent, and fills the upper half of the back cover.
- [ ] Three non-transparent flavor images are named `flavor_image<X>.<extension>`, sit 1 grid space below the gameplay image, and are spaced as described.
- [ ] The flavor images show normal gameplay with no spoilers, pause screens, or menus.
- [ ] The flavor text sits directly below the flavor images and comes from GOG or another official source.
- [ ] System requirements are in their own section, sourced from GOG or an official source, with at least one AMD and one NVIDIA card where listed.
- [ ] Storage is listed, and for bundles it is the rounded-up total of the installer sizes.
- [ ] Metadata includes Genre, Tags, Works on, Release date, and Company.
- [ ] What's included lists the GOG GALAXY Installer, the game or sub-bundles, and each latest GOG patch.
- [ ] A short ESV Bible verse is included.
