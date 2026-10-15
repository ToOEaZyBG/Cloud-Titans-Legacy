# Legacy of the Cloud Titans — 0.4.2-alpha

Tower artifact set and quests for Heroes III ERA/WoG by ToOEaZyBG.

**This build supports local testing. Network map placement, level component rewards and quests are disabled. Multiplayer support is not ready.**

The repository root is prepared for Heroes Launcher Mod Browser. Catalog submission and moderation are separate steps.

Third-party credits are retained in THIRD_PARTY.txt and script headers. No ownership of Heroes III or third-party components is claimed, and no blanket license for upstream materials is granted by this repository.

# Cloud Titans 0.4.2 — инсталация за втори тестер

Това е тестова версия за **локална игра**, с новите трудни задачи. Мрежовото придобиване на части и задачите са изключени. Двамата можете да тествате отделни локални игри; пакетът не обещава съвместна онлайн игра.

## Инсталация

1. В Heroes Launcher инсталирай ERA и обнови избрания ERA профил. Нужни са WoG, Era Erm Framework, WoG Scripts, Game Enhancement Mod, WoG Graphic Fix, Advanced Classes Mod и същият JS профил като на основния тестер. Виж TEST_PROFILE.json за списъка на активните модове и контролните суми на основните зависимости.
2. Затвори играта напълно. Разархивирай ZIP в главната папка на **ERA играта**, където е h3era.exe. Трябва да получиш `Mods/Cloud Titans Legacy - Local Test/mod.json`, без допълнителна вложена папка.
3. Отвори ERA Mod Manager и включи **Cloud Titans - EXPLORATION ALPHA** (папка Cloud Titans Legacy - Local Test). Провери версия **0.4.2-alpha**. Постави го след зависимостите, с по-висок приоритет от WoG Graphic Fix, ACM и JS.
4. Изключи други копия на Cloud Titans и помощника Cloud Titans - Lineage Test Army. Не включвай несъвместимите разширения от mod.json, особено тези, които заемат artifact IDs 450–458 или заменят emerald.cfg/artifact.def/ZOBJCTS.
5. Стартирай **нова локална random карта**, избери Tower. За награди при ниво включи WoG опция 126. От ниво 18 има шанс за част от сета; няма гарантиран предмет от сета на всяко ниво.

ZIP се разархивира, а Mod Manager включва мода. Това не е инсталация от публичния Mod Browser: модът още не е подаден там.

## Кратка проба

- Първи ден: съобщение за поставените по картата части; собствени сини/златни изображения и успешно вземане.
- Tower: бутон за допълнителни действия вдясно от името на града → превъртане надолу → Cloud Titans quests.
- Осем цели: 500 победи; 4000 магове; 10000 скелета; 100000 общи убийства; 2000 вампира; 1000 победи; 150 Behemoths/Ancient/Ghost; 10000 импове.
- Всяка награда: герой поне ниво 25 и всички обикновени сгради в същия Tower, включително Capitol, Mage Guild 5 и всички подобрени жилища. Skyship от Граала не е нужен. При липсващо условие награда не се дава.
- Обикновени битки, включително Auto Combat вътре в битката: броячите се увеличават само след победа и потвърден резултат. Проверете трите форми на Behemoths и че джиновете не увеличават новата задача.
- Сет: бонуси, сглобяване/разглобяване, Giant/Titan/Lord of Thunder, седмично +2, save/load и връщане на стойностите след сваляне.

Запиши версията, датата в играта и какво точно си направил при проблем. Запази сейв преди проблема и Debug файловете от съответната ERA инсталация. Не е нужен достъп до GitHub за ZIP инсталацията.

## Обновяване и премахване

Преди обновяване архивирай старата папка на мода. За чист тест използвай нова карта; старите получени награди остават получени. В стар сейв само новият Behemoth брояч започва от нула, останалият напредък се запазва. За премахване изключи мода през Mod Manager и използвай карта/сейв, който не зависи от него.
